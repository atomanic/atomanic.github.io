# atomano.com — Personal Academic Website

This repository contains the static files for **atomano.com** (André Tomano).

## Quick start (GitHub Pages)

1. Create a new repository on GitHub named **atomanic.github.io** (public).
2. Upload all files from this folder to the repository root (including `CNAME`). Commit to `main`.
3. In the repo: Settings → Pages → **Custom domain** → enter `atomano.com`. Check **Enforce HTTPS** once available.

> If GitHub removes/overwrites `CNAME`, simply re-add it with `atomano.com` as the only line.

## DNS at united-domains

Create/verify the following records for your domain:

**Apex (`atomano.com`)** — A records (add all four):

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

Optional (IPv6): AAAA records (add all four)

- 2606:50c0:8000::153
- 2606:50c0:8001::153
- 2606:50c0:8002::153
- 2606:50c0:8003::153

**Subdomain (`www.atomano.com`)** — CNAME record:

- Host: `www`
- Value: `atomanic.github.io`

> DNS changes can take time to propagate (usually minutes, sometimes up to 24–48h).

## Structure

- `index.html` — main page
- `styles.css` — site styles (no frameworks, fast and lightweight)
- `assets/Andre-Tomano-CV-2025-05.pdf` — your current CV (linked from the homepage)
- `404.html` — not-found page
- `CNAME` — tells GitHub Pages the custom domain

## Edit content

All content lives in `index.html`. Update sections as needed (Research, Teaching, Talks).

## Local preview

Open `index.html` directly in your browser, or serve with a simple server:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000
