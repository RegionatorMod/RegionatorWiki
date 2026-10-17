# Multiplayer

Multiplayer is tested on a dedicated server with one guest. Two players at once, and hosting
from your own game, are not tested yet. Reports from multiplayer sessions are welcome.

## How it is built

Everything that changes the world (Replace, Move, Copy, Save Blueprint, Fill inputs, Clear items,
building auto pillars, and the dismantle's container routing) runs on the host, from a request your
machine sends. Blueprints are written on the host, and a dedicated server sends the blueprint file
to the player who asked for it.

## What to expect

- Selection, regions, the HUD and all keys are local to you; two players can use the tool at
  the same time.
- Costs and refunds are attributed to the player who confirmed, through their
  [targeted containers](Container-Targeting) and inventory. The game's No Build Cost that
  applies is that player's own.
- The Selection, Dismantle, volume and Auto pillar limits in force are the host's; your own
  settings are ignored while you are connected. See [Limits and Known
  Issues](Limits-And-Known-Issues).
- Your requests reach the host in the order you made them. A large selection is sent in pieces;
  if the host stops answering for 30 seconds the HUD says "The selection did not reach the host.
  Try again."
- While a guest has three jobs still running on the host, or when a new request would take what
  they have running past the host's Selection limit, that request is refused with "The host is
  still working on your earlier jobs. Wait for one to finish, then try again." The host's own
  jobs are not limited this way.
- Before the blueprint milestone, the blueprint menu stays unlocked for everyone while any
  player present has [Save Blueprint](Save-Blueprint) enabled (a guest counts from the first
  time they equip the tool), and is hidden again once nobody present does.

## Known soft spots

- On a dedicated server, selection can miss buildings your game has not received yet.
