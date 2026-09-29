# Regions

A region says which buildings you mean. Machines, belts, pipes, foundations, walls, beams and
modded buildings are all selectable; what happens to them is the [tool mode's](Home) job.

## What counts as inside

A building is selected when the region touches any part of it; it does not have to be fully
enclosed. Touching is judged by the building's real shape, so a region that passes beside a
machine without clipping it leaves the machine out, whatever angle either of them stands at.

## Boxes

1. Click to fix the first corner.
2. The box previews between that corner and the cursor; everything inside is outlined and the
   [panel](The-Panel) counts it. Click (or press the hologram lock key) to fix the second corner.
3. The region locks. The game's nudge keys move it; the build-mode key picks what they move:
   **Move Region**, **Move Anchor 1** or **Move Anchor 2** (the anchors that would move are
   marked red; on a controller press `L3 + B` instead, see
   [Controller and Steam Deck](Controller)). Scroll rotates the region with the game's rotation
   step.
4. Click to confirm, or secondary fire to step back one stage.

Unlocking lets anchor 2 follow the cursor again. Mods that turn or scale holograms (Infinite
Nudge, pitch and roll modes) shape the region the same way.

## Spheres

`Ctrl + B` (Regionator: toggle region shape; `L3 + Y` on a controller) switches between box and
sphere; the shape sticks for later regions and the next equip. The first click sets the centre,
the second the radius, which the panel reads out in metres. In the adjust step the nudge targets
are **Move Center** and **Adjust Radius**; a nudge along the line from the centre changes the
radius by exactly the nudge step. Scrolling leaves a sphere as it is.

> [demo placeholder, about 8 seconds: toggle to sphere, grow it over a tank farm, adjust the radius]

## Several regions

With both anchors down, `Ctrl + N` (Regionator: add region) freezes the current region (drawn
fainter) and starts a new one on the cursor. There is no limit. The selection is the union of
every region: a building in two of them counts once, boxes and spheres mix freely, and each keeps
the angle it was drawn at. Nudging and rotating only move the region being shaped. Stepping back
before the new region's first anchor is down drops it and takes up the previous one again.

## Rotation and what it means

The angle a region is drawn at only selects buildings. A [Move](Move) or [Copy](Copy) of a
rotated region comes up facing the way the originals stand, not turned by the region.
