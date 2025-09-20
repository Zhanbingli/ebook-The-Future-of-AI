# 技术改造报告：GitBook 构建与发布流水线

## 背景
- 原仓库使用全局 `gitbook-cli`（GitBook 3.2.3）进行构建，在现代 Node.js（v24）环境下触发 `graceful-fs` 回调崩溃。
- GitHub Actions 同样依赖该 CLI，导致 CI 构建失败并阻塞 GitHub Pages 发布。

## 目标
1. 在本地与 CI 环境内提供可持续的构建工具链。
2. 调整仓库结构以兼容新工具，并保持文档导航正确。
3. 恢复自动部署到 `gh-pages` 分支的发布流程。

## 主要改动
### 构建工具链
- 引入 `honkit`（GitBook 开源分支，支持新 Node 版本），通过 `package.json` 中的脚本暴露 `npm run gitbook` / `npm run serve`（`package.json`）。
- 新建 `.gitignore` 排除 `_book/` 与 `node_modules/`，避免构建产物与依赖污染仓库（`.gitignore`）。

### 目录与配置
- 约定 `docs/` 作为内容根目录：`book.json` 添加 `root` 字段并指向 `./docs`，`structure.readme` / `structure.summary` 分别指向 `README.md` 与 `SUMMARY.md`（`book.json`）。
- 将原 `docs/index.md` 重命名为 `docs/README.md`，并同步更新 `docs/SUMMARY.md` 导航路径，确保 Honkit 能识别首页与章节。
- 更新根目录 `README.md` 的使用说明：
  * 依赖安装：要求 Node.js 20 LTS，使用 `npm ci`/`npm install`。
  * 预览与构建命令：`npm run serve`、`npm run gitbook`。
  * 调整开发者指引，保持与新结构一致（`README.md`）。

### CI/CD 与部署
- 调整 GitHub Actions Workflow：
  * Node 版本升级至 20；
  * 使用 `npm ci` 安装依赖；
  * 调用 `npm run gitbook` 生成 `_book`；
  * `peaceiris/actions-gh-pages@v4` 发布静态站点。
- 新增 `permissions.contents: write`，允许内置 `GITHUB_TOKEN` Push 至 `gh-pages` 分支（`.github/workflows/gitbook.yml`）。

## 测试与验证
- 本地执行 `npm run gitbook`，Honkit 成功生成 18 个页面，无错误日志（`npm run gitbook`）。
- GitHub Actions 在最新 push 后应完成构建并成功 Push；如仍失败，可在 Actions 日志确认 `peaceiris/actions-gh-pages` 步骤状态。

## 运行与发布指引
1. **本地预览**：
   ```bash
   npm ci           # 首次或依赖更新后执行
   npm run serve    # 打开 http://localhost:4000
   ```
2. **静态构建**：`npm run gitbook`，产物位于 `_book/`。
3. **推送发布**：`git push` 触发 workflow，自动发布到 `gh-pages`。
4. **访问地址**：`https://<GitHub用户名>.github.io/<仓库名>/`，仓库设置需将 Pages 分支配置为 `gh-pages`。

## 已知事项与后续建议
- `_book/` 与 `node_modules/` 已在 .gitignore 中忽略，若需手动部署请使用 `npm run gitbook` 重新生成。
- 若访问 Pages 出现 404，可能是 workflow push 被拒绝或 Pages 分支未指向 `gh-pages`；需查看最新 Actions run。
- 建议定期运行 `npm audit` 关注低风险漏洞，并在 Honkit 发布新版本时同步升级。
- 如需扩展主题/插件，可通过 `book.json` 的 `plugins` 字段集中管理。

## 参考命令
```bash
# 安装依赖
npm ci

# 开发预览
npm run serve

# 生成静态站点
npm run gitbook
```
