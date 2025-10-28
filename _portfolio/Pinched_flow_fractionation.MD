---
title: "Pinched flow fractionation"
excerpt: "Pinched flow fractionation (PFF) is a simple, biocompatible microfluidic technique for particle separation, well-suited for applications."
header:

  teaser: /assets/img/header.png

---

# μFluidic Device Introduction

* **Pinch Flow Fractionation (PFF) Principle**  
  Pinched flow fractionation (PFF) is a simple, biocompatible microfluidic technique for particle separation, well-suited for applications requiring easy design, ease of operation, and gentle sample handling.
A buffer flow squeezes the particle stream against one wall in a narrow region, and when the channel widens, the particles follow different streamlines based on their size, allowing them to exit through separate outlets.

* **Specific Application & Benefit**  
  It makes separation microplastics for water quality evaluation. Compared to traditional filters, PFF avoids clogging and does not rely on membranes or pressure drops. It separates particles continuously in a laminar flow, using only fluid dynamics. This makes it gentle, reusable, and suitable for handling fragile or irregular particles such as microplastics in water samples.Fiedler, S., Gielen, F., & Sadr, R. (2022). Design advances in pinched flow fractionation for enhanced particle separation in microfluidics. Lab on a Chip, 22(10), 1805–1821. DOI: 10.1039/D5LC00497G

# μFluidic Device Design 
* **Design Approach**  
  Adopted an **asymmetric configuration**, where the buffer inlet has a higher flow rate, pushing the sample flow toward one wall for effective focusing.

* **Outlet Boundary Placement**  
  Outlet positions were aligned with calculated streamline bands (Y₀) for the 125–150 μm and 425–500 μm particle ranges. Based on the following calculation,
![Design process](/assets/img/design_process_1.jpg)

* **Flow Balancing Strategy**  
  Adjusted each outlet’s hydraulic resistance. Based on following equation,![Design process](/assets/img/design_process_2.jpg)
  The buffer outlet was designed shorter and wider, while particle outlets were longer with equal width, achieving a flow ratio of **Qbf : Qsm : Qlg ≈ 2 : 1 : 1**.

* **Outlet Geometry Improvements (Iteration Plan)**  
  - Equalize outlet widths and control flow only by length (1 : 2 : 2 ratio).  
  - Add gentle fillets at turns 
  - Increase outlet spacing for cleaner separation and easier tubing.

# μFluidic Device Design 
* **Fabrication Steps (Resin Printing to Device)**  
  1. Design mold in Fusion 360 and export STL.  
  2. Print with resin 3D printer and post-cure.  
  3. Coat mold with parylene to prevent PDMS adhesion.  
  4. Pour and cure PDMS, then peel off.  
  5. Punch inlet/outlet holes and plasma-bond to glass.

## Key size of mold
![Key size of mold](/assets/img/size_of_mold_2.jpg)

## Mold
![Mold](/assets/img/mold.jpg)

## Device
![Device](/assets/img/device.jpg)

## Plasma treating
![Plasma treating](/assets/img/Plasma-Treating-Image.jpg)










* **Why Resin Printing**  
  Resin printing was chosen because it provides high resolution and smooth surface finishes needed for micro-scale channels. 
  Besides,
  1.  Barrier against leachables & curing inhibition: Photopolymer resins release inhibitors that retard or prevent PDMS curing; a conformal Parylene-C coating blocks diffusion, avoiding inhibition. 
  2. Biocompatibility & stability: Parylene renders 3D prints more biocompatible, reduces absorption/toxicity, and protects the mold from solvents—extending mold lifetime.
  3. Lower surface energy and smoother coated surfaces improve PDMS release and channel quality.

* **Follow-up improvement**  
  I would choose interchangeable pinched widths w_p and add multiple outlet positions to target different bands in order to handle a wider range of particle sizes. Whether the particle will have laminar phenomenon or not set the lower limit on the particle size that can be separated with pinch flow fractionation. When particles become too small, diffusion dominates over laminar focusing, and they no longer follow stable streamlines.



# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281121cf20e91f2f3df4?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


