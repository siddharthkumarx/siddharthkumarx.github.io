# Maintainers' notes

What each file is: `README.md`. This file holds the rules the pictures follow.

## Canvas rule (owner decision, 22 Nov 2026)

Every image's outermost background is `#F3F8F7`: never pure white `#FFFFFF`, never
dark `#0B1416`, never transparent with dark text. Cards inside stay `#FFFFFF` with
border `#E2EAE8` and radius 14px. A screenshot of a white page is shown framed: the
page as a card (radius 14, border `#E2EAE8`) on about 40 px of `#F3F8F7`.

- `assets/og.png`: the founder card sits on the canvas; its soft shadow fades out
  before the edge, so every edge pixel is exactly `#F3F8F7`. Keep it that way when
  you render a new one.
- Exceptions: the page background (`#FFFFFF` with `#F3F8F7` bands), the favicon and
  app-icon tiles (`favicon.ico`, `assets/img/icon.svg`, `icon-192.png`,
  `apple-touch-icon.png`, `logo-512.png`) and the founder photo.

Check before every commit (Node only, no packages):

```bash
node tests/check_canvas.cjs
```

It checks every edge pixel of every tracked PNG and the first `<rect>` fill of every
SVG, and fails on anything else outside the exceptions.
