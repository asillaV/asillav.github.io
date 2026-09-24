# asillav.github.io — Data & Signal Processing Portfolio

Personal technical portfolio of Francesco Vallisa, Data & Signal Processing Engineer. It presents selected projects on industrial and sensor data — Python tooling, signal processing, data pipelines and dashboards — with a long-form CV (`cv.html`) and a detailed case study (`case-study.html`). The site stays lightweight and fast: plain HTML/CSS, no build step.

## Project Layout
- `index.html` — Landing page with hero, background, projects, process, and contact sections.
- `cv.html` — Standalone résumé with bilingual content (IT/EN), project grid, and skills matrix.
- `case-study.html` — CSV Analyzer case study (source text in `case-study.md`).
- `style.css` — Global theme, layout primitives, and responsive rules for all pages.
- `assets/` — Logos, screenshots, and other static media referenced by the pages.

## Getting Started
```bash
# launch a local preview on http://localhost:8000
python3 -m http.server 8000
```
Open the URL in your browser to iterate on copy, layout, or assets. For a Node-based preview you can also run `npx serve .`.

## Customization
- Update hero text and project cards directly in `index.html`.
- Adjust typography, color tokens, or grid breakpoints in `style.css`.
- Keep new assets optimized (WebP/PNG ≤1 MB) before placing them in `assets/`.
- All pages share `style.css` — test each page after editing shared styles.

## Deployment
The repository is configured for GitHub Pages:
1. Push to the `main` branch of `asillav/asillav.github.io`.
2. Ensure Pages is enabled on the `main` branch, root directory.
3. Changes go live within a few minutes at `https://asillav.github.io`.

If assets appear stale, trigger a cache refresh by touching the file (`git commit --allow-empty -m "Refresh site"`) and redeploy. For bespoke hosting, serve the static folder through any CDN or S3-style bucket with HTML/CSS MIME types.
