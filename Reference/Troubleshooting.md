# Troubleshooting

## Common problems

- **The HUD is gone**: check **Mods > Regionator > HUD > Show the panel**, and its position; a
  Manual position can be off screen.
- **A key does nothing**: keys are paused while a Regionator popup is open, and chords need the
  exact modifier (`Left Ctrl` by default). The container key works on a quick tap only. On a
  controller, hold `L3` first.
- **The region is red and confirm does nothing**: the selection is over the volume limit. Shrink
  it, or raise **Selection volume limit factor** in the Mods menu.
- **"The selection did not reach the host. Try again."**: the host did not answer in time.
  Confirm again; if it repeats, check your connection.
- **"The host is still working on your earlier jobs."**: wait for one of your operations to
  finish, then confirm again. See [Multiplayer](Multiplayer).
- **A Move left the originals standing**: a safety rule kept them; see [Move](Move). The log
  names the reason.

## Vanilla bugs Regionator works around

- **A blueprint hologram vanishes at a Flat Roof**: aiming a blueprint at the side of a Flat Roof
  makes the hologram disappear. Regionator prevents this.
- **Smoke stays where a machine stood**: some running machines leave their smoke behind when
  dismantled. Regionator removes it.

If either workaround misbehaves after a game update, it can be switched off; see
[Console Commands](Console-Commands).

## Reporting a bug

The log is at `%LOCALAPPDATA%\FactoryGame\Saved\Logs\FactoryGame.log`. Include the lines
containing `LogRegionator` from around the time it happened, the mode you were in, and roughly
what the selection held. Open an issue at
https://github.com/RegionatorMod/RegionatorWiki/issues (the Get Support button in the Mods menu
goes there too).
