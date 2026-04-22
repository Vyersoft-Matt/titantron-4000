# titantron-4000

A wrestling entrance titantron simulator. Load a video, pick a screen layout, fire pyro.

## Current Version
**v0.2.4**

---

## Versioning — Hard Rule

**Every update to this project increments the version by `0.0.1`.**

This applies to all changes: bug fixes, new features, UI tweaks, refactors, copy changes — anything. No exceptions.

When making any update:
1. Increment the version number in `README.md` (the "Current Version" line above)
2. Increment the version number in the `index.html` header subtitle: `by SOL · vX.X.X`
3. Both must match. Always.

---

## Changelog

| Version | Change |
|---------|--------|
| v0.0.1 | Initial release |
| v0.0.2 | Bug #1: Refactored renderScreens — DOM only rebuilds on preset change, play/pause no longer nukes video elements |
| v0.0.3 | Bug #2: WeakSet guard on createMediaElementSource — prevents double-sourcing and silent audio disconnect |
| v0.0.4 | Bug #3: Delay now checks readyState before attaching canplay listener — works on already-buffered video |
| v0.0.5 | Bug #4: Pyro spam fix — timeout IDs stored and cleared before re-fire |
| v0.0.6 | Feature: Keyboard shortcuts — Space (play/pause), P (pyro stage), R (pyro ramp) |
| v0.0.7 | UI: Controls split into three separate bars — Play, Pyro, Toggles |
| v0.0.8 | UI: Info bar moved under preset buttons; version number added to header and README |
| v0.1.8 | UI: Keyboard hints moved next to Play button; ? tooltip on version shows latest update |
| v0.1.9 | UI: Visualizer button now shows On/Off consistent with other toggles |
| v0.2.0 | Feature: Fullscreen button on stage; fades out when idle; F key shortcut |
| v0.2.1 | Bug #7: Drift correction loop — non-main screens resync to main every 2s, wrap-aware |
| v0.2.2 | Feature #8/#9: Click any screen to solo full-stage; fade transition between presets |
| v0.2.3 | Feature: 5 new layouts — Cinematic, Diamond, Throwback, Cascade, Suplex City |
| v0.2.4 | Layout: Removed Throwback (duplicate of Classic); Cinematic screens repositioned to stay in bounds; Diamond + Cascade aligned to trusses |
