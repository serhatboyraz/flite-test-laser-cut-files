# Flite Test Laser-Cut Files

**English** · [Türkçe](README.tr.md)

Laser-cut files for three [Flite Test](https://www.flitetest.com/) foam-board RC airplanes: the **FT Corsair**, the **FT Explorer**, and the **FT P-51 Mustang**. Each model folder includes the original Flite Test build plans (PDF) and cut files prepared for a laser cutter.

Foam parts are nested for **1000 × 700 mm** foam-board sheets (fotoblok). Wooden parts are separate and are not cut from those sheets.

These are not new aircraft designs. The airplanes, specifications, and plan PDFs belong to Flite Test. The CDR and DXF files are laid out so the parts can be cut on a laser.

## Models

### FT Corsair

Four-channel warbird (throttle, aileron, elevator, rudder), version 1.0 (9 March 2019).

| | |
| --- | --- |
| Designed by | John Overstreet, in collaboration with Flite Test |
| Drawn by | Dan Sponholz |
| Length | 30.75 in (781 mm) |
| Wingspan | 46.00 in (1168 mm) |
| Wing area | 355.5 in² (22.9 dm²) |
| Channels | 4 |

Suggested setup from the plan: 2218B 1080 kv motor, 10×4.7 propeller, 35 A ESC (minimum), four 9 g servos, 2200–2800 mAh 3S or 4S battery. Center of gravity is 2.00 in (50.8 mm) back from the leading edge, as marked on the plan.

### FT Explorer

Trainer that can be built as a 3-channel trainer wing or a 4-channel sport wing.

| | |
| --- | --- |
| Designed by | Josh Bixler |
| Drawn by | Dan Sponholz |
| Length | 36.5 in (927 mm) |
| Wingspan | 57 in (1448 mm) |
| Wing area | 460 in² (29.7 dm²) |
| Channels | 3 (trainer) or 4 (sport) |

Suggested setup from the plan: Park 370–425 motor, 1000 kv minimum, 20–30 A ESC, 2200 mAh 3S battery (minimum), 9 g servos (two for the trainer, four for the sport), 8×4.5 slow-fly or 9×6 propeller. Center of gravity is 2.25 in (57 mm) back from the leading edge.

The plan calls for hobby plywood as well as foam board: a 3/32 in (2.4 mm) firewall and 1/16 in (1.5 mm) control horns. Those wooden parts are in `wood.cdr` and `wood.dxf`.

### FT P-51 Mustang

Flite Test Master Series warbird, four-channel (throttle, aileron, elevator, rudder), version 1.0 (26 May 2020).

| | |
| --- | --- |
| Designed by | John Overstreet |
| Drawn by | Dan Sponholz |
| Length | 41.0 in (1042 mm) |
| Wingspan | 48.25 in (1225 mm) |
| Wing area | 400 in² (26 dm²) |
| Channels | 4 |

Suggested setup from the plan: 2218B 1080 kv motor, 10×4.7 propeller, 35 A ESC (minimum), four 9 g servos, 2250–3000 mAh 4S battery. Center of gravity is 3.0 in (76 mm) back from the leading edge. The plan lists 12° throws and 30% expo.

The wooden sheet on the plan is 3/32 in (2.4 mm) plywood. Those parts are in `woods.cdr` and `woods.dxf`.

## Repository layout

```
flite/
├── ft-corsair/
│   ├── ft-corsair-1.cdr      Laser parts, sheet 1 (CorelDRAW)
│   ├── ft-corsair-2.cdr      Laser parts, sheet 2 (CorelDRAW)
│   ├── wood.cdr              Wooden parts (CorelDRAW)
│   └── ft-corsair.pdf        Flite Test all-in-one plan
├── ft-explorer/
│   ├── 3ch-explorer-parts-1.cdr / .dxf   3-channel parts, sheet 1
│   ├── 3ch-explorer-parts-2.cdr / .dxf   3-channel parts, sheet 2
│   ├── 4ch-explorer-parts-1.cdr / .dxf   4-channel parts, sheet 1
│   ├── 4ch-explorer-parts-2.cdr / .dxf   4-channel parts, sheet 2
│   ├── wood.cdr / wood.dxf               Wooden parts
│   └── ft-explorer.pdf                   Flite Test full-size plan
└── ft-p51/
    ├── p51-parts-1.cdr                   Laser parts, sheet 1 (CorelDRAW)
    ├── p51-parts-2.cdr                   Laser parts, sheet 2 (CorelDRAW)
    ├── p51-parts-3.cdr                   Laser parts, sheet 3 (CorelDRAW)
    ├── p51-parts-4.cdr                   Laser parts, sheet 4 (CorelDRAW)
    ├── woods.cdr / woods.dxf             Wooden parts
    └── P51.pdf                           Flite Test full-size plan
```

Pick **one** Explorer variant. `3ch` is the trainer (no ailerons). `4ch` is the sport wing with ailerons. Each variant is split across two sheets.

## File formats

| Extension | Use |
| --- | --- |
| `.dxf` | Send this to the laser. Opens in LightBurn, RDWorks, LaserGRBL, Inkscape, and most cutter software. AutoCAD DXF R2018. |
| `.cdr` | CorelDRAW source. The Corsair foam sheets and the P-51 foam sheets are CDR only; export a DXF from CorelDRAW if the cutter software cannot open CDR. The P-51 wooden parts already include a DXF (`woods.dxf`). |
| `.pdf` | Original Flite Test plan. Use it to build the airplane: part names, folds, scores, bevels, and electronics. |

Before cutting, confirm the drawing is **1:1**. A scaled import will not fit the airframe.

Explorer DXF files are a single layer of geometry. The plan PDF distinguishes cuts, scores, creases, and bevels. Do not cut every line. Foam-board scores and fold lines must stay as scores.

## Build notes

- Foam parts are laid out for **1000 × 700 mm** fotoblok (foam board) sheets. Follow the sheet layout and part callouts in the PDF.
- Wooden parts (spars, firewall, control horns) come from the `wood` files (`woods` in the P-51 folder). Match the thickness printed on the plan.
- Electronics, throws, and expo are printed on the plan sheets. Those figures are a starting setup, not a guarantee for every power system.
- Build videos and the current plans are on [flitetest.com](https://www.flitetest.com/).

## Credit and use

The FT Corsair, FT Explorer, and FT P-51 Mustang designs, and the plan PDFs in this repository, are by **Flite Test, LLC**.

The Corsair plan is marked:

> © 2019 FliteTest, LLC. Plans provided free of charge. Copies allowed for personal use only. Not for commercial use.

The P-51 plan is marked:

> © 2020 FliteTest, LLC. Plans provided free of charge. Copies allowed for personal use only. Not for commercial use.

Use these files for your own builds. Do not sell the plans, the cut files, or kits made from them.

- FT Corsair: designed by John Overstreet with Flite Test, drawn by Dan Sponholz, version 1.0 (2019).
- FT Explorer: designed by Josh Bixler, drawn by Dan Sponholz.
- FT P-51 Mustang: designed by John Overstreet, drawn by Dan Sponholz, version 1.0 (2020).
