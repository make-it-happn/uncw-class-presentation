# UNCW class presentation

Static HTML slides for the UNCW guest lecture (AI and entrepreneurship). Served as a single `index.html` with no build step.

## Live site

**Production:** https://uncw-class-presentation.vercel.app

Pushing to `main` on GitHub triggers a new Vercel production deploy (Git integration is connected).

## Repo

https://github.com/make-it-happn/uncw-class-presentation

## Local preview

* Open `index.html` in a browser (double-click or `open index.html` on macOS).
* Or from this directory: `python3 -m http.server 8765` then visit http://localhost:8765

## Editing

* Edit `index.html` directly. Keep each slide in a `.slide` block and follow the existing theme variables in `:root` if you change colors or type.
* Put images, logos, or other files under `assets/` and reference them with relative paths (for example `assets/logo.png`).
* After changes: commit and push to `main` for an automatic production deploy.

## Manual deploy (CLI)

If you need to deploy from your laptop without pushing:

```bash
cd /Users/mattcimino/Documents/Projects/mini-projects/uncw-class-presentation
npx vercel@latest --prod --yes
```

Requires a Vercel account and `npx vercel login` if not already logged in.

## Vercel project

Dashboard: https://vercel.com/matt-mattciminocs-projects/uncw-class-presentation

* **Framework:** Other (static). Root serves `index.html`.
* **Git:** Connected to `make-it-happn/uncw-class-presentation`, branch `main`.

## Optional: custom domain

In the Vercel project: Settings → Domains → add your domain and follow DNS instructions.

## Related notes in personal OS

Outline and talk context only: `personal-os` at `datasets/community/uncw/guest-lecture/outline.md`. The HTML deck lives only in this repo (no duplicate under `personal-os`).
