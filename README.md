# Codex: A RimWorld Compendium

A dynamic in-game encyclopedia that connects items, creatures, recipes, research,
workbenches and more across your loaded mods. It has extra support for
[Medieval Overhaul](https://steamcommunity.com/sharedfiles/filedetails/?id=3219596926)
to cover its unique mechanics, and stays fully usable with any other mod setup.

For any item it answers the two questions the game itself never answers: where
does this come from, and what is it for. Everything is linked, so you can follow
a chain instead of guessing — from a locked research to the schematic it needs,
to the ruin that schematic drops in and the odds of finding it there.

## What it covers

- **Items, buildings, plants and materials** — recipes, processing chains,
  mining, harvesting, smelting, construction costs and stats
- **Creatures** — combat power, armour, attacks with damage per second, and where
  they occur: biomes with commonality, events, factions, or the container they
  hide in
- **Pawns** — every pawn kind with its faction variants, skills, possible weapons
  and apparel, plus a generated example
- **Factions, traders and royal titles**, including full room and apparel
  requirements
- **Research** — what it unlocks, what it leads to, and what blocks it:
  schematics, techprints, benches and prerequisites

Nothing is hard-coded. The index is generated at runtime from whatever mods you
have installed, so it stays correct when they update and it covers modded content
the same way it covers vanilla.

The Medieval Overhaul support reads what is otherwise invisible: monster drop
chances, loot table percentages, which schematic a research project needs, which
container a mimic is hiding in, and what the Explorer's Workbench can discover.

## Performance

Nothing is built at startup. The index is created the first time you open the
window, which takes a fraction of a second. If you never open it, it costs
nothing.

## Usage

Open it with the book button in the toggle row at the bottom right.

## Requirements

Harmony. Nothing else.

## Installing from here

Download the repository and drop the folder into `RimWorld/Mods`. The built
assembly is included, so nothing needs to be compiled.
