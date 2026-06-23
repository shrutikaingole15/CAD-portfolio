# Project B — Multi-Feature Block with Fillets

**Software:** FreeCAD 1.1 — Part Design & Sketcher workbenches

A complex solid that chains multiple additive and subtractive Part Design operations in a single model tree. The goal is to stay parametric throughout — each feature references the previous one so the model rebuilds cleanly if dimensions change.

## Operations
| Step | Operation | Purpose |
|------|-----------|---------|
| 1–3 | Sketch + Pad (×3) | Build up the base geometry in stages |
| 4 | SubtractiveBox | Cut a rectangular void |
| 5 | Fillet | Round selected edges for manufacturability |
| 6 | SubtractiveCylinder | Drill a cylindrical hole |
| 7–8 | Pocket (×2) | Refine remaining features |

## Views
See the `images/` folder for orthographic and isometric views.


