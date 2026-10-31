# Console Commands

Launch options and console commands for troubleshooting. None of these are needed for normal
play.

## Switches

Two switches turn off Regionator's workarounds for vanilla bugs, in case one misbehaves after a
game update. They only work as launch options (in Steam, **Properties > Launch Options**), and
can be joined with a comma:

```text
-dpcvars=Regionator.FixFlatRoofSnap=0,Regionator.FixLeftoverMachineEffects=0
```

| Switch | Default | What it does |
|---|---|---|
| `Regionator.FixFlatRoofSnap` | 1 (on) | Stops blueprint holograms vanishing at the side of a Flat Roof. |
| `Regionator.FixLeftoverMachineEffects` | 1 (on) | Removes the smoke some machines leave behind when dismantled. |

## Log detail

For a more detailed log, type `log LogRegionator Verbose` in the console. Switch it back with
`log LogRegionator Log`. The log is at `%LOCALAPPDATA%\FactoryGame\Saved\Logs\FactoryGame.log`.
