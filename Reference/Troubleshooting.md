# Troubleshooting

## Where the log is

`%LOCALAPPDATA%\FactoryGame\Saved\Logs\FactoryGame.log`. The mod logs under `LogRegionator`: one
line per operation with its outcome, plus warnings when something is refused or falls back.

More detail: enter `log LogRegionator Verbose` in the game console, or put
`LogRegionator=Verbose` under `[Core.Log]` in the game's `Engine.ini`. Verbose adds per-frame and
per-building detail.

## Timing a slow dismantle

The console variable `Regionator.TraceDismantle=1` (set at startup, for example with
`-dpcvars=Regionator.TraceDismantle=1` on the launch command line) logs a timeline of each server
dismantle call.

## A blueprint hologram vanishes at a Flat Roof

The vanilla game has a bug where aiming a blueprint hologram at the side of a Flat Roof makes the
hologram vanish for good (a division by the roof's zero height). Regionator fixes it for every
blueprint while the mod is loaded. If the fix ever misbehaves after a game update, it can be
switched off with `-dpcvars=Regionator.FixFlatRoofSnap=0`.

## Common questions

- **The panel is gone**: check **Mods > Regionator > HUD > Show the panel**, and its position; a
  Manual position can be off screen.
- **A key does nothing**: keys stand down while any of the mod's dialogs is open, and chords
  need the exact modifier (`Left Ctrl` by default). Check
  **Options > Keybindings > Regionator** for rebinds. On a controller every command is a chord:
  hold `L3` first; apart from equip they only count while the tool is in hand.
- **The region is red and confirm does nothing**: the selection is over the volume limit.
  Shrink the region, remove one, or raise **Mods > Regionator > General > Selection volume
  limit factor**; see [Limits and Known Issues](Limits-And-Known-Issues).
- **"The selection did not reach the host. Try again."**: a large selection is sent to the host
  in pieces and the host did not answer for 30 seconds. Confirm again; if it repeats, check the
  connection.
- **The blueprint menu appeared before the milestone**: that is the Save Blueprint unlock; see
  [Save Blueprint](Save-Blueprint) for how it behaves and how to take it back.
- **A Move left the originals standing**: that is the safety rule working, not failing; see
  [Move](Move). The log names the reason.

## Reporting a bug

Include the log (the `LogRegionator` lines around the time it happened), what mode you were in,
and roughly what the selection contained. See the mod page for where to report.
