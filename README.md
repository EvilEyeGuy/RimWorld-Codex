# Codex: A RimWorld Encyclopedia

![Codex](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/preview.png?v=2)

A dynamic in-game encyclopedia that connects items, creatures, recipes, research,
workbenches and more across your loaded mods. It has extra support for
[Medieval Overhaul](https://steamcommunity.com/sharedfiles/filedetails/?id=3219596926)
to cover its unique mechanics, and stays fully usable with any other mod setup.

For any item it answers the two questions the game itself never answers: where
does this come from, and what is it for. Everything is linked, so you can follow
a chain instead of guessing, from a locked research to the schematic it needs,
to the ruin that schematic drops in and the odds of finding it there.

## What it covers

![What a page shows](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/02_what_it_shows.png?v=2)

- **Items, buildings, plants and materials**: recipes, processing chains,
  mining, harvesting, smelting, construction costs and stats
- **Creatures**: combat power, armour, attacks with damage per second, and where
  they occur: biomes with commonality, events, factions, or the container they
  hide in
- **Pawns**: every pawn kind with its faction variants, skills, possible weapons
  and apparel, plus a generated example
- **Factions, traders and royal titles**, including full room and apparel
  requirements
- **Research**: what it unlocks, what it leads to, and what blocks it, meaning
  schematics, techprints, benches and prerequisites
- **Structures**: the ruins and hideouts of the world generator, drawn as a floor
  plan in the colours of the materials they are built from, with every possible
  layout as a tab, what you can loot there, and how you come across the place

While a game is running, each page also shows where that thing currently is on
your maps, in stockpiles, carried by a pawn or out with a caravan. Clicking the
entry jumps the camera there, and clicking again walks through the other copies.

Floor plans give away what a ruin looks like inside, so they start blurred and
uncover on a click. You can turn that off in the mod settings.

Nothing is hard-coded. The index is generated at runtime from whatever mods you
have installed, so it stays correct when they update and it covers modded content
the same way it covers vanilla.

The Medieval Overhaul support reads what is otherwise invisible: monster drop
chances, loot table percentages, which schematic a research project needs, which
container a mimic is hiding in, and what the Explorer's Workbench can discover.

## Two ways to read a page

![Two ways to read it](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/03_two_views.png?v=2)

Every page starts with the two questions it exists for open and the rest folded
away, with a count on each folded heading. The button in the top right corner
strips it further, down to where it comes from, what it is for and what it does,
with a single search field and no filters. The game remembers your choice.

Anything built from a material carries a picker. Choose granite instead of wood
and the market value, the mass, the hit points, the beauty and the work all
follow. Opening the Codex from something on your map sets the material for you.

## What it reads

![What it reads](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/06_what_it_reads.png?v=2)

## Works with anything

![Works with](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/05_works_with.png?v=2)

## Combat Extended

With Combat Extended loaded, the vanilla ranged numbers are wrong, so they are
not shown. In their place you get the real ones: range, minimum range, warmup,
burst, recoil, magazine, reload time, sight efficiency and bulk, plus every
ammunition type the weapon fires with its armour penetration.

## Performance

![Performance](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/07_performance.png?v=3)

Nothing is built at startup. The index is created the first time you open the
window, and it runs as a loading event with a progress readout, so a very large
mod list does not look like a freeze. If you never open the window, it costs
nothing.

Drawing was measured with Dubs Performance Analyzer on a paused colony. With the
window open on its heaviest page it costs about 1.05 ms per frame, roughly the
same as the vanilla work tab at 1.02 ms and a fifth of the vanilla research tree
at 4.90 ms. In the small panel view the same page costs about 0.24 ms, so
leaving it open beside the game is close to free. The live occurrence lookup
refreshes every few seconds and does not register.

## Usage

![Where to open it](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/04_where_to_open.png?v=2)

Open it with the book button in the toggle row at the bottom right.

## Questions

![FAQ](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/08_faq.png?v=2)

## Credits

![Credits](https://raw.githubusercontent.com/EvilEyeGuy/RimWorld-Codex/workshop/09_credits.png?v=2)

## Requirements

Harmony. Nothing else.

## Installing from here

Download the repository and drop the folder into `RimWorld/Mods`. The built
assembly is included, so nothing needs to be compiled.
