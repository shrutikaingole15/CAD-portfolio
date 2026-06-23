# Project A — Sketched Solid with Groove & Pocket

**Software:** FreeCAD 1.1 — Part Design & Sketcher workbenches

A solid part built from a fully constrained 2D sketch. The workflow uses Pad → Groove → Pocket to progressively add and remove material. A Datum Line serves as the axis reference for the Groove operation, keeping the model tree clean and rebuild-safe.

## Operations
| Step | Operation | Purpose |
|------|-----------|---------|
| 1 | Sketch + Pad | Base extrusion from 2D profile |
| 2 | Datum Line | Construction axis for the groove |
| 3 | Groove | Revolve-cut to remove material |
| 4 | Pocket | Final pocket cut |

## Views
See the `images/` folder for orthographic and isometric views.

**Source file:** `Exercise 2D -10_byHannu.fcstd`
