# DragonTower

**Play → https://thebabeldragon.github.io/DragonTower/**

One more attempt. One more floor. Don't fall.

A tiny dragon climbs an endless, seeded tower. Miss a platform and the whole climb is lost. Jump timing, platform variety, and altitude progression are the core of the game.

## Controls

- **Desktop:** Arrow keys / A D to move · Space (or W / ↑) to jump — hold for higher jump
- **Mobile:** On-screen buttons (left / right / JUMP)

## Core Loop

- Climb as high as you can
- Fall = lose the current climb and restart from the bottom
- Personal best is saved locally (per browser / device)

## Features (Production Pass)

- **Expressive dragon** — idle, run, jump stretch, landing squash, fall panic, celebration
- **Platform types** (introduced progressively):
  - Normal
  - Narrow
  - Moving
  - Crumbling
  - Bouncy
  - Disappearing
- **Altitude themes**
  - The Castle → Old Tower → Machine → Above the Clouds → Sky City → The Impossible
- **Special events** (rare)
  - Tower Collapse
  - Passing Train
- **Milestones** with feedback (50m, 100m, 250m…)
- **Improved fall** presentation and fast restart
- Deterministic tower generation with reachability checks
- Local save (backward-compatible with v1)

## Run Locally

Just open `site/index.html` in a browser, or serve the `site/` folder with any static server.

## Deploy

GitHub Actions deploys the `site/` folder to GitHub Pages on every push to `main`.

## Tuning

All major numbers live in the `CFG` object at the top of the script in `site/index.html`.
