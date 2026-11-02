# Accrue assets: which file to use

Open `index.html` in a browser for previews. Version 2.0, 30 October 2026.

## HexDocs, the README, documents and slides on a light background

- `logo/accrue-lockup-light.svg`

## The same on Ledger Green or another dark background

- `logo/accrue-lockup-dark.svg`

## One-color printing, engraving, embroidery

- `logo/accrue-lockup-mono-ledger-green.svg`
- `logo/accrue-lockup-mono-paper.svg`

## The symbol alone: avatars, the Accrue Admin sidebar, stickers

- `logo/accrue-symbol-light.svg`
- `logo/accrue-symbol-dark.svg`
- `logo/accrue-symbol-mono-ledger-green.svg`

## 64 px and below: the symbol drawn for each size (use the file for the size)

- `logo/accrue-symbol-16-light.svg`
- `logo/accrue-symbol-16-dark.svg`
- `logo/accrue-symbol-24-light.svg`
- `logo/accrue-symbol-24-dark.svg`
- `logo/accrue-symbol-32-light.svg`
- `logo/accrue-symbol-32-dark.svg`
- `logo/accrue-symbol-48-light.svg`
- `logo/accrue-symbol-48-dark.svg`
- `logo/accrue-symbol-64-light.svg`
- `logo/accrue-symbol-64-dark.svg`

## The closing line as a graphic (titles, totals, slides)

- `logo/accrue-closing-line-light.svg`
- `logo/accrue-closing-line-dark.svg`

## App tile: Hex, Livebook, GitHub, avatars

- `icon/accrue-tile.svg`
- `icon/accrue-tile-1024.png`
- `icon/accrue-tile-512.png`
- `icon/accrue-tile-64.png`

## Browser tab, HexDocs favicon and home screen

- `icon/favicon.svg`
- `icon/favicon-32.png`
- `icon/favicon-16.png`
- `icon/accrue.ico`
- `icon/apple-touch-icon-180.png`

## GitHub social preview and avatars

- `social/accrue-social-preview-1280x640.png`
- `social/accrue-avatar-1024.png`

## Sounds: raw WAVs for sound designers; MP3s mastered for speakers, for the web and videos

- `sound/accrue-close.wav`
- `sound/accrue-confirm.wav`
- `sound/listening/accrue-close.mp3`
- `sound/listening/accrue-confirm.mp3`

## The logo animation with its sound, for videos and talks

- `motion/accrue-logo-animation.mp4`
- `motion/accrue-logo-animation.webm`

## The photo grade (a LUT) and the example photos, with licenses

- `imagery/accrue-ledger-daylight.cube`
- `imagery/README.md`

## Fonts for design apps (install) and the web

- `fonts/variable/`
- `fonts/static/`
- `fonts/web/`

## Colors (code colors included), type and motion values for Accrue Admin’s theme and HexDocs

- `../tokens.json`
- `code/accrue-exdoc.css`

## The whole brand as data, or as text for an AI assistant

- `../brand.json`
- `../BRAND.md`

## This book to print or send, a one-page summary, and a visual guide to every file

- `../accrue-brand-book.pdf`
- `../accrue-one-page.pdf`
- `index.html`

All logo SVGs are transparent, outlined (no fonts needed) and use the exact brand colors. `-light` files are colored for a light background, `-dark` for a dark one. The symbol is drawn separately for 16, 24, 32, 48 and 64 px: use the file for the size you need, at exactly that size, and the plain symbol file above 64 px. `accrue.ico` holds 16 to 256 px. Avatars are square: platforms crop them to circles themselves. Sounds: 48 kHz mono WAV, Close at -20 LUFS and Confirm at -23 LUFS (integrated, ITU-R BS.1770). Fonts: SIL Open Font License 1.1 (see `fonts/OFL-*.txt`); `variable/` holds every weight in one file, `static/` one file per named weight (IBM Plex Mono ships as static files only), `web/` Latin WOFF2 subsets with a `fonts.css`.
