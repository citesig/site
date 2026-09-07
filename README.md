# citesig.org — marketing site

Single-file static site for [citesig.org](https://citesig.org), deployed via **Cloudflare Pages** with automatic builds on push to `main`.

## What's here

- `index.html` — the entire site (self-contained HTML/CSS/JS, no build step)
- `favicon.png`, `apple-touch-icon.png`, `og-image.png` — brand assets (add if missing)

## Deploy

Cloudflare Pages watches this repo. Every push to `main` triggers a production deploy at citesig.org. No build command needed; output directory is the repo root.

To preview locally:

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Making changes

1. Edit `index.html` on a branch
2. Open a PR
3. Cloudflare Pages posts a preview URL on the PR
4. Merge to `main` → live at citesig.org within ~30 seconds

## Related repos

- [`citesig/spec`](https://github.com/citesig/spec) — protocol specification (CC BY 4.0) + reference vectors (MIT)
- [`citesig/verifier-extension`](https://github.com/citesig/verifier-extension) — Chrome MV3 verifier (MIT)

## License

MIT — see [LICENSE](./LICENSE). CiteSig™ is a trademark of Epic Sky, LLC.
