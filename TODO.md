# Sudoku — hosting TODO

Product docs: [`README.md`](./README.md). Workspace migration: [rasok.at docs/TODO.md](https://github.com/JavanXD/rasok.at/blob/main/docs/TODO.md).

## Live

- Canonical: `https://sudoku.rasok.at/` — Worker **`sudoku`** on **`rasok.at - Dev`**
- Legacy: `https://sudoku.javan.de/` → **301** path+query → `https://sudoku.rasok.at/` (zone Single Redirect on `javan.de`, enabled)
- Platform URLs: `workers_dev` / `preview_urls` disabled
- GitHub: repo homepage `https://sudoku.rasok.at/`; **GitHub Pages disabled** (hosting is Workers, not Pages)

## Deploy notes

- Static assets from `public/` (`wrangler.jsonc`); `account_id` → Dev.
- Workspace path contains `*` — deploy from a `/tmp/…` copy.
- GHA secrets `CLOUDFLARE_API_TOKEN` + `CLOUDFLARE_ACCOUNT_ID` → Dev (`builtby-rasok-at.env`)

## Follow-ups

- [x] Move Worker to **`rasok.at - Dev`** with zone `rasok.at`
- [x] Enable redirect → drop `sudoku.javan.de` custom domain / Javan Worker *(redirect already live; no Javan `sudoku` script; DNS `AAAA 100::` proxied for redirect-only)*
- [x] Update `javan.de` sitemap / `projects.javan.de` links to `sudoku.rasok.at` *(projects already rasok.at; removed `sudoku.javan.de` from `sitemap-links.json` 2026-09-10)*
- [x] Add GHA secrets for `.github/workflows/deploy.yml` (Dev account) *(2026-09-10)*
- [x] GitHub Pages: remove `sudoku.javan.de` custom domain; disable Pages *(2026-09-10 — cannot attach `sudoku.rasok.at` to Pages without stealing Worker DNS)*
