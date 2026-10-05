# FreeCAD Steam Deck Stand Leaner (EU Plug)

Personal project to design a 3D-printable Steam Deck stand in FreeCAD: a
charger cradle that stores the EU power adapter and its cable inside, props
the Deck up, and slides into the strap on the official carrying case in place
of the original support.

This is a remake of
[Steamdeck USB-C Charger Cradle with built in stand (USA Plug)](https://www.printables.com/model/170877-steamdeck-usb-c-charger-cradle-with-built-in-stand)
by Neebick on Printables, redrawn from scratch in FreeCAD (1.1) for the EU
plug.

## Project structure

```
cad/                     # FreeCAD source file (.FCStd)

exports/                 # 3MF export for slicing and printing
└── steamdeck-stand-leaner-eu-plug-Support.3mf

images/                  # reference photo, renders, slicer screenshot and print photos
```

## Design

The stand is a rounded, open tray, sized from the support that ships with
the original Steam Deck carrying case (photographed next to a ruler as a
reference) so that it fits the case strap the same way.

![Original Steam Deck support next to a ruler](images/original-steam-deck-support.png)

Inside, a recess shaped like the EU power adapter holds the charger in
place, with room left along the tray for the coiled USB-C cable.

| | |
|---|---|
| ![Stand, isometric render](images/output_20261005-122137.png) | ![Stand on the Prusa Core One build plate](images/output_20261005-122055.png) |

![FreeCAD model with the EU plug adapter in place](images/freecad-work.png)

Overall size of the exported part: **178.7 × 68.7 × 35.8 mm** (X × Y × Z).

### Model structure

The final part is the `Support` group, built from:

- `RawSupport`: the stand body.
- `steamdeck-eu-plug001`: the shape of the EU plug adapter.
- `Cut`: the stand body minus the plug adapter, which gives the plug recess.

To re-export, select the `Support` group and use *File → Export…* as 3MF.

## Final print

Printed, loaded with the EU charger and its cable, and used both as a desk
stand and in the carrying case strap.

| | |
|---|---|
| ![Empty print next to the EU charger](images/print-empty-with-charger.png) | ![Inside of the print](images/print-inside.png) |
| ![Charger and cable stored in the stand](images/print-charger-stored.png) | ![Charger and cable stored, in hand](images/print-charger-stored-in-hand.png) |
| ![Bottom of the stand](images/print-bottom.png) | ![Stand sliding into the case strap](images/case-strap-sliding-in.png) |
| ![Stand fitted in the case strap](images/case-strap-fitted.png) | ![Steam Deck on the stand, front](images/deck-on-stand-front.png) |
| ![Steam Deck on the stand, angled](images/deck-on-stand-angle.png) | ![Steam Deck on the stand, on top of the case](images/deck-on-case-front.png) |
| ![Steam Deck on the stand on the case, side view](images/deck-on-case-side.png) | |

## License

The original model is published under
[CC BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/)
(Attribution, NonCommercial, ShareAlike), so this remake is shared under the
same license.

## Status

v1.0.0 — first working print, validated with the EU charger and the carrying
case.
