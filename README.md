# Football Fútbol ⚽🏈

A silly little arcade soccer game — but the ball is an American football, so it **wobbles, curves, and never rolls quite straight**. Run your player into the ball to shove it toward the goal. Play the AI, a friend, or a chaotic 2v2.

**Play it:** [ff.notsteve.com](https://ff.notsteve.com)

## How to play

Run into the ball to push/kick it. How you hit it matters:

- **Hit it broadside** (across the ball's short side) → a clean, straight shot.
- **Catch it end-on** (the pointy way) → it wobbles and curves unpredictably.
- **Boost** for a burst of speed — great for steals, saves, and lofting the ball into the air.
- **Sprint** by holding a direction; you build speed the longer you run in a straight line.
- A hard enough kick sends the ball **airborne**, flying over players (but not the posts).

Score in the far goal. First to a point target, or most goals when the clock runs out (ties go to sudden death).

## Controls

| | Move | Boost |
|---|---|---|
| **Home** | WASD | Left Shift |
| **Away** (2-player) | Arrow keys | Right Shift |
| **Gamepad** | Left stick | A / bumper |

- **Esc / P** or **gamepad Start** — pause
- **C** — cycle team colors
- **M** — mute

Up to **4 controllers** for 2v2. Plug them in and they're detected automatically.

## Setup

On the title screen, pick your match:

- **Format** — Timed (set the minutes) or Points (first to N).
- **Players** — 1v1 or 2v2, and how many are human (the rest are AI).

## Tech

One self-contained `index.html` — no frameworks, no build step, no dependencies. Vanilla JavaScript + the Canvas 2D API, with the Web Audio API for sound and the Gamepad API for controllers. All the physics (the signature wobble, fake-3D ball height, collisions) and the AI are hand-rolled. Runs on a fixed 60 Hz timestep so it plays the same on any display refresh rate.

Built with [Claude Code](https://claude.com/claude-code).
