# Dismantle

The selection is highlighted in the game's own dismantle tool, already selected, with the refund
shown before you dismantle.

## How to use it

1. Pick **Dismantle** with the build-mode key, draw a [region](Regions), confirm.
2. The game's dismantle tool comes up holding the selection, and the [HUD](Regionator-HUD) shows the
   refund and where it will go.
3. Fire once to dismantle. Until you fire, secondary fire cancels and returns the selection
   untouched.

<img alt="Confirming a region over a factory, reading the HUD and dismantling it" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/main/images/pages/dismantle.webp" width="800" loading="lazy">

## While the selection is held

- The game's own multi-select keys still add or remove buildings.
- The game's normal and blueprint dismantle modes can be switched without losing the selection.
- [Targeted containers](Container-Targeting) receive the refund first, then your inventory, then
  one dismantle crate, which the game drops where the buildings stood. The HUD says the split
  before you fire. Under the game's No Build Cost only what the buildings hold comes back, as with
  the game's own dismantle.
- If your game has a refund stack limit (how many stacks of a refund may go to your inventory,
  changed only through cheats or other mods), the targeted containers still take what they can
  first. Past the limit the game's own rule applies: what it would throw away is thrown away, and
  the HUD counts it before you fire ("N discarded over your refund stack limit").
- A building the game's tool would not take is named on the HUD ("N buildings could not be
  handed to the dismantle tool and will be left standing") and in the log, and the completion
  line repeats the count; nothing is silently skipped.

## Buildings in use

Buildings in a [Move](Move) cannot be dismantled from the moment the Move is confirmed until its
originals are removed. The same goes while a large [Copy](Copy) or
[Save Blueprint](Save-Blueprint) is being written, until its hologram comes up or the blueprint
is saved. This applies to every player, and the game's dismantle tool shows "Being moved or saved
by Regionator" over them.

## Vehicles

Trucks, tractors, explorers, drones and trains inside the region are selected too: outlined,
counted, and listed by name in the [type filter](Type-Filtering), so they can be left out. A
vehicle driving through the region at the moment you confirm is taken as well. Only Dismantle
selects vehicles; the other modes leave them alone.

## Large selections

100 buildings or more are dismantled in the background: the build gun is put away and the HUD
shows progress. Once it has started, a dismantle runs to the end.

The game caps how many buildings one dismantle can hold; the mod sets that cap to the
**Dismantle limit** in the Mods menu, from 100000 (the default) to 1000000. It applies to the
game's own dismantle tool too, and with Infinite Dismantle installed Regionator's limit is the
one used. A Dismantle selection is also cut at that limit. In
[multiplayer](Multiplayer) the host's limit applies. Above 3000 buildings the refund estimate is
skipped; the dismantle itself is unaffected.
