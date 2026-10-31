# Limits and Known Issues

## Limits

All of these are set in the Mods menu. In [multiplayer](Multiplayer) the host's values apply.

| Limit | Default | Range |
|---|---|---|
| Selection limit (buildings per selection) | 35000 | 1000 to 1000000 |
| Selection volume limit factor (side of a cube, in meters) | 500 | 100 to 10000 |
| Dismantle limit (buildings per dismantle) | 100000 | 100000 to 1000000 |
| Auto pillar limit (extra pieces per placement) | 5000 | 100 to 100000 |

- Over the selection limit, the extra buildings are left out, starting with foundations, walls and
  other building pieces, so machines are kept. The HUD's estimate says how many it covers.
- At most 64 [targeted containers](Container-Targeting).
- The [Dismantle](Dismantle) refund estimate is skipped above 3000 buildings.

## Known issues

- With thousands of pieces, a [Move](Move), [Copy](Copy) or [Save Blueprint](Save-Blueprint)
  takes a moment to prepare, and the game may pause briefly as the hologram appears.
- In multiplayer, buildings far away that your game has not received yet can be missed by a
  selection.
- Fluid moved by [Replace](Replace) or [Move](Move) only goes where the pipes carry the same fluid
  and have room; the rest is lost, as when the game dismantles a pipe.
- A moved railroad track only reconnects where the game's own Auto-Connect joins it.
