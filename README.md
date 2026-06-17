# KitKat QR landing page

A single static page that displays a QR code linking to:

<https://sparkling-flan-5a1cf0.netlify.app/kitkat-4-finger-milk-chocolate-41-5g/>

The QR is generated in the browser (self-contained), with a fallback to a QR
image API if the script can't load. No build step required.

## Files
- `index.html` — the page
- `netlify.toml` — Netlify config (publishes the repo root)

## Deploy

### Option A — Netlify drag & drop (no tools needed)
1. Go to <https://app.netlify.com/drop>
2. Drag the `kitkat-qr-page` folder onto the page.
3. Done — Netlify gives you a live URL.

### Option B — GitHub + Netlify (continuous deploy)
1. Create a repo on GitHub and push this folder (see commands below).
2. In Netlify: **Add new site → Import an existing project → GitHub**, pick the repo.
3. Publish directory: `.` (root). No build command needed.

```sh
git init
git add .
git commit -m "Add KitKat QR landing page"
git branch -M main
git remote add origin https://github.com/<you>/<repo>.git
git push -u origin main
```
