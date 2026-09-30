# Replace

Swaps buildings for another type, material or colour, in place. Connections, contents and
positions survive; nothing is dismantled and rebuilt where a restyle will do.

## How to use it

1. Pick **Replace**, draw a [region](Regions), confirm.
2. A popup lists every building type in the selection. For each row, choose what it becomes
   and/or a material and colour. The net cost and refund update as you pick, and Replace greys
   out when you cannot afford it.
3. Confirm the popup. The host re-checks the whole mapping and refuses it if it can no longer be
   paid for.

> [screenshot placeholder: the Replace popup with building rows, a recipe list and the palette]

## What can become another type

Foundations, walls, ramps, roofs, beams, pillars and other architecture, belts, conveyor lifts,
pipes, hypertubes, and floor and wall holes. A candidate must fit the same footprint (belts,
pipes and hypertubes swap within their own family, beams with beams), and only unlocked recipes
are offered.

## Restyle only

Machines, splitters and mergers, pipe junctions and pumps, power poles and lights keep their
type; the material and colour are written onto them where they stand, so their connections, items
and fluid are untouched. A manufacturer row can also set a **production recipe**: the machine is
emptied, the recipe set, and items the new recipe cannot use are handed back. Recipe changes are
free.

## What is kept

Position, curve, beam length, lift height, floor and wall holes, and the connections between
replaced pieces and to everything around them. Items on replaced belts and lifts go back where
they were; any that cannot (the belt runs into a machine with no power, paused, or into nothing)
are handed back at once, and the completion line says why. A replaced pipe keeps its fluid where the new pipe
has room and carries the same fluid. Throughput monitors are rebuilt on the new belt; one that
cannot be is refunded.

## Cost

Each replacement costs its recipe scaled by length, the same way the game refunds a belt, pipe or
beam, so swapping and swapping back cost what they return. The refund of what comes down is
netted against the cost per item. What is owed comes from [targeted containers](Container-Targeting),
then your inventory, then the Dimensional Depot; what is over goes back the same way, then to a
crate. Under No Build Cost the replacements are free and what they replace is refunded in full.

## Left alone

A power pole a player's hover pack is drawing from, and anything whose removal would take down
something Replace cannot put back. The HUD lists the reasons when the job ends.
