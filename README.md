# Sticker Studio

Mobile PWA for generating transparent-background text stickers.

## Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "Sticker Studio PWA"
gh repo create sticker-studio --public --source=. --push
# or without the gh CLI:
# git remote add origin https://github.com/<you>/sticker-studio.git
# git branch -M main && git push -u origin main
```

Then: repo Settings > Pages > Source "Deploy from a branch" > branch `main`, folder `/docs` > Save.

The app lands at `https://<you>.github.io/sticker-studio/`.

## Install on iPhone

Open that URL in Safari > Share > Add to Home Screen. Full screen, and it works offline after the first load.

## Note

The app is served from the repo root (`index.html`) **and** from `/docs`, so either GitHub Pages folder setting works.

## Files

- `docs/index.html` — the app
- `docs/support.js` — runtime
- `docs/manifest.webmanifest`, `docs/sw.js`, `docs/icon-*.png` — PWA plumbing
- `docs/.nojekyll` — stops Jekyll from touching the files
