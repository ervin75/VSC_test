# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A browser-based Gomoku (Tic Tac Toe variant) game — single HTML file with inline CSS and JavaScript. Two players take turns on a 9×9 grid; first to get 5 in a row wins.

## Architecture

Everything lives in `tictactoe.html`:
- **CSS**: Grid layout, dark theme, cell states (`.x`, `.o`, `.win`), animations
- **JS game engine**: Board state as a flat array (81 cells), turn-based play, directional win detection (horizontal, vertical, both diagonals), score tracking across games

Key constants: `SIZE=9`, `WIN_LEN=5`, `TOTAL=81`. Win checking scans from the last-placed piece outward in 4 directions.

## Development

No build tools or dependencies. Open `tictactoe.html` directly in a browser to run. Changes are tested by refreshing the page.
