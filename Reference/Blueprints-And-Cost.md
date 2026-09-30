# Blueprints and Cost

[Move](Move), [Copy](Copy) and [Save Blueprint](Save-Blueprint) all write a blueprint on the
host; this page is what that blueprint carries and costs.

## The cost

A blueprint's cost is the buildings' build cost plus the machines' power shards and Somersloops,
which every blueprint carries so that a copy keeps its overclock. Items on belts are never part
of a blueprint. A Move is free; a Copy and a menu placement pay that cost per placement.

## Include items in Blueprint

**Mods > Regionator > General > Include items in Blueprint** (off by default) makes Move, Copy
and Save Blueprint also record what the machines and containers hold, the way the game's own
blueprints do, and counts those items into the cost, so nothing is created from nowhere. The
setting is read on your own machine, so in a shared world your answer travels with your request.
A Move carries its originals' contents by hand either way.

## Auto-Connect

In the game's Auto-Connect blueprint build mode, a blueprint lands on a grid, so its open belt,
pipe, hypertube and track ends rarely meet the connections they were built against; the game
bridges a gap but cannot fix an overlap. Regionator helps: when an open end comes within 1.5 m of
a free connection of the same kind facing it, the hologram is moved (never turned) so the ends
meet exactly and the game joins them directly. The game joins only belt ends by itself, so the
host also links a machine, container, splitter or lift port that lands exactly on a free belt or
pipe end. Where several ends could meet, the move that lines up the most wins.

This applies to every blueprint, Regionator's or not, and not while the hologram is snapped to
another blueprint.

## Large blueprints

Blueprints of 100 or more buildings are placed without the game's build effect to speed up placement.

## Buildings that can only be built once

The HUB and the Space Elevator can only be built once, and a blueprint holding one could build it
again. Copy and Save Blueprint leave them out of the selection, and a Move that includes one is
never kept as a blueprint.
