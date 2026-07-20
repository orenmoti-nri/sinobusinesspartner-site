# Sino Business Partner — Website

Static site. **No build step, no dependencies** (only Google Fonts via CDN).

## Files
- `index.html` — homepage (current version).
- `china-guide.html` — China Guide for business travelers.
- `_headers` — basic security headers for Cloudflare Pages.

## Deploy to Cloudflare Pages via GitHub
1. Create a new GitHub repo (e.g. `sinobusinesspartner-site`) and upload **all files in this folder to the repo root**.
2. Cloudflare dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git** → select the repo.
3. Build settings: **Framework preset = None**, **Build command = (leave empty)**, **Build output directory = /** (root).
4. **Save and Deploy** → you get a `*.pages.dev` preview URL.
5. **Custom domain:** in the Pages project → **Custom domains** → add `sinobusinesspartner.com` and `www.sinobusinesspartner.com`. As the domain already lives on Cloudflare, DNS is configured automatically.

## Updating the site
Edit the HTML, commit & push to GitHub — Cloudflare Pages redeploys automatically.

## Notes
- Fully self-contained: all graphics are inline SVG; no local image files.
- Internal links use `index.html` and `china-guide.html` (consistent for hosting).
