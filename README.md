# SWING

> Working title — the final game name has not been decided.

SWING is a mobile game concept built around momentum, timing and movement. The core idea is simple: attach to hooks, swing, release at the right moment, and keep progressing through an increasingly challenging world.

## Platforms

- iOS — planned from day one
- Android — planned from day one
- Current development/testing: Windows + Godot 4.x

## Current status

**Phase:** Playable prototype / core gameplay validated  
**Current build:** Swing physics prototype with horizontal camera movement, selectable hooks, hook skipping, restart/game-over state and fixed UI instructions.

The core swing currently feels smooth enough to use as the physics baseline for further development. The game is moving toward an **endless-run structure** rather than a fixed finish line.

### Current design direction

- Endless run rather than a fixed level finish.
- Primary score is distance travelled in meters.
- Falling ends the run.
- Best distance/high score will be retained later.
- Hooks will eventually be generated continuously as the player progresses.
- Current player/hook/background visuals are temporary prototype art.
- Final visual direction is intended to use a stylized character, distinctive hook/cable design, layered environment, particles and strong motion effects.

## Development philosophy

1. Validate the core gameplay quickly.
2. Keep the first playable version small.
3. Use AI-assisted development wherever it provides leverage.
4. Keep iOS and Android in scope from the beginning.
5. Build analytics into the architecture at the appropriate stage.
6. Treat audio, monetization and legal/compliance as first-class project concerns.
7. Keep this repository as the single source of truth for project decisions and documentation.
8. Freeze working physics when the game feel is good; make changes only when a concrete gameplay problem is identified.

## Documentation

- [Game Design](docs/01_GAME_DESIGN.md)
- [Roadmap](docs/02_ROADMAP.md)
- [Architecture](docs/03_ARCHITECTURE.md)
- [Design System](docs/04_DESIGN_SYSTEM.md)
- [Development Log](docs/05_DEVELOPMENT_LOG.md)
- [Legal & Compliance](docs/06_LEGAL_AND_COMPLIANCE.md)
- [Monetization](docs/07_MONETIZATION.md)
- [Analytics](docs/08_ANALYTICS.md)
- [Audio](docs/09_AUDIO.md)
- [Release Checklist](docs/10_RELEASE_CHECKLIST.md)
- [Future Ideas](docs/11_FUTURE_IDEAS.md)
- [Decision Log](docs/12_DECISIONS.md)

## Repository rule

After every development session, the relevant documentation should be updated so that it reflects the actual state of the project, not an outdated plan.
