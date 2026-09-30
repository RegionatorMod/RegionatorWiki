# Controller and Steam Deck

Everything the build gun does on a pad works on the tool: place and confirm with primary fire,
step back with secondary fire, lock, nudge and rotate with the game's buttons, and switch the
tool mode or nudge target with the build-mode button. Equip the tool from the hotbar radial, the
build menu or quick switch.

## Modes, nudging and nudge targets

The build-mode button switches the tool mode, as on the keyboard. Once both anchors are down the
region is locked and the game's own nudge controls move it: the D-pad nudges, and the game's
vertical-nudge toggle switches up and down between forward and back and up and down.

While locked, the D-pad is a nudge, so the nudge target (Move Region, Move Anchor 1, Move
Anchor 2) is picked with `L3 + B`, which does what a tap of the build-mode key does; the
[HUD](Regionator-HUD) names it in that step. Unlocking releases the second anchor to the cursor
again, as on the keyboard.

## Chords

Every command has a pad key of its own, a chord on the left stick click. Hold `L3` and press:

- `LB` to equip the tool or put it away.
- `X` to open the [type filter](Type-Filtering).
- `RB` to [target the container](Container-Targeting) you are aiming at.
- `A` to freeze the region and [add another](Regions).
- `Y` to switch the region between a box and a [sphere](Regions).
- `R3` for [Snap to Origin](Snap-To-Origin).
- `B` to switch the nudge target while the region is locked.

All but equip only count while the tool, a blueprint hologram or the dismantle tool is in hand.
Anywhere else `L3` and those buttons are the game's, so sprinting and jumping are untouched; `LB`
is the mod's whenever `L3` is held, so that equip works from anywhere. All of them can be rebound
on the controller page of the options menu without touching the keyboard bindings. The table on
[Controls](Controls) has a controller column for every action.

## Popups on a pad

The [type filter](Type-Filtering), the [Replace](Replace) popup and the
[Save Blueprint](Save-Blueprint) dialog work like the game's own popups on a pad. The left stick
moves between fields, and a frame marks the one in focus. D-pad down jumps to the next section,
for example from the name straight to the icon list. `A` ticks or chooses, and on a text field
opens the on-screen keyboard. Where no field takes it, `A` confirms the popup and `B` cancels
it, as in the game's own popups; the empty strip at the end of each popup is there so a D-pad
press past the last field always reaches that. A hint row at the bottom of the popup lists
these while a pad is in use.

## Switching devices

The [HUD](Regionator-HUD) shows the pad chords while a pad is in use, and switches to keyboard key
caps the moment you pick up the mouse, including mid-hologram.

> [screenshot placeholder: the HUD with pad button captions while placing a region]
