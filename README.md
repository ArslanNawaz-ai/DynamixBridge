# Dynamix Bridge website

Static multi-page site, deployed to GitHub Pages by `.github/workflows/static.yml`.

## Structure
- `index.html`, `about.html`, `contact.html`, `404.html`
- `services/` — offerings (managed services, staff augmentation, custom development, web & mobile, consulting)
- `dynamics-365/`, `power-platform/`, `microsoft-365/`, `azure/`, `fabric/` — one overview page (`index.html`) and one page per product
- `assets/site.css` (styles), `assets/site.js` (menus, tabs, form), `assets/data.js` (generated menu data)
- `icons/` — product logos

## Editing
Pages are generated. Change text in `_build/content_tech.py` or `_build/content_services.py`
(or templates in `_build/build.py`), then run from the repo root:

    python _build/build.py

Commit the regenerated files. If you move to a custom domain, update `SITE_URL` in `_build/build.py` and rebuild.
