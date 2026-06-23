# FreeCAD Mechanical Design Portfolio

A progressive set of mechanical and product design projects built in FreeCAD, moving from a single parametric part to a fully documented multi-part assembly with manufacturing-ready drawings. Each project emphasizes parametric modeling, clean design intent, and the kind of documentation expected in a professional engineering workflow.

> **What to look for in each project:** the model tree (parametric history), the sketch constraints, and the 2D technical drawing — not just the final render. These show *how* the part was built, which is what proves real mechanical design skill.

---

## Project 1 — Parametric Flange / End Cap

**Goal:** Master Part Design with spreadsheet-driven parameters. A bolt-hole flange where bolt count, bolt-circle diameter, and thickness are all driven from a spreadsheet, so changing one value rebuilds the whole part cleanly.

**Skills demonstrated:** sketching, geometric constraints, parametric model tree, design intent.

**References:**
- MangoJelly Solutions — "FreeCAD spreadsheet" tutorials (YouTube)
- Official FreeCAD wiki — Part Design tutorial

---

## Project 2 — Sheet-Metal Bracket

**Goal:** Learn the Sheet Metal workbench. An L- or U-bracket with proper bend radii, relief cuts, and an unfolded flat pattern — the form a manufacturer actually cuts and bends.

**Skills demonstrated:** manufacturability awareness, bends, flat patterns.

**References:**
- Search "FreeCAD sheet metal workbench tutorial" (MangoJelly)
- FreeCAD wiki — Sheet Metal workbench page

---

## Project 3 — Reverse-Engineered Real Part

**Goal:** Measure a real object (a caliper, hinge, or hose fitting) with a ruler/caliper and model it accurately. This mirrors real shop work and is highly relatable to hiring managers.

**Skills demonstrated:** measurement, tolerance thinking, working from physical objects.

**References:**
- GrabCAD — for comparison models
- Any caliper-measurement tutorial

---

## Project 4 — Multi-Part Assembly

**Goal:** Combine 3–5 parts into a working assembly with mating constraints — for example a small bench vise, a caster wheel, or a two-stage gear pair. Built with the Assembly workbench (native to FreeCAD 1.0+).

**Skills demonstrated:** assemblies, mates, interference checking, exploded views.

**References:**
- MangoJelly Solutions — FreeCAD 1.0 assembly series (dedicated playlist for the built-in assembly tools)

---

## Project 5 — Full Technical Drawing of the Assembly

**Goal:** Take Project 4 into the TechDraw workbench and produce a complete engineering drawing: orthographic views, a section view, an exploded isometric, full dimensions, tolerances, a bill of materials, and a title block.

**Skills demonstrated:** GD&T basics, drawing standards, technical communication — the piece that most separates a hobbyist portfolio from a professional one.

**References:**
- MangoJelly Solutions — TechDraw tutorials
- FreeCAD wiki — TechDraw workbench page

---

## Notes on Sequencing

Projects 1–3 are standalone parts that can be completed fairly quickly. Project 4 should reuse the good habits from the earlier work (spreadsheet parameters, clean sketches), and Project 5 depends entirely on Project 4 existing.

For a lean portfolio, Projects 3, 4, and 5 together tell the strongest story: *"I can measure something real, model it as a working assembly, and produce manufacturing-ready drawings."*

---

## Documentation Standard

For each project, include:
- A screenshot of the **model tree** alongside the final render
- The **2D technical drawing** (where applicable)
- A short writeup (2–3 sentences) covering the **design requirements** and the **key decisions** made

Hiring managers value seeing the reasoning behind a design as much as the model itself.

---

## Completed Projects

> All models below were built in **FreeCAD 1.1** using the Part Design and Sketcher workbenches. Each folder contains the `.fcstd` source file and orthographic view images.

---

### Project A — Sketched Solid with Groove & Pocket
**Folder:** [`01_sketched-solid/`](./01_sketched-solid/)

A solid part built from a 2D sketch using the Part Design workbench. The workflow begins with a constrained sketch that is extruded via **Pad**, then material is removed using a **Groove** (revolve-cut) and a **Pocket** operation. A **Datum Line** is used as a construction reference for the groove axis, demonstrating clean design intent rather than relying on geometry edges.

**Tools used:** Sketcher, Pad, Groove, Pocket, Datum Line
**File:** `Exercise A.fcstd`

---

### Project B — Multi-Feature Block with Fillets
**Folder:** [`02_multifeature-block/`](./02_multifeature-block/)

A more complex solid combining multiple additive and subtractive operations. The base is built up with sequential **Pad** operations, then shaped further using a **SubtractiveBox** and a **SubtractiveCylinder** to cut out material. **Fillet** edges are applied for realism and manufacturability. Additional **Pocket** features refine the final form. This part demonstrates the ability to manage a multi-step model tree without losing parametric control.

**Tools used:** Sketcher, Pad (×3), SubtractiveBox, SubtractiveCylinder, Fillet, Pocket (×2)
**File:** `Exercise B.fcstd`

---

### Project C — Revolved / Turned Part
**Folder:** [`03_revolved-part/`](./03_revolved-part/)

A rotationally symmetric part modelled using the **Revolution** tool — the FreeCAD equivalent of a lathe operation. A profile sketch is drawn on a plane and revolved 360° around an axis to produce the solid. A **Pocket** is then cut into the face to add an internal feature. This type of part is common in mechanical assemblies (shafts, caps, bushings) and this exercise focuses on clean sketch profiles and axis selection.

**Tools used:** Sketcher, Revolution, Pocket
**File:** Exercise C.fcstd`
