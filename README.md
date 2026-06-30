# juwon1405.github.io

Personal site of **Bang Juwon (優心 / YuShin)** — DFIR &amp; Detection Engineering, Tokyo.

→ Live: https://juwon1405.github.io/

## Stack

- Single-page static site. No framework, no client-side build step.
- `index.html` ships HTML + CSS + JS inline. That's the whole thing.
- Local `assets/` images are used for Agentic-DART and public YuShin Trade / YuShin Watch showcase previews.
- Fonts via Google Fonts CDN: **Fraunces** (display serif), **Geist** (sans), **Geist Mono** (mono). `404.html` uses **Instrument Serif** + **JetBrains Mono**.
- `.nojekyll` is kept for safety, though the deploy workflow uploads the repo as a Pages artifact directly (Jekyll is not invoked).
- CI substitutes `__BUILD_DATE__` and `sitemap.xml`'s `<lastmod>` at deploy time.

## Layout

```
.
├── index.html      # the site
├── 404.html        # custom error page
├── assets/         # local preview images for showcase sections
├── .nojekyll       # bypass jekyll
├── robots.txt
├── LICENSE         # MIT
└── README.md
```

## Develop

Open `index.html` directly in a browser, or:

```bash
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy

Pushing to `main` is the deploy. GitHub Pages serves from the repo root.

## License

MIT — see [LICENSE](./LICENSE).
