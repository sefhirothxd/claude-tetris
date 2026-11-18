# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Vanilla JS Tetris (HTML5 Canvas). No dependencies, no package.json, no build, no tests, no linter. Files: `index.html`, `style.css`, `game.js`.

## Running

Open `index.html` directly, or serve statically (`python -m http.server 8000`).

## Gotchas

- Changing `COLS`, `ROWS` or `BLOCK` in `game.js` requires updating `width`/`height` of `<canvas id="board">` in `index.html` (`COLS*BLOCK` x `ROWS*BLOCK`, currently 300x600).
- `game.js` runs in `'use strict'` and looks up DOM elements by id at load; keep ids in `index.html` in sync with the `getElementById` calls.
- README and UI text are in Spanish; keep README edits in Spanish.
