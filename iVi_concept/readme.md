# iVi (possibly split keyboard concepts)

## Left 60s

The "default" configuration, is the left side of a 60% keyboard with the 'align' adjustments. Has multiple possible options for the thumb cluster, split left shift for semi ISO layout, optional stepped "Caps Lock", and a couple extra keys on the edge of the left side.

### KLE horizontal with variants

```json
[{"x":1.25, "w":2}, "", {"x":0.5}, "", "", "Esc", "~\n`", "!\n1", "@\n2", "#\n3", "$\n4", "%\n5"],
[{"x":1.25, "w":2}, "", {"x":0.5}, "", "", {"w":1.5}, "Tab", "Q", "W", "E", "R", "T"],
[{"w":1.5}, "", {"w":1.25, "w2":1.75, "l":true}, "", {"x":1, "w":1.5}, "", {"w":1.75}, "Caps Lock", "A", "S", "D", "F", "G"],
[{"w":2.75}, "Shift", {"x":1}, "", {"w":1.75}, "Shift", "Z", "X", "C", "V", "B"],
[{"x":3.75, "w":1.5}, "", {"w":1.25}, "Ctrl", {"w":1.25}, "Win", {"x":0.5, "w":1.25}, "Alt", "", {"w":2}, "", ""],
[{"y":0.5, "x":3.75, "w":1.25}, "Ctrl", {"w":1.25}, "Win", {"w":1.25}, "Alt", {"x":2, "w":2}, "", "", ""],
[{"y":0.25, "x":9.5}, "", "", {"w":2}, ""],
[{"y":0.25, "x":9.5, "w":2}, "", {"w":2}, ""],
[{"y":0.25, "x":9.5}, "", {"w":3}, ""],
[{"y":0.25, "x":9.5, "w":3}, "", ""]
```

### KLE 12 degrees balanced layout

```json
[{"r":12, "ry":5, "y":-5}, "", "", "Esc", "~\n`", "!\n1", "@\n2", "#\n3", "$\n4", "%\n5"],
["", "", {"w":1.5}, "Tab", "Q", "W", "E", "R", "T"],
[{"w":1.5}, "", {"w":1.75}, "Caps Lock", "A", "S", "D", "F", "G"],
["Fn", {"w":1.75}, "Shift", "Z", "X", "C", "V", "B"],
[{"w": 1.5}, "", {"w":1.25}, "Ctrl", {"w":1.25}, "Win", {"x":0.5, "w":1.25}, "Alt", "", {"w":2}, "", ""]
```


## Right 60s

The "default" configuration, is the right side of a standard 60% with the 'align' adjustments to the bottom row. Has multiple possible options for the thumb cluster, split backspace, split right shift, and option for a more standard 60% bottom right set of keys (removes the recommended VIM based arrow keys).

#### KLE horizontal with variants

```json
[{"x":0.75}, "^\n6", "&\n7", "*\n8", "(\n9", ")\n0", "_\n-", "+\n=", {"w":2}, "Backspace", {"x":1.25}, "~\n`", "|\n\\"],
[{"x":1.25}, "Y", "U", "I", "O", "P", "{\n[", "}\n]", {"w":1.5}, "|\n\\", {"x":2, "w":1.25, "h":2, "w2":1.5, "h2":1, "x2":-0.25}, "Enter"],
[{"x":1.5}, "H", "J", "K", "L", ":\n;", "\"\n'", {"w":2.25}, "Enter", {"x":1}, ""],
[{"x":2}, "N", "M", "<\n,", ">\n.", "?\n/", {"w":2.75}, "Shift", {"x":0.5, "w":1.75}, "Shift", "Fn"],
["", {"w":2}, "", "", {"w":1.25}, "Alt", {"x":0.5}, "Left", "Down", "Up", "Right"],
[{"y":0.5}, "", "", {"w":2}, "", {"x":2, "w":1.25}, "Win", {"w":1.25}, "Menu", {"w":1.25}, "Ctrl"],
[{"y":0.25, "w":2}, "", "", ""],
[{"y":0.25, "w":2}, "", {"w":2}, ""],
[{"y":0.25, "w":3}, "", ""],
[{"y":0.25}, "", {"w":3}, ""]
```

#### KLE 12 degrees balanced layout

```json
[{"r":-12, "rx":1, "ry":2}, "^\n6", "&\n7", "*\n8", "(\n9", ")\n0", "_\n-", "+\n=", {"w":2}, "Backspace"],
[{"x":0.5}, "Y", "U", "I", "O", "P", "{\n[", "}\n]", {"w":1.5}, "|\n\\"],
[{"x":0.75}, "H", "J", "K", "L", ":\n;", "\"\n'", {"w":2.25}, "Enter"],
[{"x":1.25}, "N", "M", "<\n,", ">\n.", "?\n/", {"w":2.75}, "Shift"],
[{"x":-0.75}, "", {"w":2}, "", "", {"w":1.25}, "Alt", {"x":0.5}, "Left", "Down", "Up", "Right"]
```


## Full ~60% --- FINAL

KLE for the full balanced board with both sides angled 12 degrees inwards.

```json
[{"r":12, "ry":5, "y":-5}, "m1", "m2", "Esc", "~\n`", "!\n1", "@\n2", "#\n3", "$\n4", "%\n5"],
["m3", "m4", {"w":1.5}, "Tab", "Q", "W", "E", "R", "T"],
[{"w":1.5}, "m5", {"w":1.75}, "Caps Lock", "A", "S", "D", "F", "G"],
["fn", {"w":1.75}, "Shift", "Z", "X", "C", "V", "B"],
[{"w":1.5}, "", {"w":1.25}, "Ctrl", {"w":1.25}, "Win", {"x":0.5, "w":1.25}, "Alt", "Shift", {"w":2}, "", "Del"],
[{"r":-12, "rx":9.10945, "ry":2.1365, "x":0.75}, "^\n6", "&\n7", "*\n8", "(\n9", ")\n0", "_\n-", "+\n=", {"w":2}, "|\n\\"],
[{"x":1.25}, "Y", "U", "I", "O", "P", "{\n[", "}\n]", {"w":1.5}, "Backspace"],
[{"x":1.5}, "H", "J", "K", "L", ":\n;", "\"\n'", {"w":2.25}, "Enter"],
[{"x":2}, "N", "M", "<\n,", ">\n.", "?\n/", {"w":2.75}, "Shift"],
["Bksp", {"w":2}, "", "Shift", {"w":1.25}, "Alt", {"x":0.5}, "Left", "Down", "Up", "Right"]
```

## Extended Concepts

### Arrows concept
```json
[{"r":12, "ry":5, "y":-5}, "m1", "m2", "Esc", "~\n`", "!\n1", "@\n2", "#\n3", "$\n4", "%\n5"],
["m3", "m4", {"w":1.5}, "Tab", "Q", "W", "E", "R", "T"],
[{"w":1.5}, "m5", {"w":1.75}, "Caps Lock", "A", "S", "D", "F", "G"],
["", {"w":1.75}, "Shift", "Z", "X", "C", "V", "B"],
[{"w":1.5}, "", {"w":1.5}, "Ctrl", {"w":1.5}, "Win", {"w":1.25}, "Alt", "Shift", {"w":2}, "", "Del"],
[{"r":-12, "rx":9.10945, "ry":2.1365, "x":0.75}, "^\n6", "&\n7", "*\n8", "(\n9", ")\n0", "_\n-", "+\n=", {"w":2}, "|\n\\"],
[{"x":1.25}, "Y", "U", "I", "O", "P", "{\n[", "}\n]", {"w":1.5}, "Backspace"],
[{"x":1.5}, "H", "J", "K", "L", ":\n;", "\"\n'", {"w":2.25}, "Enter"],
[{"x":2}, "N", "M", "<\n,", ">\n.","Up", "?\n/", {"w":1.75}, "Shift"],
["Bksp", {"w":2}, "", "Shift",  "Alt", "Left", "Down", "Right", {"w":1.75}, ""]
```

### KLE for variants (horizontal)

```json
[{"x":1.25, "w":2}, "", {"x":0.5}, "", "", "Esc", "~\n`", "!\n1", "@\n2", "#\n3", "$\n4", "%\n5", {"x":1.75}, "^\n6", "&\n7", "*\n8", "(\n9", ")\n0", "_\n-", "+\n=", {"w":2}, "Backspace", {"x":1.25}, "~\n`", "|\n\\"],
[{"x":1.25, "w":2}, "", {"x":0.5}, "", "", {"w":1.5}, "Tab", "Q", "W", "E", "R", "T", {"x":2.75}, "Y", "U", "I", "O", "P", "{\n[", "}\n]", {"w":1.5}, "|\n\\", {"x":2, "w":1.25, "h":2, "w2":1.5, "h2":1, "x2":-0.25}, "Enter"],
[{"w":1.5}, "", {"w":1.25, "w2":1.75, "l":true}, "", {"x":1, "w":1.5}, "", {"w":1.75}, "Caps Lock", "A", "S", "D", "F", "G", {"x":3.25}, "H", "J", "K", "L", ":\n;", "\"\n'", {"w":2.25}, "Enter", {"x":1}, ""],
[{"w":2.75}, "Shift", {"x":1}, "", {"w":1.75}, "Shift", "Z", "X", "C", "V", "B", {"x":4.25}, "N", "M", "<\n,", ">\n.", "?\n/", {"w":2.75}, "Shift", {"x":0.5, "w":1.75}, "Shift", "Fn"],
[{"x":3.75, "w":1.5}, "", {"w":1.25}, "Ctrl", {"w":1.25}, "Win", {"x":0.5, "w":1.25}, "Alt", "", {"w":2}, "", "", {"x":0.25}, "", {"w":2}, "", "", {"w":1.25}, "Alt", {"x":0.5}, "Left", "Down", "Up", "Right"],
[{"y":0.5, "x":3.75, "w":1.25}, "Ctrl", {"w":1.25}, "Win", {"w":1.25}, "Alt", {"x":2, "w":2}, "", "", "", {"x":0.25}, "", "", {"w":2}, "", {"x":2, "w":1.25}, "Win", {"w":1.25}, "Menu", {"w":1.25}, "Ctrl"],
[{"y":0.25, "x":9.5}, "", "", {"w":2}, "", {"x":0.25, "w":2}, "", "", ""],
[{"y":0.25, "x":9.5, "w":2}, "", {"w":2}, "", {"x":0.25, "w":2}, "", {"w":2}, ""],
[{"y":0.25, "x":9.5}, "", {"w":3}, "", {"x":0.25, "w":3}, "", ""],
[{"y":0.25, "x":9.5, "w":3}, "", "", {"x":0.25}, "", {"w":3}, ""]
```


## Left Numpad

A more "useful" configuration, is the left side of a 60% keyboard with a couple extra keys to make it squared off as well as a left side full number pad. Has the same multiple possible options for the thumb cluster as the 60% one, optional stepped "Caps Lock", and a couple extra keys on the edge of the left side. For the left num pad it is also possible to have all keys be 1u instead of have the typical 2Us for `+`, `=`, `0`. 

### KLE for variants (horizontal)

```json
["Num Lock", "/", "*", "-", {"x":0.25, "w":1.5}, "", "Esc", "~\n`", "!\n1", "@\n2", "#\n3", "$\n4", "%\n5"],
["7", "8", "9", {"h":2}, "+", {"x":0.25, "w":1.5}, "", {"w":1.5}, "Tab", "Q", "W", "E", "R", "T"],
["4", "5", "6", {"x":1.25}, "", {"w":1.75}, "Caps Lock", "A", "S", "D", "F", "G"],
["1", "2", "3", {"h":2}, "Enter", {"x":0.25, "w":2.25}, "Shift", "Z", "X", "C", "V", "B"],
[{"w":2}, "0", ".", {"x":1.25, "w":1.25}, "Ctrl", {"w":1.25}, "Win", {"w":1.25}, "Alt", {"x":1.5}, "", {"w":2}, "", ""],
[{"y":0.5, "x":3}, "", {"x":1.25, "w":1.25, "w2":1.75, "l":true}, "", {"x":3, "w":2}, "", "", ""],
[{"x":3}, ""],
[{"y":-0.75, "x":9.5}, "", "", {"w":2}, ""],
[{"y":-0.25, "x":3}, ""],
[{"y":-0.5, "x":9.5 ,"w":2}, "", {"w":2}, ""],
[{"y":-0.5}, "", "", {"x":1}, ""],
[{"y":-0.25, "x":9.5}, "", {"w":3}, ""],
[{"y":0.25, "x":9.5, "w":3}, "", ""]
```

#########################################


## Alive (65%-ish):

### Right Side

#### Right side horizontal with variants

```json
[{"x":0.75},"^\n6","&\n7","*\n8","(\n9",")\n0","_\n-","+\n=",{"w":2},"Backspace",{"x":1.5},"Home",{"x":1},"~\n`","|\n\\"],
[{"y":-0.25,"x":10,"c":"#000000","t":"#ffffff","a":7,"h":2},"Oled"],
[{"y":-0.75,"x":1.25,"c":"#cccccc","t":"#000000","a":4},"Y","U","I","O","P","{\n[","}\n]",{"w":1.5},"|\n\\",{"x":1.5},"End"],
[{"x":1.5},"H","J","K","L",":\n;","\"\n'",{"w":2.25},"Enter",{"x":1.5},"PgUp"],
[{"x":2},"N","M","<\n,",">\n.","?\n/",{"w":2.75},"Shift",{"x":1.5},"PgDn",{"x":1,"w":1.75},"Shift","Fn"],
[{"y":-0.75,"x":10},"Up"],
[{"y":-0.25},"",{"w":2},"",{"w":1.25},"Alt",{"w":1.25},"Win",{"w":1.25},"Menu",{"w":1.25},"Ctrl"],
[{"y":-0.75,"x":9},"Left","Down","Right"],
[{"w":2},"",""],
[{"y":0.25,"w":3},""]
```

#### Right side 12 degrees default

[{r:-12,ry:2.5,x:0.75},"^\n6","&\n7","*\n8","(\n9",")\n0","_\n-","+\n=",{w:2},"Backspace",{x:1.5},"Home"],
[{y:-0.25,x:10,c:"#000000",t:"#ffffff",a:7,h:2},"Oled"],
[{y:-0.75,x:1.25,c:"#cccccc",t:"#000000",a:4},"Y","U","I","O","P","{\n[","}\n]",{w:1.5},"|\n\\",{x:1.5},"End"],
[{x:1.5},"H","J","K","L",":\n;","\"\n'",{w:2.25},"Enter",{x:1.5},"PgUp"],
[{x:2},"N","M","<\n,",">\n.","?\n/",{w:2.75},"Shift",{x:1.5},"PgDn"],
[{y:-0.75,x:10},"Up"],
[{y:-0.25},"",{w:2},"",{w:1.25},"Alt",{w:1.25},"Win",{w:1.25},"Menu",{w:1.25},"Ctrl"],
[{y:-0.75,x:9},"Left","Down","Right"]

### Full angled at 12 degrees

### Full angled at 12 degrees on the left 11 on the right

This one has the issue that the left side is about 0.96mm higher than the right side. That is with the middle parts aligned.

[{r:12,ry:5,y:-5,w:1.5},"","Esc","~\n`","!\n1","@\n2","#\n3","$\n4","%\n5"],
[{w:1.5},"",{w:1.5},"Tab","Q","W","E","R","T"],
["",{w:1.75},"Caps Lock","A","S","D","F","G"],
[{w:2.25},"Shift","Z","X","C","V","B"],
["",{w:1.25},"Ctrl",{w:1.25},"Win",{w:1.25},"Alt",{x:0.5},"",{w:2},"",""],
[{r:-11,rx:8.618,ry:2.02,x:0.75},"^\n6","&\n7","*\n8","(\n9",")\n0","_\n-","+\n=",{w:2},"Backspace"],
[{x:1.25},"Y","U","I","O","P","{\n[","}\n]",{w:1.5},"|\n\\"],
[{x:1.5},"H","J","K","L",":\n;","\"\n'",{w:2.25},"Enter"],
[{x:2},"N","M","<\n,",">\n.","?\n/",{w:2.75},"Shift"],
[{w:2},"","",{w:1.25},"Alt","",{x:0.5},"Left","Down","Up","Right"]

