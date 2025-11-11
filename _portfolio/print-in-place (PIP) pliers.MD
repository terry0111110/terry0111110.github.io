# Print-in-Place Pliers

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

The design process started with a simple two-arm plier model joined by a central pin. The first iteration failed to move freely because the hinge clearance was too tight. Through several test prints, the joint gap was increased, and the hinge pin was slightly tapered to reduce surface fusion.

A key innovation in this project is the **print-in-place spring** integrated between the handles. Instead of using a separate metal spring, a flexible arc-shaped section was modeled into the base of the handles. This geometry stores elastic strain energy when squeezed, automatically returning the jaws to the open position.

Material-wise, the pliers were printed using **PLA** on a **Formlabs FDM printer**, chosen for its balance between rigidity and printability. The flexible spring section was oriented along the print’s layer direction to enhance bending durability. For more compliant motion, PETG or TPU can also be used in future iterations.

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
| Layer Height | 0.2 mm |
| Vertical sheels perimeters | 2 minimum |
| Infill Density and pattern | 25% (Gyroid for sparse and monotonic for top infill) |
| Support Material | None (bridging design for clearance) |
| Material | PLA, TPU for flexible jaws |
| Print Time | ~ 3 hours |

---

### Picture Gallery

Below are a few stages of the design and testing process.

| Iteration | Description | Image |
|------------|--------------|-------|
| **V1** | Initial prototype — hinge fused after print due to insufficient clearance. | ![](/assets/img/pliers_v1.jpg) |
| **V2** | Adjusted clearance and added spring geometry. | ![](/assets/img/pliers_v2.jpg) |
| **V3 (Final)** | Smooth hinge operation and reliable spring return. | ![](/assets/img/pliers_final.jpg) |

---

### Reflection

This project demonstrates how print-in-place design principles can transform traditional multi-part tools into single-print, functional mechanisms. Through iterative prototyping and tuning material parameters, the PIP pliers evolved from a static prototype to a fully operable tool that highlights the precision and creativity of additive manufacturing.

---

*Created by Letian Ren – CHBE 4200 Additive Manufacturing Project.*
