# AGENTS.md

## Project Goal
Customize the forked project `doggy8088/trigonometric-functions` by adding an interactive control panel that lets users adjust angle and animation speed, while showing live trigonometric values (`sin`, `cos`, `tan`) in a clear teaching-focused UI.

## Tech Stack
- HTML5 + CSS3 + vanilla JavaScript (ES6+)
- Three.js (existing dependency from source project)
- No backend; static-site deployment on GitHub Pages

## Architecture Overview
- `index.html`: UI structure, panel layout, and script wiring
- Existing rendering/animation logic: extended with panel-driven state updates
- Control state: single source of truth for angle, speed, and play/pause
- Numeric display layer: derives and renders `sin/cos/tan` from current angle

## References
- Source fork: https://github.com/doggy8088/trigonometric-functions
- Three.js docs: https://threejs.org/docs/

## Global Acceptance Criteria
1. A visible control panel exists and allows setting angle directly (slider and/or numeric input).
2. Users can adjust animation speed with clear controls, and the animation responds immediately.
3. Live values for `sin(θ)`, `cos(θ)`, and `tan(θ)` are displayed and update correctly with angle changes.
4. Manual angle changes and autoplay remain consistent (no desync between visualization and displayed values).
5. The app runs as a static site and is deployable/accessible via GitHub Pages.
