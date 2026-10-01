# Troubleshooting

## Where the log is

`%LOCALAPPDATA%\FactoryGame\Saved\Logs\FactoryGame.log`. The mod logs under `LogRegionator`: one
line per operation with its outcome, plus warnings when something is refused or falls back. How
to raise the detail, and the diagnostic switches, are on [Console Commands](Console-Commands).

## A blueprint hologram vanishes at a Flat Roof

The vanilla game has a bug where aiming a blueprint hologram at the side of a Flat Roof makes the
hologram vanish for good (a division by the roof's zero height). Regionator fixes it for every
blueprint while the mod is loaded. If the fix ever misbehaves after a game update, it can be
switched off with `-dpcvars=Regionator.FixFlatRoofSnap=0`.

## The game crashes when closing or loading a save, with SnapOn

With SnapOn, a blueprint holding snapped-on splitters or mergers could crash the game when you
quit or loaded a save after holding it. Regionator now prevents that crash for every blueprint,
Regionator's or the game's own; lines starting `Mod compat: not dismantling` in the log at that
moment are expected. Old blueprints are still worth saving again so their splitters and mergers
connect; see [Blueprints and Cost](Blueprints-And-Cost).

## Common questions

- **The HUD is gone**: check **Mods > Regionator > HUD > Show the panel**, and its position; a
  Manual position can be off screen.
- **A key does nothing**: keys stand down while any of the mod's dialogs is open, and chords
  need the exact modifier (`Left Ctrl` by default). The container key (`Left Alt` by default)
  acts on a quick tap alone: `Alt` held long, or with a click, a scroll or another key, targets
  nothing. Check **Options > Keybindings > Regionator** for rebinds. On a controller every
  command is a chord: hold `L3` first; apart from equip they only count while the tool is in
  hand.
- **The region is red and confirm does nothing**: the selection is over the volume limit.
  Shrink the region, remove one, or raise **Mods > Regionator > General > Selection volume
  limit factor**; see [Limits and Known Issues](Limits-And-Known-Issues).
- **"The selection did not reach the host. Try again."**: a large selection is sent to the host
  in pieces and the host did not answer for 30 seconds. Confirm again; if it repeats, check the
  connection.
- **"The host is still working on your earlier jobs."**: a guest can have at most three jobs
  running on the host at once, and together they stay within the host's Selection limit; see
  [Multiplayer](Multiplayer). Wait for the HUD to report one finished, then confirm again.
- **The blueprint menu appeared before the milestone**: that is the Save Blueprint unlock; see
  [Save Blueprint](Save-Blueprint) for how it behaves and how to take it back.
- **A Move left the originals standing**: that is the safety rule working, not failing; see
  [Move](Move). The log names the reason.

## Reporting a bug

Include the log (the `LogRegionator` lines around the time it happened), what mode you were in,
and roughly what the selection contained, and open an issue at
https://github.com/RegionatorMod/RegionatorWiki/issues (the Get Support button on the mod's entry
in the Mods menu goes there too).
