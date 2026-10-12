# LEVITRIX — corrected STL printing pack (Bambu Lab A1 mini + AMS Lite)

## What is inside

- `READY_SINGLE_COLOR_STL/`: 11 separate single-color parts, already oriented with the print bed at Z=0.
- `AMS_LITE_MULTICOLOR/`: four multipart 3MF groups (front panel, left frame, right frame, BlueNode badge). Import each as ONE multipart object in Bambu Studio, then assign black and yellow AMS slots.
- `PARTS_ORIGINAL_ASSEMBLY_POSITION/`: the same 21 plastic geometries as individually separate STL parts in assembled coordinates. For CAD inspection, not bed-oriented for printing.
- `FIT_TESTS/`: dimensional test pieces for transducer, heat-set insert, vertical rocker, DC jack/pot and LCD.
- `LEVITRIX_FIXED_ASSEMBLY_REFERENCE_ONLY.stl`: all plastic bodies concatenated in assembled positions, **reference only**. DO NOT slice as a one-piece print.
- `GENERATE_FIXED_STLS.py`: CadQuery source, for later parametric changes; unnecessary for printing the ready files.

## Changes made in this corrected edition

- Front switch centered at X = -60 mm and potentiometer at X = +60 mm, mirror symmetry around the central LCD.
- Rear DC jack centered at X = -60 mm and vertical switch at X = +60 mm.
- Relieved LCD retainer side rails so the nominal rear switch body no longer intersects it.
- No indicator LED cutout, no USB 5V output cutout.
- Retained two curved 10-transducer carriers with reinforced removable arch supports, both retainer plates, removable panels, traced BlueNode badge, and M3 insert locations.

## Checks completed

- All 21 source STL components reported watertight; each fits within the A1 mini 180 mm cube.
- 17 candidate CAD overlap tests yielded no unintended positive-volume overlap.
- Nominal collision envelopes for UNO, LCD, DRV8833, XL4015, 5V regulator, front/rear rocker, jack, and potentiometer did not intersect modeled structural plastic.

**These CAD checks cannot guarantee that unmeasured real hardware will fit.** The nominal rocker cutout is 13.2 x 19.2 mm (vertical). The nominal transducer can bore is Ø16.5 mm. The nominal M3 insert pilot is Ø4.2 mm. Print and physically test coupons first; adjust dimensioned CAD if the test fails. Check 3MF material assignments and slicer preview before printing. Electronic parts/transducers are intentionally absent from printable geometry. Screws, metal standoffs and inserts are not printable parts.
