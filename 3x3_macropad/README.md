# Stacked Acrylic Case for 3x3 macropads

## Recommended Layers for Pro Micro based PCBs

### 3mm Acrylic Layers

* Top Layers (Optional): 2x3mm 
* Switch Layer: 3mm
* Closed Layer: 3mm
* Open Layers: 3x3mm
* Closed Layer (Optional): 3mm
* Bottom Layer: 3mm

If using the two optional top layers (one with screw holes, the other with spacer holes) for a high profile case then I recommend: adding a closed layer between the open layers and the  bottom layer, making the switch layer use holes for the spacers. That way you can use 20mm spacers.

If not using the top layers then make sure the switch layer has holes for screws, and without the optional closed layer between the open layers and the bottom layer you will be able to use 15mm spacers.

(UN-TESTED) If you are using low profile sockets for the pro micro then the closed layer between the switch layer and the open layer may not necessary but I would recommend moving it to the below the open layers to use the spacers mentioned in the last paragraphs.

## KLE Layout

Pretty simple really.
```
["7","8","9"],
["4","5","6"],
["1","2","3"]
```

## SWILLKB Settings

**Switch Type**

I prefer using MX + ALPS `_t:2` for fully acrylic cases because in those scenarios it is better for the space to be as tight as possible for the switch. If using a metalic plate it is possible to use the MX `_t:3` type.

**Stabilizer Type**

Cherry Only

**Case Type**

Sandwich:
* USB Cutout: (0mm, 14mm)
* Mount Holes:
  * Number: 4
  * Diameter: 4.4mm for plastic M2 spacers; 3mm for brass M2 spacers; 1.9mm for M2 screws
  * Edge Width: 10mm
* Edge Padding: 10mm for all
* Plate corners: 5mm