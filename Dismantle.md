# Dismantle

Hands the whole selection to the game's own dismantle tool, pre-selected.

## How to use it

1. Pick **Dismantle** with the build-mode key, draw a [region](Regions), confirm.
2. The game's dismantle tool comes up holding the selection, and the [panel](The-Panel) shows the
   refund and where it will go.
3. Fire once to dismantle. Secondary fire cancels and returns the selection untouched.

> [demo placeholder, about 10 seconds: confirm a region, read the panel, fire]

## While the selection is held

- The game's own multi-select keys still add or remove buildings.
- The game's normal and blueprint dismantle modes can be switched without losing the selection.
- [Targeted containers](Container-Targeting) receive the refund first, then your inventory, then
  one dismantle crate at your feet. The panel says the split before you fire.
- A building the game's tool would not take is named on the panel ("N buildings could not be
  handed to the dismantle tool and will be left standing") and in the log, and the completion
  line repeats the count; nothing is silently skipped.

## Large selections

100 buildings or more are dismantled in the background: the build gun is put away and the panel
shows progress. To stop a running dismantle, equip the build gun and press secondary fire.

The game caps how many buildings one dismantle can hold; the mod raises that cap to 100000, the
same value Infinite Dismantle uses, so the two mods coexist.

## Notes

- Refunds follow the game's rules exactly; the mod adds routing, not new refunds.
- The refund estimate is skipped above 3000 buildings to keep the panel responsive; the dismantle
  itself is unaffected.
