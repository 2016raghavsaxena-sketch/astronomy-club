# Astronomy Club — Static Site

## Admin passphrase (client-only)
Default passphrase = **stargazer** (demo). Change it via `ADMIN_SHA256` in `assets/app.js` (see README in chat).

## Quick start
- Open `index.html` locally to preview.
- Events load from **local draft** (if any) → `data/events.json` → stub.
- Click **🔒 Manage Events (local)** → enter passphrase → edit events.
- Click **Download JSON** to save `events.json` and commit it.

## Deploy

### GitHub Pages (no build)
1. Create a new repo (e.g., `astronomy-club-site`) and push these files.
2. Add `.nojekyll` at repo root (included).
3. Enable Pages: **Settings → Pages → Deploy from a branch**. Select `main`, `/ (root)`.
4. Optional: Use the included GitHub Actions workflow for auto-deploy on push.

### Netlify (easiest)
- Drag & drop this folder at https://app.netlify.com/drop — done.
- Or connect your Git repo. Build command: _none_. Publish directory: `/`.

### Custom domain
- GitHub Pages: add your domain in Pages settings; create a `CNAME` file with your domain.
- Netlify: add domain in Site settings → Domain management; update DNS per Netlify instructions.

## Space Fact of the Week
Edit `FACTS` in `assets/app.js`. Shown fact is `ISO week number % FACTS.length`.
