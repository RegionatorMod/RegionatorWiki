# Auto Pillars

Mark the pillars of a blueprint while you save or copy it. Each time the blueprint is placed, the
marked columns reach down to the ground, however high the blueprint stands. The extra pieces are
added to the cost and built with the blueprint.

Off by default: switch it on under **Mods > Regionator > General > Enable auto pillars**. The
switch takes effect at once, with no restart.

> [demo placeholder, about 10 seconds: mark the pillars of a platform, save it, place it on a
> hillside, the pillars reach the ground at every corner]

## Marking

1. In [Save Blueprint](Save-Blueprint) or [Copy](Copy), draw the selection as usual until both
   anchors of a region are down.
2. Press **Regionator: mark auto pillars** (`Left Ctrl + P` on the keyboard, `L3 + LT` on a
   controller; see [Controls](Controls)). The region is frozen and a teal marking region starts.
3. Draw the marking region around the pillars that should reach down. Buildings of the selection
   inside it are outlined in blue instead of the selection's red, and the
   [Regionator HUD](Regionator-HUD) counts them under **Auto pillars**. A marked building whose
   column cannot extend wherever the blueprint goes is outlined in yellow instead and left out of
   that count, and the HUD says why (see [What extends](#what-extends)). With several such
   columns it names one reason at a time: put it right and the next one shows.
4. Confirm as usual.

A marking region adds nothing to the selection: it only marks what the selection already holds.
Draw as many as you need. Secondary fire steps back through them like any region, and they count
toward neither the selection nor the volume limit.

## Placing

While you hold the blueprint, the hologram shows each marked column reaching down to the ground,
or to a lower floor of the same blueprint, measured where the hologram stands. Move it and the
columns follow, and so does the cost. When you place it, the extra pieces are built with it and
charged with it, and dismantling the blueprint takes them down too. Ctrl + Z does not remove them.
A save made while the extra pieces are still going up, the autosave included, waits until they
are all built (at most a minute).

The extra pieces follow the same rules as any building: while a player, a creature or a vehicle
stands where one would go, the hologram turns red and says what is in the way, and the blueprint
cannot be placed until it moves. Columns reach past them to the ground below.

A Copy is placed straight away. A saved blueprint keeps its marks: picking it from the blueprint
menu later extends it the same way, wherever you put it.

## What extends

A column is a stack of marked pieces along one line, at least 10 degrees below level: a pillar
upright, or a slanted support at its own angle. A beam repeats along its length, so a vertical or
slanted beam works as a column too; a beam laid level stacks straight down instead, like any other
piece. A column of several pieces repeats as a whole.

A column does not extend when:

- it holds belts, lifts, pipes, railways or power lines (anything laid along a path);
- it has a gap in it, or one piece of it is less than 10 cm long along the column (a flat roof,
  thin trim);
- one repeat of it holds more than 1024 pieces;
- it already stands on another building of the blueprint;
- nothing solid is within 1 km below it, or it would pass through another column.

One placement adds at most 5000 extra pieces, all columns together. For very tall builds, raise
**Auto pillar limit** under **Mods > Regionator > General** (up to 100000). The extra pieces go up
over a moment after the blueprint is placed, from the top of each column down, so even a very tall
build does not stall the game. A column that would go past the limit does not extend at all. In
multiplayer the host's limit applies to everyone.

## Notes

- Re-saving a blueprint in the Blueprint Designer drops its marks: the buildings may have changed.
  Mark it again with Save Blueprint to get them back.
- Switching Auto pillars off removes the preview and the extra cost at once. The marks stay with
  their blueprints, ready for when you switch it back on.
- In multiplayer each player's own setting applies, host and guests alike: your marked blueprints
  extend when you have Auto pillars on, whatever the other players have chosen.
