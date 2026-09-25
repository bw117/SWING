# Game Design

## Working concept

SWING is a mobile, momentum-based endless-run game focused on timing, movement and mastery.

### Core loop

1. Start a run.
2. Identify a reachable hook.
3. Attach / swing.
4. Build and manage momentum.
5. Release at the right moment.
6. Reach another hook or navigate an obstacle.
7. Continue as far as possible.
8. Fall / fail.
9. Record the distance and try again.

## Primary score

The primary score is **distance travelled in meters**.

There is no fixed finish line in the intended game structure. A run continues as long as the player stays alive. Falling ends the run.

Future supporting metrics may include:

- Best distance
- Maximum speed
- Longest swing
- Perfect releases
- Combo / streak
- Near misses

These are secondary to distance and should only be added when they improve the game.

## Design goals

- Easy to understand.
- Difficult to master.
- Short, replayable runs.
- Strong sense of momentum.
- Clear and satisfying feedback.
- Skill should be more important than grinding.
- Good runs should visibly and mechanically benefit from maintaining momentum.

## Current gameplay baseline

The current pendulum-based swing physics are considered the baseline because the latest playable version feels substantially smoother than earlier iterations. Physics should not be repeatedly rewritten without a concrete gameplay problem.

The current prototype supports:

- Horizontal camera movement.
- Deliberate hook selection.
- Skipping hooks.
- Swinging around a selected hook.
- Momentum carried into the next hook.
- Release into free flight.
- Restart and game-over state.

## Visual direction

The current player, hooks and environment are temporary debug/prototype visuals.

The intended final direction is substantially more stylized:

- A recognizable character rather than a simple ball.
- A distinctive, visually interesting hook/cable.
- A layered environment with depth and atmosphere.
- Strong movement feedback through trails, particles and animation.
- Environmental obstacles that feel integrated into the world.
- A cohesive visual identity rather than relying primarily on color changes.

## Future possibilities

Potential future systems include procedural generation, increasingly difficult obstacles, world-specific mechanics, progression, cosmetics, premium content, leaderboards, daily challenges and other high-score systems. These remain subject to validation.
