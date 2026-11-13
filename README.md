# AQUASENSE Dashboard

Open `index.html` in any modern browser (or run `python -m http.server` in this folder). No installs or build tools.

## Files
- `index.html` – structure, icon sprite
- `styles.css` – design system and responsive layout (mobile bottom nav, tablet, desktop sidebar)
- `app.js` – species selection, live simulated readings, responsive canvas charts, records CSV download, cleaning checklist

## Your image assets
Place these in `assets/` (missing images fall back to a simple fish icon):
`bangus.png`, `crab.png` (Alimango), `tilapia.png`, `shrimp.png` (Hipon), `hito.png`

## Connecting real sensors
Replace the `tick()` function in `app.js` with a fetch from your device/API and write the values into `state.values`.
Species safe ranges are in the `SPECIES` object at the top of `app.js`.
