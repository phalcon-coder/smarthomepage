# Adib's Browser Homepage

## Setup

1. Unzip / place this folder anywhere on your PC.
2. In Brave → Settings → **On startup → Open a specific page** → set it to the path of `index.html`
   - e.g. `file:///C:/Users/Adib/homepage/index.html`

---

## Adding Wallpapers

1. Drop any `.jpg` / `.png` / `.webp` image into the `backgrounds/` folder.
2. Open `backgrounds/manifest.json` and add the filename to the list:

```json
{
  "wallpapers": [
    "1.jpg",
    "2.jpg",
    "3.jpg",
    "your-new-image.jpg"
  ]
}
```

That's it — no touching `index.html`.

---

## Features

| Feature | Notes |
|---|---|
| Dynamic wallpaper | Rotates every 3 min, crossfades |
| Greeting + clock | Updates every 30s |
| Search / URL bar | Auto-detects URL vs search query → Brave Search |
| Leo button | Opens `brave://leo` (Brave's native AI sidebar) |
| Pinned sites | Saved in browser localStorage, persist forever |
| Brave Stats | Brave's ad-block stats are stored in browser internals and **cannot be read by any webpage** — this is a Brave security restriction, not a limitation of this page. The shield icon links to `brave://adblock`. |

---

## Brave Leo Note
The **✦ Leo** button opens `brave://leo`. This is the only way to interact with Leo from a local HTML file — Brave doesn't expose a JavaScript API for it.
