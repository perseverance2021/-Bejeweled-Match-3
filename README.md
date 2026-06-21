# Bejeweled Match 3

A browser-based Bejeweled-style match-3 puzzle game. No build step, no dependencies — open `index.html` or host the folder on any static server.

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## Features

- **8×8 grid** with six gem types
- **Four game modes**
  - **Classic** — play until no valid swaps remain
  - **Timed** — score as much as you can in 60 seconds
  - **Zen** — endless play; the board reshuffles when stuck
  - **Challenge** — reach 1,000 points to win
- **14 color themes** with custom UI and gem palettes
- **Procedural sound effects** (Web Audio API)
- **Watch AI** — computer plays automatically
- **Mobile-friendly** — responsive layout with tap and swipe controls
- **Per-mode high scores** and saved theme/mode preferences (`localStorage`)

## How to play

**Desktop:** Click a gem, then click an adjacent gem to swap.

**Mobile:** Tap to select, tap an adjacent gem to swap, or swipe a gem toward a neighbor.

Matches of three or more identical gems (horizontal or vertical) clear, gems fall, and new ones drop in. Chain reactions increase your combo multiplier.

## Quick start

### Option 1 — Open locally

```bash
open index.html
```

Or double-click `index.html` in your file browser.

### Option 2 — Local server (recommended for mobile testing)

```bash
python3 -m http.server 8080
```

Then open [http://localhost:8080](http://localhost:8080).

### Option 3 — GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Set **Source** to deploy from the `main` branch (root folder).
4. Your game will be available at `https://<username>.github.io/<repo>/`.

## Project structure

```
.
├── index.html   # Complete game (HTML, CSS, JavaScript)
├── LICENSE      # MIT License
└── README.md    # This file
```

## Browser support

Works in modern browsers that support CSS Grid, ES6+, and the Web Audio API (Chrome, Firefox, Safari, Edge). Audio starts after the first user interaction due to browser autoplay policies.

## License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
