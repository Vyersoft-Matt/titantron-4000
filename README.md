# Titantron.xyz

A wrestling entrance titantron simulator. Load any video, pick a screen layout, fire pyro.

🔗 [titantron.xyz](https://titantron.xyz) &nbsp;|&nbsp; 💬 [Discord](https://discord.gg/rURA6bTrWm)

---

## Current Version
**v0.3.6**

---

## What It Does

Drag any video file (entrance video, music video, whatever) into the arena and it plays back on a simulated WWE-style titantron setup. Switch between screen layouts, fire pyro, toggle arena lighting and fog, pick an accent color, and go fullscreen for the full effect.

No install. No account. One HTML file.

---

## Layouts

| Screens | Layouts |
|---------|---------|
| 1 | Classic |
| 3 | Cinematic, Suplex City |
| 5 | PPV, Vertical, Diamond, Cascade |
| 9 | Roman, 3x3, 3x3 Stagger |
| 13 | Videodrome |

---

## Controls

| Key | Action |
|-----|--------|
| Space | Play / Pause |
| P | Pyro Stage |
| R | Pyro Ramp |
| F | Fullscreen |

Click any screen to solo it fullstage. Click again to exit.

---

## Versioning — Hard Rule

Every update increments the version by `0.0.1`. No exceptions — bug fixes, features, copy changes, all of it.

When making any update:
1. Increment the version in `README.md` (Current Version above)
2. Increment the version in `index.html` header subtitle and tooltip
3. Both must match. Always.

---

## Changelog

| Version | Change |
|---------|--------|
| v0.0.1 | Initial release |
| v0.0.2 | Bug #1: DOM only rebuilds on preset change; play/pause no longer nukes video elements |
| v0.0.3 | Bug #2: WeakSet guard on createMediaElementSource — prevents double-sourcing |
| v0.0.4 | Bug #3: Delay uses readyState check before canplay listener |
| v0.0.5 | Bug #4: Pyro spam fix — timeout IDs stored and cleared before re-fire |
| v0.0.6 | Feature: Keyboard shortcuts — Space, P, R |
| v0.0.7 | UI: Controls split into three bars |
| v0.0.8 | UI: Info bar moved under preset buttons; version number added |
| v0.1.8 | UI: Keyboard hints next to Play; ? tooltip on version |
| v0.1.9 | UI: Visualizer button shows On/Off |
| v0.2.0 | Feature: Fullscreen button; F key shortcut |
| v0.2.1 | Bug #7: Drift correction loop — screens resync to main every 2s |
| v0.2.2 | Feature #8/#9: Solo mode; fade transition between presets |
| v0.2.3 | Feature: 5 new layouts — Cinematic, Diamond, Throwback, Cascade, Suplex City |
| v0.2.4 | Layout: Removed Throwback; Cinematic repositioned; trusses aligned |
| v0.2.5 | Fix: Diamond + Cascade use prime-offset delays to prevent loop sync |
| v0.2.6 | Fix: Suplex City + Diamond delays pushed to large primes |
| v0.2.7 | UI: Presets reordered by screen count; dividers between groups |
| v0.2.8 | Layout: Suplex City left screens on truss; center truss for Diamond + Cascade |
| v0.2.9 | Bug fix: drift correction used absolute delays — was zeroing out all offsets |
| v0.3.0 | v0.3: Arena color picker; stronger spotlights + wash lights + floor bounce; animated 3-layer fog |
| v0.3.1 | Bug fix: fog height was 0; spot wash z-indexes fixed; duplicate soloHint removed |
| v0.3.2 | Bug fix: screensContainer given position+z-index for reliable screen stacking |
| v0.3.3 | Bug fix: viz canvas z-index raised above screensContainer |
| v0.3.4 | Bug fix: visualizer .active class was missing; AudioContext resume added |
| v0.3.5 | Viz canvas moved behind screens (z:5) |
| v0.3.6 | Renamed to Titantron.xyz; Discord link added to header |
