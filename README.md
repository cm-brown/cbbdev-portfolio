# cbbdev-portfolio

Source for [cbbdev.com](https://cbbdev.com), built with [Hugo](https://gohugo.io) and deployed on Cloudflare.

## Run locally

```sh
hugo server -D
```

## Add a project

Create `content/projects/<name>.md` with `title`, `summary`, `tags`, `repo`, optional `demo`, and `weight` (lower shows first).

## Deploy (one-time setup)

cbbdev.com is already on Cloudflare, so Cloudflare Pages is the simplest host.

1. Cloudflare dashboard → Workers & Pages → Create → Pages → Connect to Git → pick the repo.
2. Build settings:
   - Framework preset: **Hugo**
   - Build command: `hugo --minify`
   - Output directory: `public`
   - Environment variable: `HUGO_VERSION` = `0.167.0` (the site needs 0.158 or newer)
3. After the first deploy: the Pages project → Custom domains → add `cbbdev.com` (and `www.cbbdev.com`).

Your Cloudflare Tunnel subdomains (e.g. `fictionaluni.cbbdev.com`) keep working. Only the apex and `www` point to Pages.

After that, every push to `main` deploys, and pull requests get preview URLs.
