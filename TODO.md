# Sudoku — hosting TODO

Product docs: [`README.md`](./README.md). Workspace migration: [rasok.at docs/TODO.md](https://github.com/JavanXD/rasok.at/blob/main/docs/TODO.md).

## Live

- Canonical: `https://sudoku.rasok.at/` — Worker **`sudoku`** on **`rasok.at - Dev`** (smoked 2026-08-31)
- Alias until cutover: `https://sudoku.javan.de/` — still on Javan Worker `sudoku`
- Platform URLs: `workers_dev` / `preview_urls` disabled
- Redirect staged **disabled**: `76fca8bb6e8843e7b612f91067fcf89d` (`sudoku.javan.de` → `sudoku.rasok.at`)

## Deploy notes

- Static assets from `public/` (`wrangler.jsonc`); `account_id` → Dev.
- Workspace path contains `*` — deploy from a `/tmp/…` copy.

## Follow-ups

- [x] Move Worker to **`rasok.at - Dev`** with zone `rasok.at`
- [ ] Enable redirect → drop `sudoku.javan.de` custom domain / Javan Worker
- [ ] Update `javan.de` sitemap / `projects.javan.de` links to `sudoku.rasok.at`
- [ ] Add GHA secrets for `.github/workflows/deploy.yml` (Dev account)
