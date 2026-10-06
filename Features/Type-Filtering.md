# Type Filtering

Leave building types out of the selection, in every mode.

## How to use it

1. With a region drawn over something, press **Regionator: filter building types** (default `U`).
2. A popup lists every building type in the region with a checkbox each. Untick what should be
   left alone.
3. The [HUD](Regionator-HUD) counts what the filter removed, and the outlines follow.
4. Confirm the popup to keep the ticks. Cancel or `Escape` puts them back as they were when the
   popup opened.

> [screenshot placeholder: the filter popup over a mixed region]

## Notes

- Type in the search box above a list to narrow it down. The letters only need to appear in
  order, so `aspfnd` finds Asphalt Foundation. While a search is active, **All** and **None**
  change only the types it shows, and the ones it hides keep their ticks. `Escape` clears the
  search first, then cancels the popup.
- The filter lasts until you change it, across regions and equips.
- In [Dismantle](Dismantle) the list also names the vehicles inside the region, such as Drone or
  Truck. The other modes never select vehicles.
- In [Fill Inputs](Fill-Inputs) the popup also lists the **items to fill**, and in
  [Clear Items](Clear-Items) the **items to clear**, each with its own checkboxes. The two item
  lists are remembered separately. Each list has its own search box.
