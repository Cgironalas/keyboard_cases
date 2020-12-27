# Stacked Acrylic Case for a simplified Alice-like Keyboard

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
Reduced layout (64 keys) to fit in a blue pill with possible per key backlight / RGB backlight + TRS connection for extension boards. Could possibly add an extra key (add back rCtrl or a third macro key on the left) if both Spacebars are mapped under the same two pins (not recommended since some people prefer to map them to different functions).

```
[{x:0.15,a:7},"M1"],
[{y:-0.95,x:3.5},"2"],
[{y:-0.95,x:1.5},"~","1",{x:9.85},"-","=",{w:2},"Backspace"],
[{y:-0.1,x:0.15},"M2"],   
[{y:-0.9,x:1.4,w:1.5},"Tab","Q",{x:9.2},"P","[","]",{w:1.5},"\\|"],
[{x:1.25,w:1.75},"Caps","A",{x:9.5},":","\"",{w:2.25},"Enter"],
[{x:1,w:2.25},"L_Shift","Z",{x:9},">","/",{w:1.75},"R_Shift","R_Fn"],
[{x:1,w:1.5},"Ctrl","Win"],
[{r:12,rx:2.75,ry:3.05,y:-3.25,x:1.5},"3","4","5"],
[{x:1},"W","E","R","T"],
[{x:1.25},"S","D","F","G"],
[{x:1.75},"X","C","V","B"],
[{x:1.5,w:1.5},"L_Alt",{w:2.25},"L_Space","L_Fn"],
[{r:-12,rx:13.5,y:-3,x:-4.75},"6","7","8","9","0"],
[{x:-4.25},"Y","U","I","O"],
[{x:-4},"H","J","K","L"],
[{x:-4.5},"B","N","M","<"],
[{x:-4.5,w:2.75},"R_Space",{w:1.5},"R_Alt"]
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
  * Number: 8
  * Diameter: 4.4mm for plastic M2 spacers; 3.1mm for brass M2 spacers; 1.9mm for M2 screws
  * Edge Width: 10mm
* Edge Padding: 10mm for all
* Plate corners: 5mm