# Snap to Origin

Places a [Move](Move) or [Copy](Copy) hologram exactly where its buildings came from, locked, so
nudges move it a known distance from where it stands.

## How to use it

1. While a Move or Copy hologram is up, press **Regionator: snap to origin** (default `Ctrl + H`;
   pad: hold `L3`, press `R3`).
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
- The game limits how far a hologram can be nudged from where it was locked; Infinite Nudge
  lifts that limit.
- It does nothing for a blueprint from the menu (there is no origin to snap to), with the region
  hologram up, or while a dialog is open; the log says why.
