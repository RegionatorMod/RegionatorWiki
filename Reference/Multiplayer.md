# Multiplayer

Designed for it, not yet play tested. Reports from multiplayer sessions are welcome.

## How it is built

Everything that changes the world (Replace, Move, Copy, Save Blueprint, Fill inputs, Clear items,
and the dismantle's container routing) runs on the host, from a request your machine sends.
Blueprints are written on the host, and a dedicated server sends the blueprint file to the player
who asked for it.

## What to expect

- Selection, regions, the HUD and all keys are local to you; two players can use the tool at
  the same time.
- Costs and refunds are attributed to the player who confirmed, through their
  [targeted containers](Container-Targeting) and inventory.
- The Selection, Dismantle and volume limits in force are the host's; your own settings are
  ignored while you are connected. See [Limits and Known Issues](Limits-And-Known-Issues).
- A large selection is sent to the host in pieces. If the host stops answering for 30 seconds
  the HUD says "The selection did not reach the host. Try again."

## Known soft spots

- Nothing has been verified in a real multiplayer session yet, so treat every multiplayer oddity
  as worth reporting.
- On a dedicated server, selection can miss buildings your game has not received yet.
- Items carried onto a copy's belts during a Move reach other players only when the belt next
  sends its full state.
