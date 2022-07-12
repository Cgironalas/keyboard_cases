# Notes

## Case gen steps

- Started with keycaps file.
- Added 15.5 (10mm for case width, 0.5 for between "squared" keycaps space and "rounded" inner case, 5mm for spillover) to each side of the document size (31mm on each dimension).
- Moved keebio generated object by 15.5 on each side (15.028).

- Named Keebio generated object to "keycaps".
- Duplicated "keycaps" to "keycaps_space".
- On "keycaps_space" ran "Path->Union" to make them a single edge object.
- With the nodes editor made sure that "keycaps_space" didn't have unnecessary nodes.

- Duplicated "keycaps_space" to "inner_case".
- Moved Top, bottom and corresponding side nodes (including spacer nodes) by 0.5mm.

- Duplicated "inner_case" to "outer_case".
- Remove any "spacer hole" nodes to flatten the shape.
- Moved Top, bottom and corresponding side nodes by 10mm.


- On "inner_case" and "outer_case" ran "Path->Path Effects --> Corners (Fillet/Chamfer)" with:
    - Unit: mm
    - Method: Auto
    - Radius: 5
    - Selected -> Chamfer

- Create 2mm holes for screws with Rx and Ry of 1 (6 for each side, 3 on top 3 on bottom). Should have 4mm to both "inner_case" and "outer_case".
- Duplicate 2mm holes but update Rx and Ry to be 1.75 (for 3.5mm spacer holes). Should have a 3.25mm to both "inner_case" and "outer_case".

- Insert switches spaces 3mm and align them each to the corresponding keycaps spaces.
    - Because of the way the switches one work it does separate all of them so they can be simply aligned with the default tools.

- Add space for micro controler holder.

## General Notes

* Switch holes: 13.9mm with 0.25mm radius but need to reverse the switches object.
* Screw holes: 2mm.
* Brass spacer holes: 3.5mm.


### Keycap Holes (mm)
* 1.00u: 19.05
* 1.50u: 28.575
* 1.75u: 33.3375
* 2.25u: 42.8625
* 2.75u: 52.3875

### Keebio Plate Files
Break Apart | Ctrl-Shift-K
to split keeb.io plate generated object into all individual switches do Path -> Break Apart or Ctrl-Shift-K

### SVG files
- New shapes have: -0.125mm on each side to be aligned with top left corner.
- Starting files positions: -1.786, -1.786
- Corner file positions: -0.472, -0.472
- Add 15mm on the sides to have 5mm of space and leaving the 10mm for the case: 14.528, 14.528
- Add a layer with the keycaps generated from keebio.
- Align them to the center of all the individual switches.
- Make copy of previous layer but with just one shape, not per switch.
- Expand keycaps shape 0.5mm on each direction to give more leaway for keycaps. (May need to add 0.4mm more for stabilizers space).
- Make copy of expanded shape adding/removing 10mm to each side to make it a proper case.
- Add screw / stabilizer holes.
- Add space for USB / TRRS.
- To add roundness to random shapes go to Path -> Path Effect -> Corners (Fillet/Chamfer): mm, Auto, 5 radius.

## Amoeba builds

Amoebas adjust (only for the bottom amoebas, the other edges seem to be unaffected):
- Grab the 5mm spacer hole. Extend it 2mm downwards, and bigger to each side. Square off the corners. Remove that from the inside shape. Add champfer of 3mm to make it smooth.

## Splits

2 mm space for edges on the side that gets connected. They leave 0.52 mm from the switch space to the edge

Quefrency uses 2.2mm for holes, 3.3mm for spacers

## Acrylic Layers

Possible with pro micro based PCBs, possibly handwired. If handwiring will need for one of the open layers to have adjustments for the 2u amoeba extra space on the bottom row

- Ideal:
Top Screws
Top Spacers
Switches 3mm
Switches 5mm
Open1
Open2
Open3
Open4
Bottom

- Optional (needs more than 6mm long screws):
Top Screws
Top Screws
Switches 3mm
Switches 5mm
Open1
Open2
Open3
Open4
Open5
Bottom