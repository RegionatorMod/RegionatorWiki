# Save Blueprint

Files any region as a real blueprint in the game's blueprint menu. No blueprint designer needed,
and the region can be any size.

## How to use it

1. Pick **Save Blueprint**, draw a [region](Regions), confirm.
2. A dialog asks for the name (up to 200 characters), a description, a background colour (the
   game's colour picker) and an icon, picked from the game's icon database with a search box.
3. Save. The blueprint is filed under **Regionator > Blueprints** in the blueprint menu, with a
   number added to the name if it was taken.

> [screenshot placeholder: the save dialog with the icon search open]

## Notes

- The blueprint is a native one: build it from the menu, dismantle it with blueprint dismantle,
  share the file like any other blueprint.
- What it carries and costs is on [Blueprints and Cost](Blueprints-And-Cost).
- The HUB and the Space Elevator can only be built once, so they are left out of the selection.
- Saving a blueprint moves no items, so the target-container key is not offered in this mode.
- A region with hundreds of foundation pieces is written in the background: the
  [HUD](Regionator-HUD) counts "Preparing" and "Finishing" before the blueprint is filed.
- The game hides the blueprint menu until the blueprint milestone. While Save Blueprint is
  enabled (Mods menu) the menu is unlocked; switching the mode off before reaching the milestone
  hides it again.

> Removing the mod from a save that has not reached the blueprint milestone: untick
> **Enable Save Blueprint** first, then load and save once, so the unlock stored in the save is
> taken back.
