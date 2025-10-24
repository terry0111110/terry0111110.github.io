---
title: "Pinched flow fractionation"
excerpt: "Pinched flow fractionation (PFF) is a simple, biocompatible microfluidic technique for particle separation, well-suited for applications."
header:

  teaser: /assets/img/header.png

---

# GitHub Entry – μFluidic Device

* **Pinch Flow Fractionation (PFF) Principle**  
  A passive microfluidic method where a buffer flow pinches a particle stream into a narrow region.  
  When the channel widens, particles follow different streamlines based on size and exit through separate outlets.

* **Specific Application & Benefit**  
  Used to separate **microplastics in water samples**.  
  Compared to traditional filters, PFF provides continuous, gentle separation without clogging.  
  [Fiedler, Gielen & Sadr, *Lab on a Chip*, 2022, DOI:10.1039/D2LC00123A](https://doi.org/10.1039/D2LC00123A)

* **Design Approach**  
  Adopted an **asymmetric configuration**, where the buffer inlet has a higher flow rate, pushing the sample flow toward one wall for effective focusing.

* **Outlet Boundary Placement**  
  Outlet positions were aligned with calculated streamline bands (Y₀) for the 125–150 μm and 425–500 μm particle ranges.

* **Flow Balancing Strategy**  
  Adjusted each outlet’s hydraulic resistance \( R \propto \frac{L}{w\,h^3} \).  
  The buffer outlet was designed shorter and wider, while particle outlets were longer with equal width, achieving a flow ratio of **Qbf : Qsm : Qlg ≈ 5 : 2.5 : 2.5**.

* **Outlet Geometry Improvements (Iteration Plan)**  
  - Equalize outlet widths and control flow only by length (2 : 4 : 4 ratio).  
  - Add 3–5 mm straight settling zones before outlets.  
  - Use fillets (R = 0.5–1.0 mm) and ≥1.2 mm wall thickness to reduce shear and bubbles.  
  - Increase outlet spacing for cleaner separation and easier tubing.

* **Fabrication Steps (Resin Printing to Device)**  
  1. Design mold in Fusion 360 and export STL.  
  2. Print with resin 3D printer and post-cure.  
  3. Coat mold with parylene to prevent PDMS adhesion.  
  4. Pour and cure PDMS, then peel off.  
  5. Punch inlet/outlet holes and plasma-bond to glass.

* **Why Resin Printing**  
  Provides high-resolution, smooth surfaces for mi


# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a4f255f6522bb2efd0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>



