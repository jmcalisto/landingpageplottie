# plottie.eu

Marketing site for Plottie. One static page, no build step.

## Preview locally

Open `index.html` in a browser, or run `python3 -m http.server` in this folder and go to http://localhost:8000.

## Deploy

GitHub Pages serves `main` directly, with the custom domain in `CNAME` (`www.plottie.eu`). There is no workflow or build. **Merging to `main` is the production deploy.** Make changes on a branch, open one PR, and let Juan merge.

## Files

- `index.html` — the whole site: markup, CSS and the small bits of JS.
- `founder.webp` — founder photo in the founder block.
- `roadmap-month-dark.webp`, `task-detail-dark.webp` — product screenshots (demo data only).
- `favicon.ico`, `plottie-favicon-16/32/192/512.png`, `apple-touch-icon.png`, `site.webmanifest` — favicon and app icon set. Replace them as a set, don't edit one alone.
- `robots.txt`, `CNAME` — crawler rules and the Pages domain.

## Design

Dark mode first. Colors are CSS variables at the top of `index.html` (`--bg #1c1c1a`, `--bg2 #242422`, `--bg3 #2c2c2a`, `--text #e8e6de`, `--red #E24B4A`). Change them there, not inline.

## Copy rules

- No invented stats, testimonials, logos or prices. Leave a `<!-- TODO(juan): ... -->` instead.
- No EU or regional claims. Lead with one flat price, no per seat.
- Prices exclude VAT.

## Open TODOs in the page

Search `index.html` for `TODO(juan)`: a real named quote, pilot numbers, the self-hosted repo URL, the Talk to us address, and the privacy and terms URLs.
