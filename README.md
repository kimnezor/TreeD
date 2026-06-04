# TreeD™ Hybrid Tree Inventory — Landing Page

An interactive landing page for PlanIT Geo's TreeD™ product, featuring a
canvas-driven LiDAR "street sweep" hero (drag to look, move to scan, click to
pulse) with live tree-inventory data tags.

## Files

| File | Purpose |
|------|---------|
| `index.html` | **Deploy this.** Fully self-contained — all assets (logo, styles, scripts) are inlined. Works offline and on any static host with zero configuration. |
| `source.html` | The editable, un-bundled source (references the PlanIT Geo logo by URL). Edit this, then re-bundle if you want a new `index.html`. |
| `.nojekyll` | Tells GitHub Pages to serve files as-is (skip Jekyll processing). |

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `treed-landing`).
2. Add these files to the repo root and push:
   ```bash
   git init
   git add .
   git commit -m "TreeD landing page"
   git branch -M main
   git remote add origin https://github.com/<you>/treed-landing.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment**.
   - Source: **Deploy from a branch**
   - Branch: **main** / **/ (root)** → Save
4. Wait ~1 minute. Your site will be live at
   `https://<you>.github.io/treed-landing/`.

> Because `index.html` is self-contained, no build step is required.

## Custom domain (optional)

Add a `CNAME` file at the repo root containing your domain (e.g.
`treed.example.com`), then point a DNS CNAME record at `<you>.github.io`.
