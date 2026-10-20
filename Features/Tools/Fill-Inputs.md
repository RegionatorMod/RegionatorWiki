# Fill Inputs

Puts machine input items into every production machine and every solid-fuel generator (coal,
biomass, nuclear) in the region, from [targeted containers](Container-Targeting) and your
inventory. Fluids are never filled, and a machine with no recipe set is skipped.

## How to use it

1. Target one or more containers holding the ingredients.
2. Pick **Fill inputs**, draw a [region](Regions) over the machines, confirm.
3. The items are taken from the targets first, then your inventory, and split evenly across the
   machines that accept them.

<img alt="Filling the inputs of a row of machines" src="https://raw.githubusercontent.com/RegionatorMod/RegionatorWiki/main/images/pages/fill_inputs.webp" width="800" loading="lazy">

## Choosing what goes in

Only fillable buildings are selected. The [type filter](Type-Filtering) popup gains an
**Items to fill** list beside the building types: an unticked item is not put into any machine.
