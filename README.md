# LBLM moodboard reference

Static, dependency-free reference page for the supplied `LBLM_Moodboard_Final.pdf` and corresponding original PNG. It reproduces the board's text and 25 color values as HTML. Arial matches the fonts embedded in the source PDF; this does not establish a final brand typeface. No unapproved logo variants are included.

- Public page: https://mimi-san.github.io/lblm-moodboard/
- Isolated repository: https://github.com/mimi-san/lblm-moodboard
- GitHub Pages source: `main`, repository root; HTTPS enforced.
- Original PNG and PDF: `assets/`, copied without modification.
- No JavaScript, third-party fonts, analytics, authentication or Shopify integration.
- `noindex, follow` requests no search indexing without blocking asset fetches. It is not access control: the page, assets and repository are public.

## Preview and maintenance

Run `python3 -m http.server 8094 --bind 127.0.0.1` here, then open http://127.0.0.1:8094/. Publish intentional changes by committing and pushing this isolated repository's `main` branch; GitHub Pages deploys automatically.

## Verification

Initial browser smoke covered a loaded 3600 × 2900 moodboard, all 25 HTML color values, direct PNG/PDF HTTP 200 downloads and desktop/mobile layouts down to 320 CSS pixels without horizontal overflow. Visual review found no blocking fidelity issues. After deployment, an unauthenticated public reader extracted all 25 color values; the public browser loaded the moodboard and fetched the original PNG (6,204,855 bytes) and PDF (2,376,571 bytes) with HTTP 200 and no credentials. Kittl ingestion itself was not run; publicly fetchable assets do not guarantee which assets Kittl will select.
