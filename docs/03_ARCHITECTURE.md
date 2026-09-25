# Architecture

## Principles

- Cross-platform from day one: iOS and Android.
- Prefer one shared codebase where practical.
- Keep gameplay systems modular.
- Keep third-party services behind clear interfaces where practical.
- Avoid unnecessary SDKs and external dependencies.
- Make analytics, audio and monetization replaceable rather than deeply coupled to gameplay.

## Planned system areas

```text
Game
├── Player / Movement
├── Hook System
├── Swing Physics
├── World / Level Generation
├── Obstacles
├── Scoring / Progression
├── Camera
├── Audio
├── UI
├── Analytics
└── Monetization
```

## Technology decision

Not selected yet. The technology choice will be made before substantial gameplay implementation, with iOS/Android support, 2D/physics performance, development speed, AI-assisted development and store deployment as key considerations.

## Third-party SDK principle

External SDKs may be used for services such as analytics, advertising or platform functionality, but each SDK must be evaluated for necessity, privacy implications, licensing, platform support and legal/compliance impact before inclusion.
