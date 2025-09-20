# The Future of AI: Insights from Industry Leaders

This repository contains the GitBook source for the anthology "The Future of AI", featuring interviews and talks from founders and researchers pushing the frontier of artificial intelligence.

## Project layout

- `book.json` defines the GitBook metadata and sets `docs/` as the content root for Honkit/GitBook.
- `docs/SUMMARY.md` lists every chapter in reading order and drives the left-hand navigation.
- `docs/README.md` provides the title page; additional sections (foreword, epilogue, conclusion) live directly in `docs/`.
- `docs/chapters/` holds one Markdown file per numbered chapter, already split from the source manuscript.

## Getting started

1. Install Node.js 20 LTS (includes npm) if you have not already.
2. From the project root, run `npm ci` to install dependencies (or `npm install` when developing locally).
3. Use the scripts below to preview or build as needed.

## Local preview

Run `npm run serve` to build the book and open a preview at `http://localhost:4000`.

## Static build

Run `npm run gitbook` (alias for `npx honkit build`) to generate the static website in the `_book/` directory for deployment to GitHub Pages, Netlify, or any static host.

## Updating content

- Edit or replace the files under `docs/chapters/` to update individual interviews.
- Update `docs/SUMMARY.md` if you add, remove, or rename sections so navigation stays in sync.
- Regenerate the book with `npm run serve` or `npm run gitbook` to verify formatting before publishing.
