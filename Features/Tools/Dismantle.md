# Dismantle

Hands the whole selection to the game's own dismantle tool, pre-selected.

## How to use it

1. Pick **Dismantle** with the build-mode key, draw a [region](Regions), confirm.
2. The game's dismantle tool comes up holding the selection, and the [HUD](Regionator-HUD) shows the
   refund and where it will go.
3. Fire once to dismantle. Secondary fire cancels and returns the selection untouched.

> [demo placeholder, about 10 seconds: confirm a region, read the HUD, fire]

## While the selection is held

- The game's own multi-select keys still add or remove buildings.
- The game's normal and blueprint dismantle modes can be switched without losing the selection.
- [Targeted containers](Container-Targeting) receive the refund first, then your inventory, then
  one dismantle crate at your feet. The HUD says the split before you fire.
- A building the game's tool would not take is named on the HUD ("N buildings could not be
  handed to the dismantle tool and will be left standing") and in the log, and the completion
  line repeats the count; nothing is silently skipped.

## Large selections

100 buildings or more are dismantled in the background: the build gun is put away and the HUD
shows progress. To stop a running dismantle, equip the build gun and press secondary fire.

The game caps how many buildings one dismantle can hold; the mod raises that cap to the
**Dismantle limit** in the Mods menu, 100000 by default (the value Infinite Dismantle uses, so
the two mods coexist) and up to 1000000. A Dismantle selection is also cut at that limit. In
[multiplayer](Multiplayer) the host's limit applies. Above 3000 buildings the refund estimate is
skipped; the dismantle itself is unaffected.
