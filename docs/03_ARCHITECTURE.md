# Architecture

## Principles

- Cross-platform from day one: iOS and Android.
- Prefer one shared codebase where practical.
- Keep gameplay systems modular.
- Keep third-party services behind clear interfaces where practical.
- Avoid unnecessary SDKs and external dependencies.
- Make analytics, audio and monetization replaceable rather than deeply coupled to gameplay.
- Keep development costs at or near €0 until there is a clear reason to spend money.

## Selected technology

### Game engine: Godot 4.x

Godot is selected as the initial game engine for SWING.

Reasons:

- Free and open source under the MIT license.
- Commercial games are permitted without engine royalties.
- Native export support for Android and iOS.
- Strong 2D tooling and built-in physics suitable for the core swinging mechanic.
- GDScript is tightly integrated with the engine and well suited to gameplay iteration.
- Keeps the project lightweight and avoids paying for engine tooling while the game is being validated.
- Extensible through platform plugins when native mobile services are required.

The project should initially use GDScript rather than C# unless a concrete technical requirement justifies a change.

## Planned system areas

```text
SWING
├── Core
│   ├── Game State
│   ├── Run Management
│   └── Save Data
├── Gameplay
│   ├── Player / Movement
│   ├── Hook System
│   ├── Swing Physics
│   ├── World / Level Generation
│   ├── Obstacles
│   └── Scoring / Progression
├── Presentation
│   ├── Camera
│   ├── Visuals
│   ├── Audio
│   └── UI
├── Services
│   ├── Analytics
│   ├── Crash Reporting
│   ├── Advertising
│   └── In-App Purchases
└── Platform
    ├── iOS
    └── Android
```

## SDK / third-party integration principle

External SDKs and plugins may be used for analytics, advertising, crash reporting or platform functionality, but they should not be embedded into the core gameplay logic.

Before adding an SDK/plugin we evaluate:

1. Is it actually necessary?
2. Does it support both iOS and Android where required?
3. Is there a free tier or open-source option?
4. What data does it collect?
5. What permissions/tracking does it require?
6. What are the licensing and commercial implications?
7. How difficult would it be to replace later?

Likely examples include a mobile ads SDK, analytics/crash reporting integration and store billing APIs. These will be added only when their corresponding feature is needed.

## Platform considerations

Android export can be handled directly from Godot. iOS export requires a macOS machine with Xcode for the native build/deployment step. This is a platform requirement rather than a reason to use a different engine.

## Web / Vercel

Vercel is not part of the game runtime. It may later host the project website, privacy policy, terms, support pages and store links.

## Current status

Technology decision complete. Next technical step: create the Godot project and establish the minimum prototype structure before implementing gameplay.
