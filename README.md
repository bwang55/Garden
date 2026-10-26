# Garden

Three quiet places, rendered and simulated live in the browser. Each one is a
single self-contained HTML file: no install, no server, no assets to load.

| | Page | Open it |
|---|---|---|
| A Japanese garden seen from a tatami room | [`index.html`](index.html) | https://bwang55.github.io/Garden/ |
| Meditation in a bamboo grove at dawn | [`bamboo/index.html`](bamboo/index.html) | https://bwang55.github.io/Garden/bamboo/ |
| One tree in the wind, where it all began | [`tree/index.html`](tree/index.html) | https://bwang55.github.io/Garden/tree/ |

## The garden

The paper doors are shut when you arrive; touch them and they slide open onto
the garden in the late afternoon light, and the day begins to go by.

**Things to try**

- **Touch the paper doors** to slide them open (this also starts the sound).
  Afterwards you can slide each of the four doors by hand, or shut them all
  from the menu.
- **Drag across the gravel** to rake it.
- **Touch the pond** and drag through it to send ripples across the water.
- **Drag through the air** to stir up a gust: the branches bend, the leaves
  flip, the water ruffles.
- **Open the menu** (top right) to change the time of day, rain, snow and
  wind, the season, the light and the mist, and the sound.

**What is in it**

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

## The bamboo grove

You arrive with your eyes closed, breathing. Touch to open them: a blurred
slit that widens into focus on a small clearing in a grove of tall bamboo at
dawn, a straw cushion, a stick of incense smoking in its burner, an iron
kettle simmering beside the tea things.

**Things to try**

- **Drag through the air** to send a gust through the grove.
- **Touch a culm** to set it swaying.
- **Drag gently past the incense** to stir its smoke.
- **Open the menu** for the time of day, the wind, the grove itself (how
  dense, how thick and tall the culms, young culms, dwarf bamboo, or grow
  another one), the light and the mist, and the sound.

**What is in it**

- Some two thousand culms, each a stiff tapering pole swaying in its first
  bending mode, driven by the shared wind, so gusts sweep through the grove
  in slow waves; culms at the edge of the clearing now and then knock together.
- Incense smoke that rises as a smooth thread, wavers, curls and spreads into
  a veil, drifting with the air; steam from the kettle.
- Low morning sun through the canopy, light shafts in the mist, and the day
  going by.
- Sound, synthesized as it plays: the papery rustle of bamboo leaves, hollow
  knocks of culm on culm, the kettle's simmer, a bush warbler at dawn,
  crickets at night, and a singing bowl as the eyes open.

## The wind tree

The first study: a single broadleaf tree, grown procedurally, whose branches
are simulated on the CPU and whose sixty thousand leaves are each posed in the
wind on the GPU. Presets for a breeze, a fresh wind and a strong wind; sliders
for the gusts, the branches' stiffness and damping, the leaves' buffeting, the
tree itself and the light. The garden and the grove grew out of it.

## Running them

Open any of the pages in a recent desktop browser with WebGL 2 (Chrome, Edge,
Safari 17 or later, Firefox). A dedicated GPU or Apple silicon is recommended;
**Performance mode** in the garden's and the grove's menus lowers the
resolution for a steadier frame rate.

## Deploying

This repository holds the built pages only. To publish them with GitHub Pages:
**Settings → Pages → Build and deployment → Deploy from a branch →
`main` / `(root)`**. The pages are then served at
`https://<user>.github.io/Garden/`, `…/Garden/bamboo/` and `…/Garden/tree/`.

## Built with

[three.js](https://threejs.org/) and [lil-gui](https://lil-gui.georgealways.com/),
bundled with Vite into single files.
