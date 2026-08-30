# Codex: A RimWorld Compendium

A dynamic in-game encyclopedia that connects items, creatures, recipes, research,
workbenches and more across your loaded mods. It has extra support for
[Medieval Overhaul](https://steamcommunity.com/sharedfiles/filedetails/?id=3219596926)
to cover its unique mechanics, and stays fully usable with any other mod setup.

For any item it answers the two questions the game itself never answers: where
does this come from, and what is it for. Everything is linked, so you can follow
a chain instead of guessing, from a locked research to the schematic it needs,
to the ruin that schematic drops in and the odds of finding it there.

## What it covers

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

## Combat Extended

With Combat Extended loaded, the vanilla ranged numbers are wrong, so they are
not shown. In their place you get the real ones: range, minimum range, warmup,
burst, recoil, magazine, reload time, sight efficiency and bulk, plus every
ammunition type the weapon fires with its armour penetration.

## Performance

Nothing is built at startup. The index is created the first time you open the
window, and it runs as a loading event with a progress readout, so a very large
mod list does not look like a freeze. If you never open the window, it costs
nothing.

Drawing was measured with Dubs Performance Analyzer. With the window open on its
heaviest page it costs about 0.8 ms per frame, which is less than the vanilla
work tab at 1.1 ms and roughly a quarter of the vanilla research tree at 3.6 ms.
The live occurrence lookup refreshes every few seconds and does not register.

## Usage

Open it with the book button in the toggle row at the bottom right.

## Requirements

Harmony. Nothing else.

## Installing from here

Download the repository and drop the folder into `RimWorld/Mods`. The built
assembly is included, so nothing needs to be compiled.