### Full angled at 12 degrees on the left, 11.3 on the right

The left side is about 0.08mm higher than the right side. The middle parts aren't exactly aligned.

[{r:12,ry:5,y:-5,w:1.5},"","Esc","~\n`","!\n1","@\n2","#\n3","$\n4","%\n5"],
[{w:1.5},"",{w:1.5},"Tab","Q","W","E","R","T"],
["",{w:1.75},"Caps Lock","A","S","D","F","G"],
[{w:2.25},"Shift","Z","X","C","V","B"],
["",{w:1.25},"Ctrl",{w:1.25},"Win",{w:1.25},"Alt",{x:0.5},"",{w:2},"",""],
[{r:-11.3,rx:8.618,ry:2.024,x:0.75},"^\n6","&\n7","*\n8","(\n9",")\n0","_\n-","+\n=",{w:2},"Backspace"],
[{x:1.25},"Y","U","I","O","P","{\n[","}\n]",{w:1.5},"|\n\\"],
[{x:1.5},"H","J","K","L",":\n;","\"\n'",{w:2.25},"Enter"],
[{x:2},"N","M","<\n,",">\n.","?\n/",{w:2.75},"Shift"],
[{w:2},"","",{w:1.25},"Alt","",{x:0.5},"Left","Down","Up","Right"]