# Sorry I'm Late

An Atlanta traffic excuse generator, live at [late.jakethings.com](https://late.jakethings.com). Part of [jakethings.com](https://jakethings.com).

- `public/` is the site: one HTML file, no build step, no dependencies.
- Each excuse has a shareable link (the `#` part of the URL picks the pieces).
- Every push to `main` deploys to the Cloudflare Pages project `jakethings-late` through `.github/workflows/deploy.yml`.
- The repo needs two Actions secrets: `CLOUDFLARE_API_TOKEN` (Pages Edit) and `CLOUDFLARE_ACCOUNT_ID`.
- Bump the version in `public/index.html` (the `version` meta tag and the footer) with every change.
