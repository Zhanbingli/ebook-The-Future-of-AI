# The Future of AI: Insights from Industry Leaders

This repository contains the GitBook source for the anthology "The Future of AI", featuring interviews and talks from founders and researchers pushing the frontier of artificial intelligence.

## Project layout

- `book.json` defines the GitBook metadata and points to the primary entry file at `docs/index.md`.
- `SUMMARY.md` lists every chapter in reading order and drives the left-hand navigation.
- `docs/index.md` provides the title page; additional sections (foreword, epilogue, conclusion) live directly in `docs/`.
- `docs/chapters/` holds one Markdown file per numbered chapter, already split from the source manuscript.

## Getting started

1. Install Node.js (LTS) and npm if you have not already.
2. Install the GitBook CLI globally: `npm install -g gitbook-cli`.
3. From the project root, run `gitbook install` to pull any required plugins (none are specified yet, but the command is harmless).

## Local preview

Run `gitbook serve` to build the book and open a preview at `http://localhost:4000`.

## Static build

Run `gitbook build` to generate the static website in the `_book/` directory for deployment to GitHub Pages, Netlify, or any static host.

## Updating content

- Edit or replace the files under `docs/chapters/` to update individual interviews.
- Update `SUMMARY.md` if you add, remove, or rename sections so navigation stays in sync.
- Regenerate the book with `gitbook serve` or `gitbook build` to verify formatting before publishing.
