![Regionator](https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/main/images/banner.png)

<p align="center">
  <a href="https://ficsit.app/mod/Regionator"><img alt="Mod Page" height="28" src="https://img.shields.io/badge/ficsit.app-Mod%20Page-F28B28?style=for-the-badge"></a>
  &nbsp;
  <a href="https://github.com/RegionatorMod/RegionatorWiki/wiki"><img alt="Wiki" height="28" src="https://img.shields.io/badge/Wiki-Documentation-F28B28?style=for-the-badge&logo=github&logoColor=white"></a>
  &nbsp;
  <a href="https://www.paypal.com/ncp/payment/786A5N7Q7THKL"><img alt="Donate with PayPal" height="28" src="https://img.shields.io/badge/PayPal-Donate-003087?style=for-the-badge&logo=paypal&logoColor=white"></a>
</p>


## What it does

Draw a box or sphere around any part of your factory, then pick what happens to everything inside:

- **Dismantle**: the game's own dismantle tool opens with the whole selection already picked, and
  shows the refund before you fire.
- **Move**: your selection becomes a hologram you place somewhere else. Machine contents, belt
  items and pipe fluid come along.
- **Copy**: your selection becomes a hologram you can build again and again, at the normal cost.
- **Replace**: swap foundations, walls, belts, pipes and more for another type, material or color,
  in place. It can also set machine recipes and clock speeds, and change miner tiers.
- **Save a blueprint**: save any selection as a normal blueprint, no Blueprint Designer needed.
- **Clear items**: empty machines, belts and pipes, and pick up dropped items and dismantle crates.
- **Fill inputs**: fill machines and solid-fuel generators from your inventory or targeted
  containers.

Also included:

- **Auto pillars**: mark the pillars of a blueprint when you save or copy it, and they reach down
  to the ground wherever you place it, with the extra pieces added to the cost. Off by default:
  turn it on under **Mods > Regionator > General**.
- **Container targeting**: tap `Left Alt` on a storage container to pay for builds from its
  items, so a large blueprint is not limited by what fits in your inventory. Dismantle refunds and
  cleared items can be sent into it too.

## Example Use Cases

<details name="examples" open>
<summary style="cursor:pointer"><h3 style="display:inline">Dismantle an entire factory and send the refund to a targeted container</h3></summary>

<img alt="Drawing a box over a factory row and dismantling it all at once" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/main/images/dismantle.webp" width="800" loading="lazy">

</details>

<br>

<details name="examples">
<summary style="cursor:pointer"><h3 style="display:inline">Save an entire factory as a blueprint without the Blueprint Designer</h3></summary>

<img alt="Saving a whole factory as a blueprint without the Blueprint Designer" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/main/images/blueprint.webp" width="800" loading="lazy">

</details>

<br>

<details name="examples">
<summary style="cursor:pointer"><h3 style="display:inline">Build a large blueprint with items from targeted containers</h3></summary>

<img alt="Building a large blueprint with items pulled from targeted containers" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/main/images/rebuild_blueprint.webp" width="800" loading="lazy">

</details>


## Quick start

1. Press `J`, or find **Regionator** in the build menu under **Special > Selection**.
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
| [Infinite Dismantle](https://ficsit.app/mod/InfiniteDismantle) | ✅ Yes       | ❌ No          | Regionator provides a dismantle limit option in the Mods menu,<br>if Infinite Dismantle is installed, the value set by Regionator is preferred. |


---

**Multiplayer:** tested on a dedicated server with one guest. Two players at once, and hosting from
your own game, are not tested yet. Reports are welcome.

**Documentation:** https://github.com/RegionatorMod/RegionatorWiki/wiki

**Bugs and feedback:** https://github.com/RegionatorMod/RegionatorWiki/issues
