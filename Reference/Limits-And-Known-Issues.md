# Limits and Known Issues

## Limits

- One selection holds at most the **Selection limit** from the Mods menu: 35000 buildings and
  foundation-type pieces together by default, and it can be raised to 1000000. Beyond it the
  panel's estimate says it covers only the first ones, and the rest are left out of the
  operation. Machines are counted before foundation pieces, so an over-full selection loses
  foundation pieces first.
- A selection also has a volume limit, the **Selection volume limit factor** in the Mods menu.
  The factor cubed is the most space all your regions may enclose together: the default of 500
  allows a 500 x 500 x 500 m box, or a sphere or several regions of the same volume; it can be
  raised to 10000. While the regions enclose more than that, the region in hand turns red, the
  panel says "Over the volume limit, shrink selection to confirm", and confirming does nothing
  until the selection is made smaller.
- The game's dismantle tool holds at most the **Dismantle limit**, 100000 buildings by default;
  see [Dismantle](Dismantle).
- In [multiplayer](Multiplayer) the host's limits apply to every player.
- At most 64 [targeted containers](Container-Targeting).
- The [Dismantle](Dismantle) refund estimate is skipped above 3000 buildings; the dismantle
  itself is unaffected.
- The HUB and the Space Elevator can only be built once, so [Copy](Copy) and
  [Save Blueprint](Save-Blueprint) leave them out; a [Move](Move) moves them but is never kept as
  a blueprint.

## Known issues

- A very large [Move](Move), [Copy](Copy) or [Save Blueprint](Save-Blueprint) takes a moment:
  the panel counts "Preparing" and then "Finishing" while the blueprint is written, and with
  thousands of pieces the game itself pauses briefly while it builds the hologram. The volume
  limit is there to keep that in bounds.
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
