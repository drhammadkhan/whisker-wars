# Whisker Wars

A playable browser prototype of **Whisker Wars**, a real-time god-strategy game inspired by *Baldies* (Creative Edge, 1995). You lead a colony of alley cats: pick them up, give them jobs, breed kittens in cat beds, and drive a coven of bumbling wizards out of the storybook village of Mothwick.

**Play it:** https://drhammadkhan.github.io/whisker-wars/

## How to play

- **Drag a cat** to pick it up. Drop it on a Dojo to make a Scrapper, on a Junk Workshop for a Tinker, or on a bed for a Tabby. You can also click a cat and press **1–4**.
- **Click a bed** to pull a cat out. Two or more Tabbies in a bed breed kittens.
- **Builders** build what you place from the Build menu (B Box, F Dojo, R Workshop, U Upgrade).
- **Tinkers** research gadgets: Yarn Tripwire (Y), Hairball Spitter and Catnip Bomb (C).
- **Watch for glowing runes.** A wizard's spell lands on its rune, so drag cats out of the rune to dodge it.
- Scrappers protect working cats, fight better in packs, and rank up as they win.
- Fling a cat fast to toss it at a wizard.
- To move around, drag empty ground, use WASD or the arrow keys, or drag the minimap. Scroll or pinch to zoom, press H for home and Space to pause.

To win, topple both wizard towers. You lose if every cat uses up its nine lives, or if your last bed is destroyed.

## Tech

The game is a single self-contained `index.html` using a 2D canvas, with no build step and no dependencies apart from Google Fonts. All the art is drawn in code.
