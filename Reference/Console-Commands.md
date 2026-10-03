# Console Commands

Everything the mod accepts from the game's console, all of it for diagnosing or testing. None
of these are needed for normal play. Open the console with the `` ` `` key (press it twice for
the full window), type the line and press Enter.

Three of the switches are read once, when the game starts, so they have to be set on the launch
command line rather than typed in afterwards. In Steam that is **Properties > Launch Options**:

```text
-dpcvars=Regionator.TraceDismantle=1
```

Several can be joined with commas: `-dpcvars=Regionator.TraceDismantle=1,Regionator.FixFlatRoofSnap=0`.

## Switches

| Switch | Default | When it is read | What it does |
|---|---|---|---|
| `Regionator.FixFlatRoofSnap` | 1 (on) | At game start | Keeps the fix for the vanilla bug where a blueprint hologram vanishes for good when aimed at the side of a Flat Roof. Set it to 0 on the launch line if the fix ever misbehaves after a game update; see [Troubleshooting](Troubleshooting). |
| `Regionator.FixLeftoverMachineEffects` | 1 (on) | At game start | Keeps the fix for the vanilla bug where a running Fuel Generator, Foundry, Particle Accelerator or Packager leaves its smoke behind when it is dismantled. Set it to 0 on the launch line if the fix ever misbehaves after a game update; see [Troubleshooting](Troubleshooting). |
| `Regionator.TraceDismantle` | 0 (off) | At game start | Writes a timeline of every dismantle the host runs to the log, step by step with the time each one took. For finding out where a slow dismantle spends its time. |
| `Regionator.TracePadDialog` | 0 (off) | Immediately | Logs every controller button that reaches one of the mod's popups (the type filter, Replace and Save Blueprint) and which field has the focus at the time. For reporting a popup that a pad cannot drive; see [Controller and Steam Deck](Controller). |
| `Regionator.TracePerf` | 0 (off) | Immediately | Every 5 seconds, logs how much time the mod spent in each of its measured tasks (calls, average and longest time). For reporting a stutter while drawing a region, placing a large Move or Copy, or handing a big selection to the dismantle tool. |
| `Regionator.TraceRemoteCalls` | 0 (off) | Immediately | Logs every request your game sends to the host as it is queued and sent. For [multiplayer](Multiplayer) reports. |
| `Regionator.WorkChunkSize` | 0 | Immediately | Sends selections to the host in pieces of at most this many entries. 0 means the normal 4000; larger values count as 4000. For testing. |
| `Regionator.HoldJobs` | 0 (off) | Immediately | Pauses the mod's running jobs (Replace, Move, Fill inputs, Clear items, and a large Copy, Save Blueprint or dismantle) after this many steps, until it is set back to 0. Set it on the host. For testing what happens to a job that is interrupted, by a save for example; leave it at 0 to play. |

Type a switch and its value in the console: `Regionator.TracePadDialog 1` switches it on, `0`
switches it off, and `Regionator.HoldJobs 3` sets a number.

## Commands

| Command | What it does |
|---|---|
| `Regionator.DumpInput` | Writes every input mapping the game currently applies to you to the log, grouped by context: which key or button does what in the build gun, in a hologram, in a menu, and so on. For checking what a key is bound to when a chord seems not to work. |
| `Regionator.DumpInput pad` | The same, listing only the gamepad buttons. |

## Log detail

The mod logs under `LogRegionator`: one line per operation with its outcome, plus warnings when
something is refused or falls back. For more, type `log LogRegionator Verbose` in the console,
or put `LogRegionator=Verbose` under `[Core.Log]` in the game's `Engine.ini`. Verbose adds
per-frame and per-building detail, so switch it back with `log LogRegionator Log` when done.

Everything above lands in `%LOCALAPPDATA%\FactoryGame\Saved\Logs\FactoryGame.log`; see
[Troubleshooting](Troubleshooting) for what to include in a bug report.
