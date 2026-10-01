# Container Targeting

Route refunds, removed items and building costs through storage containers instead of your
inventory.

## How to use it

1. Aim at a storage container or a dismantle crate.
2. Press **Regionator: target hovered container** (default `Left Alt`, a quick tap) to toggle it as a target.
   A target is outlined and boxed so it stands out from a distance.

> [screenshot placeholder: two targeted containers with their outline and box]

Up to 64 containers can be targeted. A Dimensional Depot cannot be, nor a death crate: the mod
never puts items into a death crate or takes any out. The key works at every step of the tool in
every mode that moves items or pays for buildings (Save Blueprint does neither, so the key is not
offered there), and also while the build gun holds any blueprint hologram, one from the blueprint
menu as much as a Move or a Copy.

## What flows through the targets

- **Refunds and removed items** ([Dismantle](Dismantle), [Clear Items](Clear-Items),
  [Replace](Replace) overflow): targets first, then your inventory, then one crate at your feet.
- **Building costs** ([Copy](Copy), [Replace](Replace), a blueprint from the menu): paid from
  the targets first, then your inventory and the Dimensional Depot. The game's cost readout
  counts the targets too.
- **[Fill Inputs](Fill-Inputs)**: items come from the targets first, then your inventory.

Before you confirm, the [HUD](Regionator-HUD) says where things will end up, naming only the
destinations that receive something.

## With the game's own dismantle tool

Targeting also works with the game's dismantle tool in hand and no region at all: refunds go to
the targets first. A container already selected for dismantle cannot be targeted, and a target is
never added to the dismantle selection. Putting the dismantle tool away drops its targets.

## Safety rules

A container inside the region cannot be targeted, and one the region is later moved over is
dropped from the targets instead, so a target is never dismantled or moved. Targets last until
the tool is put away, or until a confirmed operation that uses them is over. For a dismantle of
fewer than 100 buildings that is about a second after you fire.
