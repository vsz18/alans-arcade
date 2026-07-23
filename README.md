# 🕹️ Alan's Arcade

A birthday arcade built for Alan's 34th birthday. Four original browser games, all playable from a single arcade cabinet UI.

## Games

| Game | Genre | Description |
|------|-------|-------------|
| 🎮 **Birthday Bash** | Beat-em-up | Fight off waves of enemies to protect the birthday cake |
| 🍜 **Longevity Noodle** | Snake | Chinese birthday noodle snake — collect 🍑 🥟 🧧 🎂 to grow |
| 🥟 **Dumpling Dash** | Pac-Man | Eat all the dumplings, avoid the R&R crew |
| 🕯️ **Wishing Well** | Breakout | Knock out birthday candles to make a wish — level 3 spells "34" |

## Running locally

No build step. Just open `index.html` in a browser:

```bash
open index.html
```

Or serve it with any static file server:

```bash
npx serve .
# or
python3 -m http.server 8080
```

## Deploying to Render

The repo includes `render.yaml` for one-click Render deployment.

1. Push this repo to GitHub
2. Go to [render.com](https://render.com) → **New → Static Site**
3. Connect the `alans-arcade` repo — Render will auto-detect `render.yaml`
4. Click **Deploy**

Render will publish the site and give you a URL like `alans-arcade.onrender.com`.

## Tech

- Vanilla HTML/CSS/JS — no frameworks, no build tools
- HTML5 Canvas for all game rendering
- `localStorage` for high scores and session persistence
- Games are embedded via `<iframe>` + `postMessage` for cross-frame navigation
- Responsive: scales from desktop down to mobile
