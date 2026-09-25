# Development Log

This file records meaningful development sessions and decisions. It should be updated after each SWING development session.

## 2026-09-25 — Project initialization

- GitHub repository created.
- SWING confirmed as the temporary working name; final name remains undecided.
- Goal established: build a small proof of concept first and validate the core gameplay before substantial investment.
- iOS and Android are both target platforms from day one.
- GitHub is the single source of truth for project documentation.
- Analytics should be incorporated at the appropriate architectural stage.
- Audio (music and sound effects) is part of the product scope.
- Legal/compliance and monetization will be documented throughout development rather than handled only immediately before launch.
- Initial development effort targets remain approximately 5–10 hours for the proof of concept, 15–30 hours for a playable prototype and 30–50 hours for an MVP, subject to actual complexity.

## 2026-09-25 — First playable swing proof of concept

### What we built

- Created the Godot 4.7.2 project locally on Windows.
- Created the initial `Main` Node2D scene at `scenes/main.tscn`.
- Created `scripts/main.gd`.
- Implemented a first playable swing prototype with a player, fixed hooks, gravity, rope attachment, swing motion, release and reset.
- Confirmed the project runs successfully in the Godot debug window.

### Findings

- The first implementation automatically selected the nearest hook, which currently forces a mostly linear hook sequence.
- The prototype currently renders a single fixed screen; the camera/world does not yet follow the player horizontally.
- The swing currently behaves as a simple circular pendulum and needs substantially more tuning before it represents the intended game feel.
- The current hooks are temporary debug geometry, not final visual assets.

### Decision for next iteration

- Move from a fixed-screen nearest-hook demo to a horizontal gameplay space.
- Allow the player to deliberately select a visible hook so hooks can be skipped.
- Add camera following and a longer hook path.
- Keep the gameplay/input design compatible with future touch controls on iOS and Android.

### Next steps

- Build the v0.2 horizontal world/camera prototype.
- Generate or define a substantially longer hook path.
- Implement deliberate hook selection rather than nearest-hook auto-selection.
- Improve release/momentum behavior after the world/camera loop is working.

### Documentation updated

- Roadmap
- Development Log
- Decision Log as needed

## Session template

### Date

### What we built

### Decisions

### Problems / bugs

### Tests / findings

### Next steps

### Documentation updated
