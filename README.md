# Orbit Raiders

> **Status:** Playable demo — one self-contained HTML file, no build step, no dependencies, no network calls.
> **▶ Play it now:** https://policani.net/orbit-raiders.html
> **Evaluate in 30 seconds:** open the live demo (or download this repo and open `index.html`), press **Space**, and read the on-screen controls.

A weekend side project, directed end to end with AI tools.

A single-file, 80s-arcade **radial tube shooter** that fuses two classics:

- **Gyruss** — your fighter orbits a circular ring around a central vortex,
  always facing inward, firing toward the middle while enemies spiral out at you.
- **Galaga** — a pink **Captor** boss can snare your ship with a tractor beam.
  Lose it and you lose a life — but blast the Captor while it holds your ship and
  you reclaim it as a **dual fighter** with double guns.

Each wave is a stop on a tour of the solar system — Mercury, Venus, Earth, the
Moon, Mars, the asteroid belt, Jupiter, Saturn, a comet — rendered as 8-bit
planets at the center that you fly toward, with a warp between stops where you
streak past other bodies.

Enemies come in several 8-bit flavors — grunts, shooters, fast weavers, armored
tanks, the capture boss, plus a **Centipede-style segmented worm** that winds
through the field and splits when you shoot its middle. **Slow-drifting asteroids**
cross the arena as obstacles to dodge or blast.

Built as a self-contained `index.html`: no build step, no dependencies, no network
calls. Ships and enemies are 8-bit pixel sprites; planets are chunky pixel art.
Music and sound are synthesized live with the Web Audio API — a driving **techno**
loop (four-on-the-floor kick, claps, offbeat hats, rolling acid bass, filtered arp)
plus laser, explosion, capture, rescue and warp effects. Nothing is loaded from
disk or the web, so it is fully royalty-free and portable. Press **F** (or the
button) for fullscreen.

## Play

Open `index.html` in any modern browser. Press **Space** (or tap) to start.

| Action | Keys |
|--------|------|
| Rotate around the ring | ◀ ▶ or A / D |
| Fire inward | Space |
| Fullscreen | F (or the button) |
| Pause | P |
| Mute / unmute | M |
| Touch | left/right half = rotate, top third = fire |

## Loop

Clear each wave of spiraling raiders. From wave 2 on, a Captor appears:
align with it, dodge the beam, and decide whether to risk the capture for a
shot at the dual-ship reward. Difficulty (enemy count, dive frequency, bullet
speed) scales each wave. Score: grunt 100, shooter 150, Captor 500, rescue 1000.

## Module boundary

- **Starts when** the page loads.
- **Produces** a playable arcade session and a high score held for the session.
- **Hands off to** nothing — it is a standalone toy/demo.
- **Does not** persist scores, call any network or storage API, or depend on any
  sibling module.

## Notes

This is a portfolio sample / playable demo, not a deployed product. All audio is
generated at runtime, so there are no external music or sound-effect assets to
license.
