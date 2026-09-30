# Move

Picks the selection up as a free hologram and places it somewhere else, contents and all. The
originals are removed once the copy stands.

## How to use it

1. Pick **Move**, draw a [region](Regions), confirm.
2. The selection is written as a free temporary blueprint and its hologram is put in your hand.
3. Place it once. Secondary fire drops the move instead.

> [demo placeholder, about 10 seconds: pick up a container row, nudge, place, items carried over]

## What moves with it

- The contents of machines and containers are carried into the copies.
- Items on belts are put back on the copies' belts where they were. One that cannot go on
  (its belt runs into a machine with no power, paused, or into nothing) is handed back at once,
  and the completion line says why.
- The fluid in pipes, fluid buffers and machines goes into the copies where the copy's pipes
  carry the same fluid and have room.
- A throughput monitor on a moved belt moves with it.
- Overclocks move because power shards are part of the blueprint.

## The edges of the selection

A belt or power line with an end outside the selection has no copy and stays where it is. A power
line the game takes down together with its building is refunded. A Move links the copies' belt
and pipe ends to what the originals were connected to outside, once the originals are gone, so a
segment can be moved and put back into the gap it came from (see
[Blueprints and Pricing](Blueprints-And-Pricing) for Auto-Connect).

## Placement

- The copy may be placed over its own originals; they are removed once it stands. That lets a
  machine be nudged into the space it already occupies. Anything else still blocks placement.
- The copies come up facing the way the originals stand, even when the region was drawn at an
  angle, and an off-grid factory keeps its own angle.
- [Snap to Origin](Snap-To-Origin) places the hologram exactly on the originals and lets you
  nudge a known distance from there. With **Start at origin** on (Mods menu, Move section) every
  Move begins that way without the key press.

## Large selections

A Move with hundreds of foundation pieces is written in the background first: the
[panel](The-Panel) counts "Preparing" and "Finishing", then the hologram comes up. With
thousands of pieces the game pauses briefly while it builds the hologram.

## Safety

A Move never removes what it cannot prove it copied: an original whose copy cannot be found stays
standing, with everything it holds. The originals are removed without a refund, because the free
copy is the refund.

## Buildings that can only be built once

The HUB and the Space Elevator move like anything else. A Move that includes one is never kept
under Move History, even with **Save each Move as a blueprint** on, because a blueprint holding
one could build it twice; the panel says so.
