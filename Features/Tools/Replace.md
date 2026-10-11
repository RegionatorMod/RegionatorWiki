# Replace

Swaps foundations, walls, belts, pipes and more for another type, material or color, in place,
and can also set machine recipes and clock speeds and change miners between Mk.1, Mk.2 and Mk.3.
Connections, contents and positions survive; nothing is dismantled and rebuilt where a restyle
will do.

## How to use it

1. Pick **Replace**, draw a [region](Regions), confirm.
2. A popup lists every building type in the selection. For each row, choose what it becomes
   and/or a material and color. The net cost and refund update as you pick, and Replace grays
   out when you cannot afford it.
3. Confirm the popup. The host re-checks the whole mapping and refuses it if it can no longer be
   paid for.

> [screenshot placeholder: the Replace popup with building rows, a recipe list and the palette]

## What can become another type

Foundations, walls, ramps, roofs, beams, pillars and other architecture, belts, conveyor lifts,
pipes, hypertubes, and floor and wall holes. A candidate must fit the same footprint (belts,
pipes and hypertubes swap within their own family, beams with beams), and only unlocked recipes
are offered.

Miners can become another miner tier, up or down. The new miner takes over the same resource
node, its belt and power lines stay connected, and the ore inside it, its power shards and its
clock speed carry over. It costs the new miner, less the refund of the old one.

## Restyle only

Machines (other than miners changing tier), splitters and mergers, pipe junctions and pumps,
power poles and lights keep their type; the material and color are written onto them where they
stand, so their connections, items and fluid are untouched. A manufacturer row can also set a
**production recipe**: the machine is emptied, the recipe set, and items the new recipe cannot
use are handed back. Recipe changes are free.

## Clock speed

Every machine whose clock speed the game lets you set (manufacturers, miners, extractors and
generators) gets a **Clock speed** section under the list when its row is open, once the clock
speed is unlocked in the game. Machines of one type on one recipe but at different clock speeds
are listed as separate rows, each tagged with its clock speed. Type a percentage, drag the
slider, or type the output per minute; **Reset** puts the row back to the clock speed its machines
run at now. The output field only appears when every machine in the row makes the same amount, so
a row of miners on nodes of different purity is set by percentage alone.

The range is the machine's own: down to 1%, and up to 100% until overclocking is unlocked, then
up to 250%. Above 100% each machine needs power shards. The shards it is missing are part of the
cost, and a machine left holding more shards than its new clock speed needs has the extra taken
out and handed back. The clock speed changes when the machine finishes the cycle it is on, as it
does with the machine's own slider.

## What is kept

Position, curve, beam length, lift height, floor and wall holes, and the connections between
replaced pieces and to everything around them. Items on replaced belts and lifts go back where
they were; any that cannot (the belt runs into a machine with no power, paused, or into nothing)
are handed back at once, and the completion line says why. A replaced pipe keeps its fluid where the new pipe
has room and carries the same fluid. Throughput monitors are rebuilt on the new belt; one that
cannot be is refunded.

## Cost

Each replacement costs its recipe scaled by length, the same way the game refunds a belt, pipe or
beam, so swapping and swapping back cost what they return. Power shards a new clock speed needs
are part of the cost, and shards taken out are part of the refund. The refund of what comes down
is netted against the cost per item. What is owed comes from [targeted containers](Container-Targeting),
then your inventory, then the Dimensional Depot; what is over goes back the same way, then to a
crate. Under No Build Cost the replacements are free and what they replace gives nothing back, as
with the game's own dismantle. Power shards are still your own: a new clock speed takes the shards
it needs from you and hands back the ones it no longer needs.

## Left alone

A power pole a player's hover pack is drawing from, and anything whose removal would take down
something Replace cannot put back. The HUD lists the reasons when the job ends.

A building that is gone before its turn comes (for example, another player dismantled it while
the job ran) is listed as no longer there. If its refund was helping to pay for the rest, the
difference is taken from the same places as the cost; if some of it cannot be found, the HUD adds
"Not enough materials." at the end.
