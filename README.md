# Torque Cup

An original, boost-powered car football game that runs in the browser. Drive, jump, flip and fly to knock a giant ball into the other team's goal under a glass dome.

## Play

Open `index.html` in a modern browser. It's a single file. The 3D engine ([three.js](https://threejs.org/)) loads from a CDN, so you need an internet connection.

To host it, enable **GitHub Pages** for this repo (Settings → Pages → deploy from branch, root folder). The game is then served at `https://<user>.github.io/<repo>/`.

## Features

- **1v1, 2v2 or 3v3** against bots, with three bot skill levels (Rookie, Pro, All-Star) and 2, 3 or 5 minute matches
- Arcade car physics: throttle, reverse, drift, jump, double-jump, directional flips, air pitch, yaw and roll, and air boost for aerial hits
- Boost meter with 6 big pads (full refill) and 22 small pads
- Supersonic speed and demolitions: hit an opponent at top speed to blow them up (they respawn after 3 s)
- Goal explosions, overtime (next goal wins), and the clock waits for the ball to land at 0:00
- End-of-match stats: goals, shots, saves, touches, demos
- Ball cam and car cam, keyboard, mouse, gamepad and on-screen touch controls
- Synthesized sound, with no audio files

## Controls

| Action | Keyboard / mouse | Gamepad |
| --- | --- | --- |
| Throttle / reverse (pitch in the air) | `W` `S` or `↑` `↓` | RT / LT (left stick to pitch) |
| Steer (yaw in the air) | `A` `D` or `←` `→` | Left stick |
| Jump, double jump, flip (jump + direction) | `Space` / right click | A |
| Boost | `Shift` / left click | B |
| Drift | `X` | X |
| Air roll | `Q` `E` | LB / RB |
| Toggle ball cam | `C` | Y |
| Pause | `Esc` / `P` | Start |
| Mute | `M` | |

On phones and tablets, a virtual joystick appears on the left, with Jump, Boost, Drift and Cam buttons on the right.
