# App template

The starting point for Michael's small apps: static, installable, offline, multilingual (EN / DE / 中文), no outside requests. See [FORMAT.md](FORMAT.md) for the checklist every app follows.

## Start a new app

1. On GitHub: **Use this template** → new repository.
2. Replace "App name" and the one-sentence description in `index.html` (all three languages), `manifest.webmanifest` and the `<title>`.
3. Draw your icon in `icons/icon.svg`, then `python3 icons/make-icons.py` (needs `pip install cairosvg pillow`).
4. Build the app inside `<main id="app">`. Put texts in the `T` table with a `data-t` key so they switch language.
5. Add every file the app needs to `FILES` in `sw.js`.
6. Settings → Pages → deploy from `main`, root. The app appears at `michaelwartmann.github.io/<repo>/`.
7. Check the list in FORMAT.md, then add a card to the hub.

## Files

| File | What it is |
|---|---|
| `index.html` | The shell: name, language switch, description, the app, install help, footer |
| `manifest.webmanifest` | Name, colours and icons for the home screen |
| `sw.js` | Offline cache |
| `icons/` | `icon.svg` and the PNGs made from it |
| `FORMAT.md` | The checklist |

MIT licence.
