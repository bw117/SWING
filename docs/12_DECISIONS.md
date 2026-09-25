# Decision Log

## D001 — SWING is a working title

**Date:** 2026-09-25  
**Decision:** Use SWING as the project working name.  
**Status:** Temporary  
**Reason:** A final name has not been selected.

## D002 — Target iOS and Android from day one

**Date:** 2026-09-25  
**Decision:** Both mobile platforms are part of the initial product scope.  
**Reason:** Avoid designing the project around a single platform and retrofitting the second later.

## D003 — Validate gameplay before scaling scope

**Date:** 2026-09-25  
**Decision:** Build a small proof of concept before substantial investment in content, monetization or polish.  
**Reason:** Reduce development risk and validate the core game loop early.

## D004 — GitHub is the documentation source of truth

**Date:** 2026-09-25  
**Decision:** Project decisions, roadmap, development history, legal/compliance notes and future plans live in the repository.  
**Reason:** Keep implementation and documentation synchronized.

## D005 — Audio is a first-class system

**Date:** 2026-09-25  
**Decision:** Music and sound effects are part of the product architecture.  
**Reason:** Audio contributes directly to game feel and player feedback.

## D006 — Use Godot 4.x as the initial game engine

**Date:** 2026-09-25  
**Decision:** Build SWING initially with Godot 4.x and GDScript.
**Status:** Active
**Reason:** Godot is free/open source under MIT, supports commercial games, has native iOS/Android export, strong 2D tooling and physics, and fits the goal of building the first version with minimal tooling cost. The engine also supports platform plugins for services such as ads and in-app purchases.
**Trade-off:** Some mobile SDK integrations require third-party plugins and native platform knowledge. We will keep those integrations isolated so they can be replaced if necessary.

## D007 — Keep external SDKs out of core gameplay

**Date:** 2026-09-25  
**Decision:** Analytics, ads, crash reporting and store billing must sit behind separate service/integration layers rather than being directly embedded throughout gameplay code.
**Reason:** Reduce vendor lock-in, simplify testing and keep legal/privacy changes isolated.
