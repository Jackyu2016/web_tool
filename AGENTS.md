# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **fully static, client-side website** (an HTML-based URL navigation/bookmark directory). There is **no backend, database, build step, or package manager** — see `README.md`. The entire product is `index.html` plus the `about/` and `assets/` directories.

### Running the app (development)

Serve the repository root with any static HTTP server, then open the site in a browser:

```bash
python3 -m http.server 8000   # serves http://localhost:8000/
```

- Entry point: `index.html` (`/`). Other pages: `/about/`, `/404.html`.
- No dependencies to install and nothing to compile; just edit the HTML/CSS/JS and refresh the browser.
- Content (the links shown on the page) is hardcoded directly in `index.html`; the About page lives in `about/index.html`.

### Lint / Test / Build

There are **no lint, test, or build scripts** in this repo (no `package.json`, no Makefile, no CI config). Validation is done by serving the site and checking it renders/behaves correctly in a browser.
