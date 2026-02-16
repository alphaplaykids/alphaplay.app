# AlphaPlay™ Game Generator

**28 kinesthetic spelling games in 37 languages.**

Students wear letter pinnies and physically spell words — turning spelling practice into full-body, team-based play.

## What It Does

AlphaPlay™ generates ready-to-run spelling games where players wear letter vests (pinnies) and arrange themselves to spell words. The app supports 37 languages with language-specific letter sets and dual-letter pairings.

## Features

- 28 unique game formats (relay races, tag games, team challenges, etc.)
- 37 language support with proper character sets
- Offline-capable PWA — works without internet after first load
- Mobile-first responsive design
- Sound effects and visual feedback
- Print-ready game cards and setup instructions

## Tech Stack

Single-file PWA — no build step, no dependencies, no framework.

- `index.html` — entire app (HTML + CSS + JS + embedded language database)
- `sw.js` — service worker for offline support
- `manifest.json` — PWA manifest

## Running Locally

Serve from any static file server:

```bash
# Python
python3 -m http.server 8000

# Node
npx serve .
```

Then open `http://localhost:8000`.

## Deployment

Push to any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages). No build step required.

For GitHub Pages: enable Pages in repo settings → set source to `main` branch, root directory.

## File Structure

```
├── index.html        # Full application
├── manifest.json     # PWA manifest
├── sw.js             # Service worker
├── icon.svg          # Vector app icon
├── icon192.png       # 192×192 app icon
├── icon512.png       # 512×512 app icon
├── og-image.png      # Open Graph social share image
├── LICENSE           # Proprietary license
└── README.md
```

## License

© 2026 AlphaPlay LLC. All rights reserved. See [LICENSE](LICENSE).
