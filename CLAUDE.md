# Aden Mina portfolio

One-page resume site for Aden Mina, built on the Draco HTML resume template. Plain HTML, CSS and jQuery. No package manager, no build step, no tests.

## Commands

| Task | Command | Notes |
| --- | --- | --- |
| Local preview | `python3 -m http.server 8000` | Then open http://localhost:8000. Also in `.claude/launch.json` as `site` |

## Layout

| Path | What it is |
| --- | --- |
| `index.html` | The whole page: nav, about, education, experiences, skills |
| `css/custom.min.css` | Site styles the page loads. `css/custom.css` is the unminified copy |
| `css/kube*.css`, `js/kube*.js` | Kube framework from the template |
| `scss/` | Template SCSS sources. Nothing compiles them here, so edits do not reach the page unless you rebuild `custom.css` and `custom.min.css` by hand |
| `js/site.js` | Smooth scroll for in-page nav links |
| `img/` | Headshot, background, favicon |

## Conventions

- Keep the Draco template credit and its CC BY-NC-SA 4.0 license notice (in `README.md` and the CSS headers).
- `index.html` mostly uses tabs; match the block you edit.

## Verify a change

Serve the folder, load the page, and check the browser console for missing files. Check phone width (about 390px) for sideways scroll.

## Deploy risk

GitHub Pages serves the `master` branch root at https://patrickking67.github.io/adenmina-portfolio/. Every push to `master` goes live.
