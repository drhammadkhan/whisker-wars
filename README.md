# Whisker Wars

A playable browser prototype of **Whisker Wars**, a real-time god-strategy game inspired by *Baldies* (Creative Edge, 1995). You lead a colony of alley cats: pick them up, give them jobs, breed kittens in cat beds, and drive a coven of bumbling wizards out of the storybook village of Mothwick.

**Play it:** https://drhammadkhan.github.io/whisker-wars/

## How to play

- **Drag a cat** to pick it up. Drop it on a Dojo to make a Scrapper, on a Junk Workshop for a Tinker, or on a bed for a Tabby. You can also click a cat and press **1–4**.
- **Click a bed** to pull a cat out. Two or more Tabbies in a bed breed kittens. **Double-click a bed** to upgrade it.
- **Builders** build what you place from the Build menu (B Box, F Dojo, R Workshop, U Upgrade).
- **Tinkers** research gadgets: Yarn Tripwire (Y), Hairball Spitter and Catnip Bomb (C).
- **Watch for glowing runes.** A wizard's spell lands on its rune, so drag cats out of the rune to dodge it.
- Scrappers protect working cats, fight better in packs, and rank up as they win.
- Fling a cat fast to toss it at a wizard.
- To move around, drag empty ground, use WASD or the arrow keys, or drag the minimap. Scroll or pinch to zoom, press H for home and Space to pause.
- **Music and sound** start when you press Start level. M toggles music and N toggles sound effects. Both settings are remembered, and the buttons are under Gadgets & game (in Orders on a touchscreen).

### On a phone or tablet

On a touchscreen the game fills the screen, and a bar along the bottom holds the controls. Landscape works best.

- **Tap a cat**, then tap a job (Tabby, Builder, Scrapper, Tinker) in the bar. Dragging a cat lifts it above your finger so you can see where you're dropping it.
- **To build**, tap Box, Dojo or Workshop, tap where it should go (drag to nudge it), then press **Place**. **Keep placing** lets you place several, and **Cancel** stops.
- **Double-tap a bed** to queue its upgrade (Box → Basket Nook → Cat Tree). A Builder does the work.
- **Orders** opens research, bed upgrades, speed, restart and full screen.
- Drag empty ground to look around. Pinch with two fingers to zoom and pan.
- The game pauses itself when you switch apps. On iPhone, use **Share → Add to Home Screen** to play full screen.

### Campaign

Five levels, unlocked in order. Your stars and unlocks are saved in the browser.

| # | Level | Twist |
|---|---|---|
| 1 | The Village Green | The tutorial: topple both towers |
| 2 | Twin Bridges | Raids pick one of two bridges; mud; teleporting Trickster wizards |
| 3 | The Moat | No bridge: survive 7 raids, or glide cats over to topple the towers |
| 4 | The Herb Garden | Three towers, the full invention tree |
| 5 | The Wizard's Tower | Boss: break two rune pylons to drop the Grand Tower's shield, dodge meteors, beat the Grand Wizard |

You lose if every cat uses up its nine lives, or if your last bed is destroyed. Stars: win, finish under the level's par time, and spend 12 lives or fewer.

### Evolution and super powers

Cats earn experience in their current job and evolve. Select an evolved cat and press **Q** (or the ★ button) for its super power.

| Job | Evolves into | Bonus | Super power |
|---|---|---|---|
| Builder (35 s of work) | Master Builder | Builds and repairs 2× faster | **Fortify**: finishes nearby building work and shields those buildings for 25 s |
| Scrapper (6 wizards) | Alley Champion | +50% damage, inspires nearby Scrappers | **Whirlwind**: hits every nearby wizard and knocks them back |
| Tinker (40 research points) | Grand Inventor | Researches 2× faster | **Mech-Mice**: four clockwork mice hunt wizards and explode |
| Tabby (5 kittens) | Queen Mum | Her bed breeds 40% faster | **Purr of Courage**: heals and wakes nearby cats; they can't be scared for 12 s |

Evolution is kept per job, so a cat that changes jobs gets its title back when it returns.

### Inventions

Nine inventions in three branches. Each tier needs the one before it, and each level offers a subset.

- **Traps:** Yarn Tripwire (Y) → Mousetrap Springboard (G), which flings a wizard back over the stream → Catnip Bomb (C)
- **Weapons:** Hairball Spitter → Sardine Catapult (T), a buildable turret → Laser Pointer (L), which bounces spells back at the caster
- **Utility:** Cat Flap Kit (scared Builders and Tinkers hide in beds) → Umbrella Glider (long tosses, even over water) → Clockwork Mouse (K), which lures apprentices

For testing, `?level=3` opens a level directly and `?unlock=all` unlocks every level.

## Tech

The game is a single self-contained `index.html` using a 2D canvas, with no build step and no dependencies apart from Google Fonts. All the art is drawn in code, and all the music and sound effects are synthesised live with the Web Audio API, with no audio files.
