# vfd-case

A desk case for the VFD clock, modelled in SolidCraft. The face tilts back 15° toward the viewer.

- `pcb.json`: script for the PCB reference model.
- `case.json`: script for the case. It also adds the acrylic and spacers as reference parts, then tilts everything.
- `vfd-case.sc`: the full saved design.

Rebuild: run `pcb.json`, then `case.json`, into a new design. For example, with two MCP `batch` calls using `path`.

## Hardware (all standard metric)
| Qty | Part | Notes |
|---|---|---|
| 4 | M3 × 16 button-head bolt (ISO 7380) | Goes from the front through the acrylic, spacer and PCB into the insert |
| 4 | M3 round spacer, 8 mm long, OD ≤ 6 mm, unthreaded | Sits between the acrylic and the PCB, clearing the VFD by 1.75 mm |
| 4 | M3 heat-set insert, 5.7 mm long, for a Ø4.0 hole | Goes in the case bosses |

**Assembly:**
1. Push the inserts into the bosses with a soldering iron.
2. Stack the acrylic, spacers and PCB.
3. Drop the stack into the front of the case and fit the 4 bolts.

## Case
- **Walls:** 2.4 mm.
- **Front:** a PCB-shaped pocket with 0.3 mm clearance and 2.42 mm corner radius. The acrylic sits flush with the front face.
- **Back:** the USB-C port sits flush with the back face, through a 9.54 × 3.86 mm cutout.
- **Button:** a flexure tongue in the top wall, 14 mm long and 1.4 mm thick, with a nub 0.25 mm above the plunger. The plunger travels 0.23 mm.
- **Base:** a flat base under a wedge foot, tilted 15°.

## Coordinates (PCB frame, before tilt; mm)
- Z is up and the front (VFD side) faces −Y.
- The PCB's front face sits at y = 0.
- The PCB's bottom-left corner, seen from the front, is at the origin.

**Measurements:**
- PCB: 93.8 × 28.8 × 1.6, corner radius 2.12 (a 3 mm caliper chord ÷ √2).
- VFD: 6.25 deep.
- Pins: stick out 2.7, 3.75 tall.
- USB-C: standard 8.94 × 3.26, 10.65 deep.
- Button casing: 4.65 × 2.6, standing 2 off the back of the PCB, with its top edge 0.42 below the PCB's top edge. Its plunger is 1.95 × 0.95 and points up (+Z).
