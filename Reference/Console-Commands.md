# Console Commands

The mod has two switches, both for the rare case where one of its fixes for a game bug
misbehaves after a game update. Neither is needed for normal play.

Both are read once, when the game starts, so they have to be set on the launch command line.
Typing one in the console after the game has started changes nothing until the game is restarted
with it on the launch line. In Steam that is **Properties > Launch Options**:

```text
-dpcvars=Regionator.FixFlatRoofSnap=0
```

Both can be joined with a comma:

```text
-dpcvars=Regionator.FixFlatRoofSnap=0,Regionator.FixLeftoverMachineEffects=0
```

## Switches

| Switch | Default | What it does |
|---|---|---|
| `Regionator.FixFlatRoofSnap` | 1 (on) | Keeps the fix for the vanilla bug where a blueprint hologram vanishes for good when aimed at the side of a Flat Roof. Set it to 0 in the launch options if the fix ever misbehaves after a game update; see [Troubleshooting](Troubleshooting). |
| `Regionator.FixLeftoverMachineEffects` | 1 (on) | Keeps the fix for the vanilla bug where a running Fuel Generator, Foundry, Particle Accelerator or Packager leaves its smoke behind when it is dismantled. Set it to 0 in the launch options if the fix ever misbehaves after a game update; see [Troubleshooting](Troubleshooting). |

## Log detail

The mod logs under `LogRegionator`: one line per operation with its outcome, plus warnings when
something is refused or falls back. For more, type `log LogRegionator Verbose` in the console,
or put `LogRegionator=Verbose` under `[Core.Log]` in the game's `Engine.ini`. Verbose adds more
detail, so switch it back with `log LogRegionator Log` when done.

Everything above lands in `%LOCALAPPDATA%\FactoryGame\Saved\Logs\FactoryGame.log`; see
[Troubleshooting](Troubleshooting) for what to include in a bug report.
