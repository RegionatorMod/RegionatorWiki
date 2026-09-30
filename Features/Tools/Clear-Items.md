# Clear Items

Empties machines, belts and pipes in the region, picks up items lying on the ground and clears
dismantle crates. Items go to [targeted containers](Container-Targeting), then your inventory,
then a crate at your feet; fluid is deleted.

## How to use it

1. Pick **Clear items**, draw a [region](Regions), confirm.
2. The HUD estimates what comes out and where it will go; large clears run in the background.

> [demo placeholder, about 8 seconds: clear a belt bus, items landing in a targeted container]

## What is emptied

- Machine inventories: inputs, outputs, buffers and fuel. Power shards and storage containers
  are left alone.
- Belts and conveyor lifts.
- Items lying on the ground: stacks you dropped and dismantle leftovers. Never the world's own
  pickups: berries, nuts and power slugs respawn where they stand and are left alone.
- Dismantle crates. A crate disappears with its last item, the same as emptying it by hand; if
  nothing has room, the items end up in a new crate at your feet. Death crates are never
  touched, and a crate you [targeted as a container](Container-Targeting) is spared.
- The fluid in pipes, fluid buffers, pumps, valves and machines. Fluid is deleted with no refund,
  the same as when the game dismantles a pipe.

## Choosing what to clear

The [type filter](Type-Filtering) popup gains an **Items to clear** list beside the building
types: an unticked item or fluid stays where it is. A belt carrying an unticked item keeps all
its items, so nothing on it is reordered; a dropped stack of an unticked item stays on the
ground, and a crate holding one keeps that stack and stays standing.

## Pipes

A pipe network that is inside the selection as a whole is flushed the way the game flushes one,
so it can carry a different fluid afterwards. Pipe that runs on outside the selection refills
what was cleared once the fluid flows again.
