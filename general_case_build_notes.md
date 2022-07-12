# General Stacked Acrylic notes

## Plate Keebio

Generate base files for a switch layer and keycaps layer in plate.keeb.io

Use the following settings to copy my preferences:

- Switch Cutouts:
  - Type: MX or MX Opening
  - Cutout Fillet Radius: 0.0 mm
- Stabilizer Cutouts:
  - Type: 3mm Plate for Screw-ins
  - Cutout Fillet Radius: 0.0 mm
- Acoustic Cutouts:
  - Type: Extreme
  - Cutout Fillet Radius: 0.0 mm
- Keyspacing:
  - Horizontal: 19.05 mm
  - Vertical: 19.05 mm

## Hole notes

I typically prefer to re-generate most of the elements generated so that they can be more precise on my build.

* Switch holes: 13.9mm with 0.25mm radius but need to reverse the switches object.
* Screw holes: 2mm.
* Brass spacer holes: 3.5mm.

## SVG files
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