# Cities & Knights — City Improvement Tracker

A lightweight, mobile-friendly web app for tracking the three city improvement disciplines in **Catan: Cities & Knights** — **Science** (Paper), **Trade** (Cloth), and **Politics** (Coin).

Each player on a device gets their own saved session. Tap to move each discipline up and down its 5-level ladder, see the matching improvement name, its special ability, the commodity cost of the next level, and when you've unlocked a **Metropolis** (4 VP).

## Features

- 🧙 **Per-player sessions** — "log in" with your name; everyone's progress is saved locally on the device. Pass the phone around a table, or open it on your own.
- 📈 **Three ladders** — Science · Trade · Politics, each 0–5, with tap-to-set rungs and − / + buttons.
- 🏛️ **Metropolis tracking** — claim a Metropolis at level 4 (worth 4 VP); only one per discipline.
- 🪙 **Costs & abilities** — every level shows its real board name (School, Library, Aqueduct, Theater, University, etc.), commodity cost, and special ability.
- 📱 **Mobile-first & offline** — pure client-side, no backend, no build step. Works from `file://` or any static host.

## Run it

It's a single self-contained file. Just open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

To use it on your phone, host the folder (e.g. GitHub Pages, Vercel, or `python3 -m http.server` on your laptop and visit your laptop's IP) and add it to your home screen.

## Tech

Plain HTML / CSS / vanilla JS. State persists in `localStorage`. No dependencies.

> Improvement names and abilities follow the Catan: Cities & Knights board. Catan is a trademark of Catan GmbH; this is an unofficial fan-made tracker.
