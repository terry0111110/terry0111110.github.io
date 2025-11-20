---
title: "Top-Down Modeled Bike Phone Mount"
excerpt: " This project focuses on designing and 3D printing a functional bike phone mount using a top-down CAD modeling approach."
header:

  teaser: /assets/img/head_phone_bike_holder.png

---

### Introduction

This project focuses on designing and 3D printing a functional bike phone mount using a top-down CAD modeling approach. The goal was to create a holder that can be quickly attached to a bicycle handlebar, securely grip a smartphone, and rotate smoothly between portrait and landscape orientations using a detent mechanism—without requiring any tools during operation.


---

### Top-Down Modeling Description & How It Was Used

Top-down modeling is a CAD strategy where the overall assembly context is defined first, and individual components are then created in place within that context. Instead of designing parts independently and later assembling them (bottom-up), top-down modeling begins with the final functional system layout. Top-down modeling ensured that any changes to the handlebar size, phone thickness, or rotation clearance automatically propagated to dependent components, reducing redesign work and improving consistency.

In this assignment, top-down modeling was leveraged in several important ways:

1. Modeling the handlebar first
I created a reference handlebar component using the exact diameter (22.2 mm or 25.4 mm). This component served as the fixed “ground truth” for the entire design.

2. Inserting the phone model early
A reference phone model was imported and positioned at a comfortable viewing angle. I used “Project” to bring its edges into sketches. This allowed me to dimension the clamp surfaces and clearance zones directly off the phone geometry.

3. Creating components in context
I used Fusion’s “Create Component” inside the main assembly to model:(There are some sub-components in a parent component.)
bearing ball, spring
Holder
Phone Case
Rotating Plate 
Each component’s sketches referenced existing geometry through projected edges and as-built joints, ensuring perfect alignment during assembly.

4. Using As-Built Joint for motion definition

Holder ↔ Handlebar: Rigid

Rotating Plate: Revolute

Phone case ↔ Rotation Plate: Rigid



## Design Rationale
### Rotation Mechanism & Detent Design

I selected a detent mechanism using an as-built joint. A ball-and-spring detent was integrated into the rotating plate to provide tactile “clicks” at 0° (portrait) and 90° (landscape).
The detent groove was shaped as a shallow U-profile to balance holding force and ease of snapping. This mechanism works effectively—the rotation feels smooth, and the phone locks positively at both viewing orientations.


### 3D Printing Dimension Adjustments
I change the design of detent mechanism, instead of rotating in X-Z plane, it rotates in X-Y plane. I also adjust the design of phone case in order to prevent screws from protruding and damaging the phone. And I also reprinted the rotator for better connection between phone case and rotator.

### printing technology 
All parts were printed using filament-based FDM due to: Fast iteration cycle,Low cost, Good dimensional accuracy, ability to mix materials (PLA + TPU) and strong interlayer adhesion on structural components.

The clamp and rotating plate benefit from PLA’s stiffness, while TPU enables comfortable, high-friction contact surfaces.
| Component          | Material | Printing Method | Reason                                                           |
| ------------------ | -------- | --------------- | ---------------------------------------------------------------- |
| Clamp              | PLA      | FDM             | High stiffness needed to resist vibration; PLA holds screws well |
| Rotating Plate     | PLA      | FDM             | High dimensional accuracy for detent mechanism                   |
| Detent Housing     | PLA      | FDM             | Rigid structure required for ball/spring interaction             |
| Phone Holder Body  | PLA      | FDM             | Solid structure; connects securely to rotating plate             |
| Phone Contact Pads | TPU      | FDM             | Flexible pads protect the phone and create friction grip         |




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

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028117bb0e35a052504aa?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
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

