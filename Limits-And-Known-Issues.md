# Limits and Known Issues

## Limits

- One request carries at most 5000 buildings and 30000 foundation-type pieces. Beyond that the
  panel's estimate says it covers only the first ones, and the rest are left out of the
  operation.
- At most 64 [targeted containers](Container-Targeting).
- The [Dismantle](Dismantle) refund estimate is skipped above 3000 buildings; the dismantle
  itself is unaffected.
- The HUB and the Space Elevator can only be built once, so [Copy](Copy) and
  [Save Blueprint](Save-Blueprint) leave them out; a [Move](Move) moves them but is never kept as
  a blueprint.

## Known issues

- Selection runs on your machine, so on a server, buildings far away that your game has not
  received yet can be missed, and the [Clear Items](Clear-Items) estimate counts only what you
  can see. A dismantle crate's contents in particular may not have reached your game until you
  open it, so the estimate can undercount a crate; the clear itself takes everything.
- Fluid carried by [Replace](Replace) or [Move](Move) only goes where the pipe network carries
  the same fluid (or none yet) and has room; the rest is lost, as when the game dismantles a
  pipe.
- A [Move](Move) links its copies to what the originals were linked to outside the selection for
  belts and pipes only. A railroad track joins the track graph when it is built, so a copied
  track is joined only where the game's own Auto-Connect joins it.
- Items carried onto a copy's belts during a Move reach other players only when the belt next
  sends its full state.

See also [Multiplayer](Multiplayer) and [Troubleshooting](Troubleshooting).
