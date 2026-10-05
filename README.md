# Robby Satya Wicaksana — Portfolio

Static site (HTML + CSS + vanilla JS, no build step, no dependencies besides Google Fonts).

## Files
`index.html` (all markup, CSS, JS) · `favicon.svg` · `sitemap.xml` · `robots.txt` · `.nojekyll`

## Run locally
Open `index.html`, or: `python3 -m http.server 8000` then visit http://localhost:8000

## Deploy to GitHub Pages
1. Create a repo named `robbysatya.github.io` (user site) and push these files to `main`.
2. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Site goes live at `https://robbysatya.github.io/`.

Using a different repo name (project site)? The URL becomes `https://robbysatya.github.io/<repo>/`. Asset paths are relative so it still works, but update the canonical, `og:url`, `sitemap.xml` and `robots.txt` URLs.

## Before publishing
- The PaperlessHospital.id card in `#projects` still says "Project details coming soon" since there's no public link or screenshot for it — add one if it becomes available.
- Project previews are hotlinked straight from each live site's own images (`<img>` with an `onerror` fallback to a text tile if a link ever breaks or an image moves). Swap in your own screenshots any time for more control.
- Add `og-image.png` (1200×630) and an `og:image` meta tag for rich link previews.
- Confirm the date ranges in the career timeline against your CV.
- alascobek.com's own footer credits "ruparagam" as builder — worth double-checking before listing it as your own work.

## Theme & language
Dark/light theme (follows system preference by default) and EN/ID language toggle live in the nav; both choices are saved in `localStorage`. Indonesian text is the `ID` dictionary at the top of the script in `index.html` (English text is the source and key). When you add new English text, add its Indonesian pair there.
