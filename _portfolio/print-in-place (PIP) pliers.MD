# Print-in-Place Pliers
---
title: "Print-in-Place Pliers"
excerpt: " Print-in-place models are functional multiple-component designs, that work immediately after removal from the print bed."
header:

  teaser: /assets/img/header_pliers.jpg

---
### Overview

This project showcases the design and fabrication of **print-in-place (PIP) pliers**, a single-step 3D-printed mechanism that functions immediately after printing — no assembly required. 

Print-in-place (PIP) designs represent one of the most creative uses of 3D printing. Instead of printing separate parts and assembling them later, PIP models integrate all components — hinges, springs, sliders — into one continuous structure. When printed correctly, the parts are free to move once the support material or bridging layers are broken away.

---

### Applications of Print-in-Place Design

Print-in-place mechanisms have been widely adopted in both functional and educational projects. A few examples include:

* **Hinged tools** such as adjustable wrenches, scissors, or clamps.
* **Living hinges and flexures** used in enclosures or folding mechanisms.
* **Articulated toys or models**, like snakes, chains, or robots with movable limbs.
* **Deployable structures** in aerospace or robotics, where compact parts unfold after printing.

External research shows that PIP techniques are valuable for **reducing post-processing time**, improving **assembly precision**, and enabling **rapid prototyping** of mechanisms that would otherwise require multiple parts and fasteners.

When it comes to materials, **PLA** and **PETG** are the most common choices due to their predictable print shrinkage and low warping. For applications needing flexibility or durability, **TPU** can also be used — especially in designs where compliant joints are integrated directly into the geometry.

---

### Embedded CAD Model

An interactive version of the CAD model can be viewed below:

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281138791c29f24582de?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

---

### Design and Iteration Process

The project began with a simple two-arm plier joined by a central pin. At first, the hinge offset was too large, so the two halves couldn’t fit together properly. I adjusted the hinge dimensions and printed several test versions with different offsets until I found one that assembled smoothly and allowed free movement.

A key innovation in this project is the **print-in-place spring** integrated between the handles. Instead of using a separate metal spring, a flexible arc-shaped section was modeled into the base of the handles. The geometry works like a leaf spring — when the handles are squeezed, the arc bends slightly and stores strain energy. Once released, it pushes the handles apart and returns the jaws to the open position.

Material-wise, the pliers were printed using **PLA** and **TPU** on a **Formlabs FDM printer**, chosen for its balance between rigidity and printability.

---

### Specifications

| Parameter | Value |
|------------|--------|
| Total Length | 160 mm |
| Jaw Length | 55 mm |
| Maximum Jaw Opening | 18 mm |
| Handle Width | 23 mm |
| Plier Height | 5 mm |
| capacity | 5 resistances in 30s |

These specifications were optimized to balance tool strength with print reliability, while ensuring all components remain functional post-print.

---

### Print Settings

| Setting | Value / Notes |
|----------|----------------|
| Nozzle Size | 0.4 mm |
| Vertical sheels perimeters | 2 minimum |
| Infill Density and pattern | 25% (Gyroid for sparse and monotonic for top infill) |
| Support Material | None (bridging design for clearance) |
| Material | PLA, TPU for flexible jaws |
| Print Time | ~ 3 hours |

---

### Picture Gallery

## Pliers
![Pliers Rotation](/assets/img/pliers_video.gif)
![Pliers](/assets/img/pliers.jpg)
## Iterations
![Iterations](/assets/img/iteration_pliers.jpg)
---

### Reflection

This project demonstrates how print-in-place design principles can transform traditional multi-part tools into single-print, functional mechanisms. Through iterative prototyping and tuning material parameters, the PIP pliers evolved from a static prototype to a fully operable tool that highlights the precision and creativity of additive manufacturing.

---

*Created by Letian Ren – CHBE 4200 Additive Manufacturing Project.*
