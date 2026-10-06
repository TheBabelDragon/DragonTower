# DragonTower

**Play → https://thebabeldragon.github.io/DragonTower/**

One more attempt. One more floor. Don't fall.

A tiny dragon climbs an endless seeded tower. Miss a platform and the climb is lost. Jump timing, platform variety, and altitude are the whole game.

## Controls

- **Desktop:** Arrow keys / A D · Space (or W / ↑) to jump — hold for higher jump
- **Mobile:** On-screen buttons

## Core Loop

Climb → risk → land or fall → restart from the bottom. Personal best is saved locally per browser.

## Platforms (introduced gradually)

| Type | Behavior |
|------|----------|
| Normal | Solid |
| Narrow | Smaller landing surface |
| Moving | Horizontal motion (deterministic) |
| Crumbling | Breaks shortly after landing |
| Bouncy | Higher launch |
| Disappearing | Cycles solid → warning → gone (readable) |

Early meters stay mostly normal so the player can learn movement and jump hold.

## Altitude themes

Castle → Old Tower → Machine → Above the Clouds → Sky City → The Impossible

## Rare event

**Tower Collapse** — platforms far below the player begin failing. Climb to stay ahead. Never destroys the platform you stand on or the next mandatory lands.

## Technical

- Single-file HTML5 Canvas + Web Audio (no external assets)
- Seeded procedural generation with reachability checks
- Local save (`dragontower.v2`, migrates v1)
- Deployed via GitHub Actions → Pages (`site/` folder)

## Local

Open `site/index.html` or serve `site/` with any static server.

Tuning lives in the `CFG` object at the top of the script.
