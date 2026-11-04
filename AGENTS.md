# AGENTS.md

## Project

Vanilla HTML5 Canvas + ES6 JavaScript asteroids clone. No framework, bundler, or dependencies; no build step.

- `index.html` — markup, inline CSS, `<canvas id="canvas">`, loads `game.js`
- `game.js` — all game logic in one file (Bullet, Asteroid, Ship, Particle; `requestAnimationFrame` loop)

## Commands

- No toolchain: no package.json, tests, lint, typecheck, build, or CI.
- Run: open `index.html` directly in browser, or `npx serve .` → http://localhost:3000.
- No automated checks — verify manually in the browser.

## Architecture notes

- Game loop: `requestAnimationFrame` with `dt` clamped to 0.05s; world wraps toroidally.
- Game states: `'playing' | 'dead' | 'gameover'`.

## Conventions

- Code identifiers in English; comments and user-facing strings in Spanish.
- Keep new code inside the existing `game.js` / `index.html`; no new modules or framework.
