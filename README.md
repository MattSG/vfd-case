# vfd-case

SolidCraft model of the VFD clock PCB, and the case built around it.

- `pcb.json`: a script that rebuilds the PCB reference model. It's the source of truth.
- `clock-pcb.sc`: the saved design. Open it in SolidCraft.

Rebuild: `solidcraft-cli run pcb.json --save clock-pcb.sc`

## Coordinates (mm)
- Z is up and the front (VFD side) faces −Y.
- The PCB's front face sits at y = 0.
- The PCB's bottom-left corner, seen from the front, is at the origin.

PCB 93.8 × 28.8 × 1.6. VFD 6.25 deep in front of the board. USB-C 10.65 deep behind it.
Total depth 18.5.

## Unverified
- PCB corner radius 1.75 (from the photo, it could be anywhere from about 1.2 to 2).
- How far the VFD pins stick out forward (set to 2.85).
- USB-C footprint 8.94 × 3.26 (the standard size, not measured).
