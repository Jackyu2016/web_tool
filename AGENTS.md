# AGENTS.md

This file gives coding agents a quick, practical guide for working in this repository.

## Project Overview

- Type: static website (no build system required).
- Purpose: online navigation page built with HTML/CSS/JS.
- Primary entrypoint: `index.html`.
- Secondary page: `about/index.html`.

## Repository Map

- `index.html` - main navigation page and link data.
- `about/index.html` - about page content.
- `assets/` - static assets (icons, styles, scripts, images).
- `README.md` - usage, deployment, and customization notes.

## Working Rules for Agents

1. Keep changes minimal and targeted to the requested task.
2. Preserve existing structure and relative paths in HTML files.
3. Prefer editing existing files instead of introducing new tooling.
4. Do not add framework/build dependencies unless explicitly requested.
5. Keep text/content style consistent with the surrounding file.

## Validation Checklist

After making changes:

1. Open `index.html` in a browser and confirm the page renders.
2. If links were edited, verify they navigate correctly.
3. If assets were changed, confirm there are no missing file references.
4. Run a quick repo sanity check:
   - `git status`
   - optional search for accidental placeholders: `rg "TODO|FIXME|PLACEHOLDER"`

## Deployment Notes

- Deploy by copying repository files to a web server.
- The site can also be previewed locally by serving the repo root (for example with a basic HTTP server).
