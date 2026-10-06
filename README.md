![Regionator](https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/wiki-updates/images/banner.png)

<p align="center">
  <a href="https://ficsit.app/mod/Regionator"><img alt="Mod Page" height="28" src="https://img.shields.io/badge/ficsit.app-Mod%20Page-F28B28?style=for-the-badge"></a>
  &nbsp;
  <a href="https://github.com/RegionatorMod/RegionatorWiki/wiki"><img alt="Wiki" height="28" src="https://img.shields.io/badge/Wiki-Documentation-F28B28?style=for-the-badge&logo=github&logoColor=white"></a>
  &nbsp;
  <a href="PAYPAL_DONATE_URL"><img alt="Donate with PayPal" height="28" src="https://img.shields.io/badge/PayPal-Donate-003087?style=for-the-badge&logo=paypal&logoColor=white"></a>
</p>


## What it does

- **Dismantle**: the selection will be highlighted in the game's dismantle tool, already selected,
  with the refund shown prior to dismantling.
- **Move**: a hologram will appear from your selection which can be moved to a new location. Machine contents, belt items and pipe fluid are included in the move.
- **Copy**: a hologram will appear from your selection which can be continually rebuilt (or pasted).
- **Replace types**: swap foundations, walls, belts, pipes and more for another type, material or
  color, in place. This mode can also set machine recipes.
- **Save a blueprint**: save any region as a normal blueprint, no Blueprint Designer needed.
- **Clear items**: empty machines, belts, pipes, dropped items and dismantle crates.
- **Fill inputs**: insert Machine input items from your inventory or selected containers.


## Example Use Cases

<details name="examples" open>
<summary><h3 style="display:inline">Selecting an entire factory, dismantle, and refund to a targeted container.</h3></summary>

<img alt="Drawing a box over a factory row and dismantling it all at once" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/wiki-updates/images/dismantle.webp" width="100%" loading="lazy">

</details>

<br>

<details name="examples">
<summary><h3 style="display:inline">Selecting an entire factory to Save as Blueprint without a blueprint designer.</h3></summary>

<img alt="Saving a whole factory as a blueprint without the Blueprint Designer" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/wiki-updates/images/blueprint.webp" width="100%" loading="lazy">

</details>

<br>

<details name="examples">
<summary><h3 style="display:inline">Building a large blueprint using items from targeted containers.</h3></summary>

<img alt="Building a large blueprint with items pulled from targeted containers" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/wiki-updates/images/rebuild_blueprint.webp" width="100%" loading="lazy">

</details>


## Quick start

1. Press `K`, or find **Regionator** in the build menu under **Special > Selection**.
2. Press the build mode key to pick a mode.
3. Click twice to draw a box, adjust it, then click again to confirm. Right-click steps back.
4. `Left Ctrl + B` for a sphere, `Left Ctrl + N` to add a region, `U` to filter types, and a tap
   of `Left Alt` to target a container. Every key can be rebound in the game's keybind menu.




## Supported and Recommended Mods

Regionator has direct support for several mods, many of which we recommend you also play with to enhance your experience.

| Mod            | Supported | Recommended | Notes                                                                                                                                          |
| :----------------- | :-------: | :---------- | :--------------------------------------------------------------------------------------------------------------------------------------------- |
| [Smart!](https://ficsit.app/mod/SmartFoundations)            | ✅ Yes       | ✅ Yes         | Helps with visualizing Regionator selection and current rotation mode.                                                                         |
| [Infinite Nudge](https://ficsit.app/mod/InfiniteNudge)     | ✅ Yes       | ✅ Yes         | Helps with fine adjustments to Regionator selection,<br>and nudging holograms to precise locations.                                            |
| [Lights +](https://ficsit.app/mod/LightsPlus)           | ✅ Yes       | Optional    |                                                                                                                                                |
| [SnapOn](https://ficsit.app/mod/DirectToSplitter)             | ✅ Yes       | Optional    |                                                                                                                                                |
| [Infinite Dismantle](https://ficsit.app/mod/InfiniteDismantle) | ✅ Yes       | ❌ No          | Regionator provides a dismantle limit option in the Mod menu,<br>if Infinite Dismantle is installed, the value set by Regionator is preferred. |


## Good to know

- Container targeting enables you to build large blueprints, even when you cannot hold all the required items in your inventory. Load the items in a container, then target the container while the blueprint hologram is active.
  - Works for any Regionator mode that consumes resources (e.g. copy or replace mode)
  - Containers can also be targeted in dismantle mode. Refunded items will be moved to the containers, then player inventory, then a dismantle crate.
- Big jobs run in the background to prevent lag and freezing for large dismantles or builds.
- A selection holds up to 35000 buildings and 500 x 500 x 500 m by default. Both limits can be
  raised in the Mods menu.
- Multiplayer is not tested yet. Reports are welcome.










---

**Documentation:** https://github.com/RegionatorMod/RegionatorWiki/wiki

**Bugs and feedback:** https://github.com/RegionatorMod/RegionatorWiki/issues
