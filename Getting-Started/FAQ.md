# FAQ

**Is this a cheat mod?**
No. Dismantles refund what the game refunds, a Copy costs the full build cost, a Move is free
because the originals are taken in exchange (a blueprint kept from it costs its normal cost
when placed from the menu), and Clear deletes fluid rather than refunding it.
The one convenience is that Save Blueprint does not need the blueprint designer.

**Can I remove the mod safely?**
Yes. Everything it builds is a normal building, and its blueprints are normal blueprint files.
One thing first: if your save has not reached the blueprint milestone, untick
**Enable Save Blueprint** and load and save once, so the blueprint menu unlock is taken back
(see [Save Blueprint](Save-Blueprint)).

**Why did my Move leave some buildings behind?**
A belt or power line with an end outside the selection has no copy and stays, and an original
whose copy cannot be verified is kept rather than destroyed. See [Move](Move).

**Why is my Copy red when it comes up after Snap to Origin?**
It is standing on its own originals, which a Copy cannot be built over. Nudge it off; see
[Snap to Origin](Snap-To-Origin).

**Why does a Copy or a Save Blueprint skip the HUB or the Space Elevator?**
They can only be built once, and a blueprint holding one could build it again, so those modes
leave them out. A Move still moves them; see [Blueprints and Cost](Blueprints-And-Cost).

**Can every Move or Copy start on its originals?**
Yes: **Start at origin**, per mode in the Mods menu; see [Snap to Origin](Snap-To-Origin).

**Which mods does it work with?**
These mods are tested with Regionator and kept working on purpose:

- **SnapOn**: splitters and mergers snapped onto machines stay connected through a Move, a Copy
  and a saved blueprint; blueprints saved with an earlier version need saving again. See
  [Blueprints and Cost](Blueprints-And-Cost).
- **Infinite Nudge**: regions and placements nudge and rotate as far as the mod allows, like any
  hologram.
- **Infinite Dismantle**: not needed, since Regionator has its own **Dismantle limit**. With
  both installed, Regionator's limit is the one used (see [Dismantle](Dismantle)).
- **Lights +**: its light beams, even the thinnest, are selected only where a region actually
  touches them.

A mod missing from the list has simply not been checked, which does not mean it fails. If
something goes wrong with one, see [Troubleshooting](Troubleshooting).

**Does it work in multiplayer?**
It is designed for it but not yet play tested; see [Multiplayer](Multiplayer).

**Does it work on a controller?**
Yes, fully; see [Controller and Steam Deck](Controller).

**Is it translated?**
All 26 of the game's languages, including live language switching.

**Where do refunds go?**
Targeted containers first, then your inventory, then a dismantle crate at your feet. See
[Container Targeting](Container-Targeting).

**Can I save while a job is still running?**
Yes. Items a running Clear, Move or Replace is still carrying go into the save as a crate where
they would have been handed back, usually at your feet, and a large dismantle hands over its
refunds before saving. The game you are playing is not affected: no crate appears and the job
finishes as usual. Fluid on its way into a pipe is not saved.

**How big can a selection be?**
Up to the **Selection limit** in the Mods menu, 35000 buildings and foundation-type pieces
together by default, and no larger than the volume limit, a 500 x 500 x 500 m box or the same
volume in any shape by default. Both can be raised; see
[Limits and Known Issues](Limits-And-Known-Issues) and the [Options Reference](Options-Reference).

**Why is my region red, and why does confirm do nothing?**
The selection is over the volume limit. Shrink the region, remove one, or raise the
**Selection volume limit factor** in the Mods menu; see
[Limits and Known Issues](Limits-And-Known-Issues).
