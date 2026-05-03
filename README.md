# juwon1405.github.io

Personal site of **Bang Juwon (優心 / YuShin)** — DFIR &amp; Detection Engineering, Tokyo.

→ Live: https://juwon1405.github.io/

## Stack

- Single-page static site. No framework, no build step.
- `index.html` ships HTML + CSS + JS inline. That's the whole thing.
- Fonts via Google Fonts CDN: **Instrument Serif**, **JetBrains Mono**, **Noto Sans JP**.
- `.nojekyll` disables GitHub Pages' Jekyll pipeline so files are served as-is.

## Layout

```
.
├── index.html      # the site
├── 404.html        # custom error page
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
