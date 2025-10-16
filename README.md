# asillav.github.io — Automation & Data Portfolio

A single-page portfolio that showcases Francesco Vallisa’s automation and data projects. The site focuses on clear messaging, lightweight assets, and fast load times so prospects can quickly grasp expertise in Python tooling, industrial data workflows, and rapid prototyping. It ships with a dedicated CV page (`cv.html`) for long-form experience details.

## Project Layout
- `index.html` — Landing page with hero, services, featured projects, process, and contact sections.
- `cv.html` — Standalone résumé with bilingual content, project grid, and skills matrix.
- `style.css` — Global theme, layout primitives, and responsive rules for both pages.
- `assets/` — Logos, screenshots, and other static media referenced by the pages.

## Getting Started
```bash
# launch a local preview on http://localhost:8000
python3 -m http.server 8000
```
Open the URL in your browser to iterate on copy, layout, or assets. For a Node-based preview you can also run `npx serve .`.

## Customization
- Update hero text, service bullets, and project cards directly in `index.html`.
- Adjust typography, color tokens, or grid breakpoints in `style.css`.
- Keep new assets optimized (WebP/PNG ≤1 MB) before placing them in `assets/`.
- Portfolio and CV share classes—test both pages after editing shared styles.

## Deployment
The repository is configured for GitHub Pages:
1. Push to the `main` branch of `asillav/asillav.github.io`.
2. Ensure Pages is enabled on the `main` branch, root directory.
3. Changes go live within a few minutes at `https://asillav.github.io`.

If assets appear stale, trigger a cache refresh by touching the file (`git commit --allow-empty -m "Refresh site"`) and redeploy. For bespoke hosting, serve the static folder through any CDN or S3-style bucket with HTML/CSS MIME types.
