# Rack

8 in. custom-width minirack, 12U tall, built from 20 × 20 aluminum extrusion.

## Frame

| | |
|---|---|
| External size (W × D × H) | 206 × 350 × 586 mm |
| Usable height | 533.4 mm, 12U (1U = 1.75 in = 44.45 mm) |
| Clear width between uprights | 166 mm |
| Mounting hole pitch | 186 mm, EIA-310 vertical spacing |
| Panel width | 203.2 mm (8 in.) |
| Profile | 20 × 20, 6 mm slot, 6063-T5 |
| Corners | 3-way corner connectors, adding 3.5 mm at each upright end, plus L brackets (see Hardware) |
| Tray mounting | M5 drop-in T-nuts in the front slot |
| Sides | acrylic panels, air flow from U12 (intake) to U1 (exhaust) |

## Cut list

| Item | Qty | Length (mm) |
|---|---|---|
| Upright | 4 | 579 |
| Width rail | 4 | 166 |
| Depth rail | 4 | 310 |
| **Total profile** | | **4220** |

## Hardware

| Item | Qty | In stock | To buy |
|---|---|---|---|
| 3-way corner connector | 8 | 4 | 4 |
| L corner bracket, 2 holes, 45° rib | 24 | 16 | 8 |
| M5 hammer nut, 20 series | 48 | 8 | 40 |
| M5 × 8 button head hex screw, silver | 48 | 0 | 48 |
| M4 × 3 headless hex screw | 64 | 32 | 32 |

Rails only close the base and top frames; there are no intermediate rails.
L brackets go 3 at each of the 8 vertices: one in the side plane, one in the front or back
plane and one lying flat in the base or top frame. Each bracket takes two hammer nuts and two
screws.
The front plane brackets sit behind the panels at Z 20 to 40 and 546 to 566, inside U12 and U1:
the trays of those two units need a notch at the corners.
Each 3-way corner connector takes eight M4 headless screws, two in each leg.

## Unit layout

| U | Use |
|---|---|
| U1 | Exhaust, 2× 140 mm fans |
| U2 | Switch, TP-Link TL-SG108 |
| U3 | 2× Orange Pi Zero 3 |
| U4-5 | NAS |
| U6-7 | Mini PC, AOOSTAR GEM12 |
| U8-9 | GPU, lying, via OCuLink |
| U10-11 | Power: ATX PS/2 at the rear, power bricks in front |
| U12 | Intake, 2× 140 mm fans |

## Files

- `desenhos/mr2020.pdf`: drawing set, five A4 sheets (isometric view, frame assembly, parts and cut list, corner details, rack unit layout)
- `desenhos/`: LaTeX sources, see the root README to build
