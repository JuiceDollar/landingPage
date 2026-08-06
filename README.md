# landingPage

juicedollar.com. The former landing page has been removed and replaced by a static
notice: control over the protocol has been lost, JUSD can be swapped for USDT until
10 August 2026, 12:57 UTC, after which juicedollar.com and bapp.juicedollar.com are
shut down permanently.

## Contents

- `index.html` — the notice page
- `404.html` — identical content, served for any path that does not exist
- `_redirects` — redirects the paths of the former pages to `/`

## Deployment

Cloudflare Pages via GitHub Actions, `wrangler pages deploy .` from the repository root:

- `develop` → development project
- `main` → production project (juicedollar.com)

A push to `develop` also opens the release PR to `main` automatically.
