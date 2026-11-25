# CV — Daniil Lazarev

Single-page-per-side resume (two A4 pages), published with GitHub Pages in two
languages. The visual identity is a printed-circuit-board theme — soldermask
green and copper — set in Unbounded (display) and Golos Text (body).

| | Live | PDF |
|---|---|---|
| 🇷🇺 Russian | https://ewener-daniil131.github.io/cv/ | [cv.pdf](cv.pdf) |
| 🇬🇧 English | https://ewener-daniil131.github.io/cv/en/ | [en/cv.pdf](en/cv.pdf) |

A RU / EN switch sits in the top-right of each page (hidden when printed).

## Files

```
index.html      Russian resume
en/index.html   English resume
cv.css          shared styles for both
cv.pdf          Russian PDF (regenerate with the command below)
en/cv.pdf       English PDF
```

## Regenerating the PDFs

Rendered from the HTML with headless Chromium:

```bash
chromium --headless --no-sandbox --virtual-time-budget=8000 \
  --no-pdf-header-footer --print-to-pdf=cv.pdf    file://"$PWD"/index.html
chromium --headless --no-sandbox --virtual-time-budget=8000 \
  --no-pdf-header-footer --print-to-pdf=en/cv.pdf file://"$PWD"/en/index.html
```
