# Garden

A Japanese garden seen from a tatami room, rendered and simulated live in the
browser. The paper doors are shut when you arrive; touch them and they slide
open onto the garden in the late afternoon light, and the day begins to go by.

**Open it:** https://bwang55.github.io/Garden/

Everything is one self-contained HTML file: no install, no server, no assets to
load.

## Things to try

- **Touch the paper doors** to slide them open (this also starts the sound).
  Afterwards you can slide each of the four doors by hand, or shut them all
  from the menu.
- **Drag across the gravel** to rake it.
- **Touch the pond** and drag through it to send ripples across the water.
- **Drag through the air** to stir up a gust: the branches bend, the leaves
  flip, the water ruffles.
- **Open the menu** (top right) to change the time of day, rain, snow and
  wind, the season, the light and the mist, and the sound.

## What is in it

- **Light.** The still garden is baked once into a G-buffer for the fixed view
  and relit every frame: sun or moon with soft shadows, the sky, stone
  lanterns and a paper floor lamp whose flames flicker. Light enters the room
  only through the opening and through the paper of the doors, so the floor
  brightens toward the garden and the shoji glow. Aerial haze, volumetric mist
  and light shafts give the depth.
- **Plants.** Two maples, a pine and clipped azaleas whose branches are
  simulated and whose leaves are each posed in the wind; 160,000 blades of
  grass bending in waves; leaves that fall, land and float on the pond.
- **Water.** A pond with a ripple simulation, a stream from a small waterfall,
  and a working shishi-odoshi: the bamboo fills, tips, pours and knocks on its
  stone.
- **Weather.** Rain soaks the garden and lets it dry again in patches. Snow
  settles faster on the moss than on the gravel and thaws the other way round.
  One wind field moves everything: trees, grass, mist, rain, snow, chimes.
- **Small things.** Glass wind chimes that ring when their clappers strike, a
  teru-teru-bōzu, dragonflies on fine days, fireflies on early summer nights,
  a seven-tiered stone pagoda, and the old town and hills beyond the wall.
- **Sound,** synthesized as it plays: water, wind in the crowns, rain,
  crickets, a distant temple bell, the chimes, the doors in their grooves.

## Running it

Open `index.html` in a recent desktop browser with WebGL 2 (Chrome, Edge,
Safari 17 or later, Firefox). A dedicated GPU or Apple silicon is recommended;
**Performance mode** in the menu lowers the resolution for a steadier frame
rate.

## Deploying

This repository holds the built page only. To publish it with GitHub Pages:
**Settings → Pages → Build and deployment → Deploy from a branch →
`main` / `(root)`**. The page is then served at
`https://<user>.github.io/Garden/`.

## Built with

[three.js](https://threejs.org/) and [lil-gui](https://lil-gui.georgealways.com/),
bundled with Vite into a single file.
