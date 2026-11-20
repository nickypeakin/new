# Torque Cup

An original, browser-based 1v1 car football game: you against a bot, a giant ball, and a glass arena whose floor curves up into the walls and ceiling. Drive the walls, fly with boost, and score.

## Play

Open `index.html` in a modern browser. It's a single file. The 3D engine ([three.js](https://threejs.org/)) loads from a CDN, so you need an internet connection.

To host it, enable **GitHub Pages** for this repo (Settings → Pages → deploy from branch, root folder).

## What's in it

- **1v1 vs a bot** at three skill levels (Rookie, Pro, All-Star), with 3, 5 or 7 minute matches, overtime, and an end-of-match scoreboard
- **Full-size arena**: an 8192 × 10240 pitch, a 2044-high ceiling, 45° corner cuts, and goals 1786 wide × 643 tall × 880 deep. The ball has a radius of 92.75 and the car hitbox is about 118 × 84 × 36. Everything uses the same unit scale.
- **Curved walls you can drive on**: every edge of the arena is rounded, so you can drive from the floor up the walls and across the ceiling. Jump to push off a wall. The arena is a signed distance field, and both the physics and the rendered mesh come from it.
- **Car feel**:
  - Throttle tops out at 1410 and boost at 2300. Supersonic is at 2200, and that's where demolitions happen.
  - Steering tightens at low speed.
  - Powerslide, jump plus hold-to-go-higher, and a double jump.
  - Flips that push the car in the stick direction.
  - Air pitch, yaw and roll with damping.
  - Boost works in the air, so you can do aerials.
- **Ball hits** combine a real impulse (a heavier car hitting a lighter ball, including the spin of a flip) with an extra speed-scaled kick, so shots feel punchy.
- **Camera**: 110° field of view, 270 behind and 110 above the car, and a -3° tilt. Switch between ball cam and car cam.
- Boost pads (6 big, 22 small), goal explosions, and a clock that waits for the ball to land at 0:00
- Keyboard, mouse, gamepad and touch controls. Sound is synthesized, so there are no audio files.

## Controls

| Action | Keyboard / mouse | Gamepad |
| --- | --- | --- |
| Throttle / reverse (pitch in the air) | `W` `S` or `↑` `↓` | RT / LT (left stick to pitch) |
| Steer (yaw in the air) | `A` `D` or `←` `→` | Left stick |
| Jump, double jump, flip (jump + direction) | `Space` / right click | A |
| Boost | `Shift` / left click | B |
| Powerslide | `X` | X |
| Air roll | `Q` `E` | LB / RB |
| Ball cam / car cam | `C` | Y |
| Pause | `Esc` / `P` | Start |
| Mute | `M` | |

If you land on your roof, press jump to flip back onto your wheels.

On phones and tablets, a virtual joystick appears on the left, with Jump, Boost, Drift and Cam buttons on the right.
