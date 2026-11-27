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
| 4 | M3 heat-set insert, 5.7 mm long, for a Ø4.0 hole | Goes in the case bosses. The thread is in the insert, so no nuts are needed |
| 4 | Ø8 self-adhesive rubber bumper, 2–3 mm tall | Sits in the recesses under the lip |

**Assembly:**
1. Push the inserts into the bosses with a soldering iron.
2. Stack the acrylic, spacers and PCB.
3. Drop the stack into the front of the case and fit the 4 bolts.

## Case
- **Walls:** 2.4 mm.
- **Front:** a PCB-shaped pocket with 0.3 mm clearance and 2.42 mm corner radius. The acrylic sits flush with the front face.
- **Back:** the USB-C port sits flush with the back face, through a 9.54 × 3.86 mm cutout.
- **Button:** a separate printed push-cap, Ø9 with a dished top, standing 3.5 mm proud. It slides in a Ø9.4 bore in the top wall. A Ø11 × 0.8 flange keeps it captive in a recess underneath, 0.1 mm above the plunger. Drop it in from inside before fitting the PCB. Nothing flexes.
- **Base:** the body sits straight on the desk at a 15° tilt, with a full-width wedge under the front. A curved cove at the back runs into a 3 mm lip that extends 22 mm back to stop it tipping. A 14 mm notch through the cove and lip gives the USB-C plug room, and the plug clears the desk by 2.4 mm. There are 4 recesses for Ø8 rubber feet, two under the front and two under the lip.

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
