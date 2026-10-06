# Snap to Origin

Places a [Move](Move) or [Copy](Copy) hologram exactly where its buildings came from, locked, so
nudges move it a known distance from where it stands.

## How to use it

1. While a Move or Copy hologram is up, press **Regionator: snap to origin** (`Left Ctrl + H` on the
   keyboard, `L3 + R3` on a controller; see [Controls](Controls)).
2. The hologram sits exactly on the originals, at the angle they stand at, locked with the game's
   own hologram lock.
3. Nudge it: whole nudge steps along the buildings' own axes, even for buildings off the world
   grid. Place when it is where you want it.

> [demo placeholder, about 8 seconds: snap a Copy onto its originals, nudge 8 m, place, repeat,
> giving evenly spaced rows]

## Behaviour

- Pressing the key again returns to the originals, undoing the nudges, and stays locked. The
  game's lock key unlocks as usual.
- A Copy stays locked after each placement, so nudge and place again makes evenly spaced copies.
  At the originals a Copy is red until nudged off them; a Move may be placed anywhere, including
  over its own originals.
- With Auto-Connect on, a locked hologram is never pulled toward a nearby open end, so each
  nudge moves it exactly one step. Unlocked, it snaps to open ends as usual (see
  [Blueprints and Cost](Blueprints-And-Cost)).
- The game limits how far a hologram can be nudged from where it was locked; Infinite Nudge
  lifts that limit.
- It does nothing for a blueprint from the menu (there is no origin to snap to), with the region
  hologram up, or while a dialog is open; the log says why.

## Start at origin

**Mods > Regionator > Move > Start at origin** and the same option under **Copy** (both off by
default) make every placement of that mode begin this way, locked on the originals, without the
key press. The key still works: press it after nudging to return to the originals.
