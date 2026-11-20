# Plottie landing page

Single static page: `index.html` (1174 lines). No build step.

## index.html map

- head/meta 1–28 · CSS `<style>` 29–749 · JSON-LD 750–829 · script 1102–1171
- CSS: vars `:root` 32–47 · nav 62–108 · buttons 110–143 · hero 148–194 · hero product frame 196–236 · section headings 238–262 · features 264–315 · how 317–354 · founder 356–383 · pricing 385–502 · FAQ 504–551 · waitlist 553–658 · footer 660–696 · responsive 718–748
- Markup: nav 833–846 · hero 851–859 · hero product frame 861–871 · features 873–909 · how 911–938 · founder 944–953 · pricing 955–1020 · FAQ 1022–1056 · waitlist 1058–1085 · footer 1089–1100

Line numbers drift after edits; re-check before relying on them.

## Design rules

- Dark-first. Colors are CSS variables in `:root` (lines 32–47): `--bg #1c1c1a`, `--bg2 #242422`, `--bg3 #2c2c2a`, `--text #e8e6de`, `--text2 #b0aea6`, `--text3 #9c9a92`, `--red #E24B4A`. Use the variables, not raw hex.
- Fonts: Instrument Serif for headings; Geist Mono for labels and chips; body is the site sans.
- Brand mark: a 7px red `#E24B4A` square dot (`.nav-logo-dot`, line 90).

## Copy rules

- No invented stats, testimonials, quotes, logos or prices. Use `<!-- TODO(juan): ... -->` placeholders instead.
- No EU or regional claims.
- Lead with one flat price, no per seat. Prices exclude VAT.

## Preview

`python3 -m http.server` in this folder, then open the printed localhost URL.

## Deploy

GitHub Pages serves `main`; merging to `main` is the production deploy. Juan merges. Never push to `main` or merge.
