# AGENTS.md

## Cursor Cloud specific instructions

### Overview

This is a **static HTML website** — a Chinese online tools navigation portal (在线工具网). There is no build system, package manager, backend, database, or test suite. All JS/CSS libraries are vendored in `assets/`.

### Running the site

Serve the static files from the workspace root with any HTTP server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080/` in a browser. The entry point is `index.html`.

### Project structure

- `index.html` — Main single-page navigation site (~6100 lines)
- `404.html` — Simple 404 page
- `about/index.html` — About page
- `assets/css/` — Stylesheets (Bootstrap 4.3.1, custom styles, Fancybox, iconfont)
- `assets/js/` — JS libraries (jQuery 3.2.1, Bootstrap, LazyLoad, etc.)
- `assets/images/` — Images, logos, favicons
- `assets/fontawesome-5.15.4/` — Font Awesome icons

### Editing

- To modify links/tools: edit `index.html`
- To modify the about page: edit `about/index.html`

### Lint / Test / Build

There is no linting, automated testing, or build step configured for this project. The site is pure static HTML served as-is.
