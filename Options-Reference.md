# Options Reference

All options are in the game's Mods menu under **Regionator**. Every option applies immediately,
including from the pause menu.

| Section | Option | Default | What it does |
|---|---|---|---|
| General | Include items in Blueprint | Off | Blueprints written by Move, Copy and Save Blueprint keep machine and container contents; see [Blueprints and Pricing](Blueprints-And-Pricing). |
| General | Selection limit | 35000 | How many buildings and foundation pieces one selection can hold, from 1000 to 1000000. Anything past the limit is left out. Larger selections take longer to send and prepare. |
| General | Dismantle limit | 100000 | How many buildings the game's dismantle tool can hold at once, from 1000 to 1000000; see [Dismantle](Dismantle). |
| General | Selection volume limit factor | 500 | The largest space one selection can cover, as the side of a cube in metres, from 100 to 10000: 500 allows 500 x 500 x 500 m, in any shape or split over several regions. Over it the region turns red and cannot be confirmed; see [Limits and Known Issues](Limits-And-Known-Issues). |
| One per mode | Enable [mode] | On | Offer the mode when the build-mode key cycles the tool modes. At least one mode stays enabled. |
| Move | Save each Move as a blueprint | Off | Keep one blueprint per Move under **Regionator > Move History**, named by the time it was made. Its machines are empty unless Include items in Blueprint is on. |
| Move | Start at origin | Off | Every Move begins locked with its buildings exactly on the originals, where [Snap to Origin](Snap-To-Origin) puts it. |
| Copy | Save each Copy as a blueprint | Off | The same, under **Copy History**. |
| Copy | Start at origin | Off | The same, for every Copy. |
| HUD | Show the panel | On | Show [the panel](The-Panel) that reports what the tool is doing. |
| HUD | Position | Top Center | Where the panel sits: nine named spots, or Manual. Picking a spot moves the two sliders below to it; moving either slider by hand switches this to Manual. |
| HUD | Horizontal position, Vertical position | Follow Position | Percent across and down the screen: 0 is the left edge or the top, 100 is the right edge or the bottom. |
| HUD | Size | 5 | How large the panel and its text are, from 1 to 10. |

## Notes

- The three limits have a number box beside the slider, so an exact value can be typed. In
  [multiplayer](Multiplayer) the host's limits apply to every player; your own values are
  ignored while you are connected.
- Disabling **Enable Save Blueprint** before the blueprint milestone hides the blueprint menu
  again; see the note on [Save Blueprint](Save-Blueprint) about removing the mod.
- Keybindings are not here; they are under **Options > Keybindings > Regionator**
  (see [Controls](Controls)).
