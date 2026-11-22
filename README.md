# siddharthkumar.com

The founder card of Siddharth Kumar, Founder of SteadyData. One screen that points to [steadydata.co](https://steadydata.co), where the offer, pricing, FAQ and case studies live.

Plain HTML and CSS on GitHub Pages: no build step, no scripts, no forms, no external requests.

| Path | What it is |
|---|---|
| `index.html` | The founder card, with ProfilePage structured data |
| `404.html` | Page shown for broken links (not indexed) |
| `assets/style.css` | All styles (light system v1); bump `?v=` in both HTML files after a change |
| `assets/fonts/` | Plus Jakarta Sans, Latin subset, weights 400 to 700 (SIL Open Font License) |
| `assets/img/siddharth-kumar.webp` | Photo, 800 px; `siddharth-kumar-400.webp` is the 400 px copy |
| `assets/og.png` | Link preview picture, 1200 × 630 |
| `favicon.ico`, `assets/img/icon.svg`, `assets/img/apple-touch-icon.png`, `assets/img/icon-192.png`, `assets/img/logo-512.png`, `site.webmanifest` | The SteadyData mark, the same icon set as steadydata.co (copied from its repo, not edited here) |
| `llms.txt` | Short plain-text summary for AI assistants |
| `robots.txt`, `sitemap.xml` | Crawler rules and the page list |
| `docs/maintainers.md`, `tests/check_canvas.cjs` | The canvas rule for every picture, and its check (`node tests/check_canvas.cjs`) |
| `CNAME` | Serves this site at siddharthkumar.com |
| `.nojekyll` | Serves the files exactly as they are |

`/ecommerce-price-monitor/`, `/job-postings-pipeline/` and `/cross-store-price-comparison/` are published from their own repositories, so those folders must never be created here.

## Changing the photo

Replace both photo files with square WebP images of the same names (800 × 800 and 400 × 400), then render a new `assets/og.png` with the same photo, on the `#F3F8F7` canvas (`docs/maintainers.md`).
