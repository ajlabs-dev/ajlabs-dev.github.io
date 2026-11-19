# A.J Labs Website — Static Edition

This is a production-ready static website. It contains no PHP, TypeScript, Node runtime requirement, or build step. The browser loads the included HTML, JavaScript bundle, stylesheet, and assets directly.

## Run locally

No build or install is needed. On Windows, double-click `start-site.bat`. On macOS/Linux, run `./start-site.sh` from this folder. The scripts start a local static file server using Python 3.

Alternatively, start any static file server. For example:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>. Do not open `index.html` directly as a `file://` URL; serve it over HTTP so root-relative assets and browser routing work correctly.

## Deploy

Upload the contents of this directory to any static hosting provider (GitHub Pages, Netlify, Cloudflare Pages, S3, or a standard web server). No install, compile, PHP runtime, or server-side application is required. All files are intentionally stored directly in this project-root folder; keep them together, including the JavaScript, stylesheet, image files, `robots.txt`, and `sitemap.xml`.

The contact form validates the inquiry and opens a pre-addressed email draft in the visitor's default mail application; it does not send email from a server.
