# Made Forever public website

Live: https://superjames33.github.io/made-forever-site/

Plain static HTML/CSS. No runtime packages, JavaScript, tracking, paid hosting, or build step. The public site lives entirely in `docs/`.

## Local preview

Run `python3 -m http.server 8765 --directory docs`, then open http://localhost:8765.

## Deploy / reproduce

GitHub Pages publishes the `/docs` folder of the `main` branch. In repository Settings → Pages, select Deploy from a branch, `main`, `/docs`. Commit and push changes to `main`; GitHub rebuilds and publishes automatically. No secrets or manual upload are required. Use the Pages deployment history to verify completion. Roll back by reverting the relevant commit and pushing the revert.

## Files

- `docs/index.html`: home, industry cards, contact section
- `docs/how-it-works.html`: six-step workflow and compatibility information
- `docs/privacy.html`, `docs/terms.html`: website policies
- `docs/assets/site.css`: responsive layout and branding
- `docs/assets/favicon.svg`, `docs/assets/social-preview.png`: branding and share preview
- `docs/404.html`: error page
- `docs/sitemap.xml`, `docs/robots.txt`: discovery metadata

All ordinary internal links are relative, so the site works at a GitHub project path and at a custom-domain root. The error page uses an absolute base. On domain activation, update canonical URLs, Open Graph URLs, sitemap, robots, and the 404 base to the verified custom-domain URL. Do not add a CNAME file before the domain connection is approved and ready.

## Contact

team@madeforever.live · 720-657-7188

Direct email and phone only. No form backend, account system, or sensitive-data collection. The workflow illustration is labeled as an example and does not simulate an actual connected system.
