# LEVITRIX — Acoustic Levitator Enclosure

A black/yellow modular 3D-printable enclosure for a prototype 20-transducer acoustic levitator, designed around the Bambu Lab A1 mini and AMS Lite. Includes removable panels, curved upper/lower transducer carriers, and BlueNode Innovations branding.

## Project files

- `cad/` — editable CadQuery Python generator and STEP assembly for reference.
- `printing/STL_BLACK/` and `printing/STL_YELLOW/` — individual print parts.
- `printing/AMS_LITE_MULTICOLOR/` — two-color 3MF parts.
- `printing/FIT_TESTS/` — test pieces to verify dimensions before full printing.
- `docs/` — print manifest and build guidance.
- `branding/` — provided BlueNode logo artwork.

## Getting started

1. Print fit-test coupons before printing the enclosure.
2. In Bambu Studio, load **individual** STLs or matching multicolor 3MF files, not the assembled STEP as a print job.
3. Check component dimensions and fastener clearances against your actual purchased hardware.
4. Open `cad/LEVITRIX_V4_PLASTIC_ASSEMBLY.step` in FreeCAD to inspect the assembled geometry.
5. `cad/GENERATE_FIXED_STLS.py` is a **CadQuery** script; it requires a suitable Python environment with CadQuery and its other dependencies. It is not native FreeCAD Python.

## Status and safety

**Prototype / unverified physical fit.** Mesh integrity and nominal CAD clearances do not guarantee parts will snap in, fasteners will engage, or the assembly will function acoustically. Test the transducer, switch, DC jack and M3 heat-set inserts first. The unmarked ultrasonic transmitters' continuous-drive ratings have not been verified; do not connect a DRV8833 module directly to 12 V. Use a regulated current-limited supply and validate the electrical waveform before sustained operation.

## Branding

BlueNode Innovations artwork is supplied by the project owner. No third-party license is implied for the branding, CAD files, or other contents. If you plan to release your project publicly, decide on and add a suitable license after reviewing intellectual-property ownership.
