# My Happy Bike (static site)

Static mirror of [myhappybike.com](https://www.myhappybike.com) for **Cloudflare Pages**.

## Cloudflare Pages settings

Cloudflare Pages → Connect Git → empty build command, output directory `/`, root `/`.

| Setting | Value |
|--------|--------|
| Build command | *(leave empty)* |
| Build output directory | `/` |
| Root directory | `/` |
| Framework preset | None |

No build step: HTML is served as-is from the repo root.

## Pages in this repo

- `/` — Journey of Hope / My Happy Bike home
- `/coffee/` — Coffee page
- `/home/` — Home page

Historically this site was **search-only** (no lead forms). Existing Universal Analytics property `UA-61762788-2` is retained in the HTML; do not invent a GA4 ID.

## Custom domain

A `CNAME` file with `myhappybike.com` is included for GitHub Pages compatibility. Attach the custom domain `myhappybike.com` later under the Cloudflare account `scott@creatingvaluellc.com` (Pages project settings; Cloudflare manages DNS at cutover — do not change live DNS until then).

## Local preview

```bash
npx serve .
# or: python3 -m http.server 8080
```
