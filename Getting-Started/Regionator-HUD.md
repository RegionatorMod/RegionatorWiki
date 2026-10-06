# Regionator HUD

The HUD is the mod's on-screen readout. It follows what you are doing: shaping a region, holding
a dismantle, placing a Move or Copy, or watching a background job.

> [screenshot placeholder: the region HUD with the mode badge, chips row, estimate and key caps]

## While shaping a region

- **Title and badge**: "Regionator" with a colored badge naming the mode (Dismantle red, Replace
  blue, Move orange, Copy purple, Blueprint gold, Fill green, Clear light blue).
- **Chips**: the region shape, the box size or sphere radius in meters, the region count, a live
  count of buildings and types inside, and how many the [type filter](Type-Filtering) removed.
- **Estimate**: what the confirm would do, for example the dismantle refund and where it goes.
  Short notices (in amber) appear here and give way to the estimate again. Over the volume
  limit the line reads "Over the volume limit, shrink selection to confirm" and stays until the
  selection fits; the region in hand is red at the same time (see
  [Limits and Known Issues](Limits-And-Known-Issues)).
- **Keys**: the keys that do something right now, as key caps with their action. The caps follow
  your input device; on a controller the caps name the pad chords.

## While a dismantle is held

Building count, the game's refund, and where it will go: targeted containers, your inventory, and
a dismantle crate for what does not fit. Untargeting a container updates the plan immediately.

## While placing a Move or Copy

The hologram status, and with containers targeted, what is paid from or refunded to them.

## During a background job

A progress bar that climbs steadily with the work done and a detail line naming the step. Large
dismantles, Clear and Fill run this way, and so does writing the blueprint for a Move, Copy or
Save Blueprint with hundreds of foundation pieces ("Preparing N of M", then "Finishing N of M").

Where the HUD sits and how large it is are set under **Mods > Regionator > HUD**; see the
[Options Reference](Options-Reference).
