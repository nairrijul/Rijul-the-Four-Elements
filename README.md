# Rijul & the Four Elements

A 2D puzzle platformer for kids. Rijul, the Keeper of Elements, uses fire, water, air and rock to fight pollution villains, clear smog and wildfires, and heal the planet across three levels.

The whole game is a single `index.html` file (HTML, CSS and JavaScript on a canvas). There's nothing to install or build.

## Play it

- **Locally:** download the repo and open `index.html` in any modern browser.
- **Online with GitHub Pages:** in your repo go to **Settings → Pages**, set the source to **Deploy from a branch**, pick `main` and `/ (root)`, then save. After a minute the game is live at `https://<your-username>.github.io/<repo-name>/`.

## Controls

| Key | Action |
|---|---|
| A / D (or ← / →) | Move |
| W (or ↑) | Jump |
| S, or 1–4 | Switch element |
| Space | Shoot |
| M | Sound on/off |
| Enter or click | Start / continue |

On phones and tablets, on-screen buttons appear under the game.

## Elements

| Element | Clears | Defeats |
|---|---|---|
| Air | Smog walls | Smoglings |
| Water | Wildfires | Ember Imps |
| Fire | Powers solar panels (opens gates) | Coal Bots |
| Rock | Rusty factory walls | Trash Golems |

## Villains

| Villain | Weak to | Hits to defeat | Attack |
|---|---|---|---|
| Smogling | Air | 2 | Touch |
| Ember Imp | Water | 3 | Throws embers |
| Coal Bot | Fire | 3 | Shoots smoke |
| Trash Golem | Rock | 4 | Touch |

Rijul has 5 health. Villains take 1 health per hit; oil slicks and falling restart the level right away.

## Levels

1. **Smoggy Rooftops**: air and water
2. **Factory District**: rock and fire, plus a solar-powered gate
3. **Wildfire Forest**: all four elements

Collect the green seeds along the way and watch the Planet health bar fill as you clean up each level.

## Editing levels

Levels are defined in the `LEVELS` array in `index.html` on a 30 × 17 tile grid. Each `R(tile, col, row)` call places a tile:

`#` ground or wall · `=` platform · `I` smog · `F` wildfire · `C` rusty wall · `T` solar panel · `G` gate · `x` oil slick · `o` seed · `P` player start · `E` exit · `s` `e` `b` `g` villains
