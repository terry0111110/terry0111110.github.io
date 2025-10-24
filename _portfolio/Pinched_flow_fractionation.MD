---
title: "Pinched flow fractionation"
excerpt: "Pinched flow fractionation (PFF) is a simple, biocompatible microfluidic technique for particle separation, well-suited for applications."
header:

  teaser: /assets/img/header.png

---

# GitHub Entry – μFluidic Device

* **Pinch Flow Fractionation (PFF) Principle**  
  Pinched flow fractionation (PFF) is a simple, biocompatible microfluidic technique for particle separation, well-suited for applications requiring easy design, ease of operation, and gentle sample handling.
A buffer flow squeezes the particle stream against one wall in a narrow region, and when the channel widens, the particles follow different streamlines based on their size, allowing them to exit through separate outlets.

* **Specific Application & Benefit**  
  It makes separation microplastics for water quality evaluation. Compared to traditional filters, PFF avoids clogging and does not rely on membranes or pressure drops. It separates particles continuously in a laminar flow, using only fluid dynamics. This makes it gentle, reusable, and suitable for handling fragile or irregular particles such as microplastics in water samples.

Fiedler, S., Gielen, F., & Sadr, R. (2022). Design advances in pinched flow fractionation for enhanced particle separation in microfluidics. Lab on a Chip, 22(10), 1805–1821. DOI: 10.1039/D5LC00497G


* **Design Approach**  
  Adopted an **asymmetric configuration**, where the buffer inlet has a higher flow rate, pushing the sample flow toward one wall for effective focusing.

* **Outlet Boundary Placement**  
  Outlet positions were aligned with calculated streamline bands (Y₀) for the 125–150 μm and 425–500 μm particle ranges. Based on the following calculation, \mathrm{Given:\ }w_p=0.6\ \mathrm{mm}, wb=40 mm
Y_0=\left(w_p-\frac{D}{2}\right)\frac{w_b}{w_p}=\left(0.6-\frac{D}{2}\right)\times\frac{40}{0.6}=\left(0.6-\frac{D}{2}\right)\times66.6
Small\ particles:125-150\mu m\left(0.125-0.150~\mathrm{mm}\right)
\ \ D\ =\ 0.125:\ \ Y_0\ =\ (0.6\ -\ 0.0625)\ \times66.67\ \approx35.83mm\ 
\ \ D\ =\ 0.150:\ \ Y_0\ =\ (0.6\ -\ 0.0750)\ \times66.67\ \approx35.00mm
\Rightarrow\mathrm{Small-particle\ outlet\ reference\ height:\ }35.0-35.8~\mathrm{mm}

Large\ particles:425-500\mu m\left(0.425-0.500\mathrm{mm}\right)
\ \ D\ =\ 0.425:\ Y_0\ =\ (0.6\ -\ 0.2125)\ \times66.67\ \approx25.83mm
\ \ D\ =\ 0.500:\ \ Y_0\ =\ (0.6\ -\ 0.2500)\ \times66.67\ \approx23.33mm
\Rightarrow\mathrm{Large-particle\ outlet\ reference\ height:\ }23.3-25.8~\mathrm{mm}


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
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281121cf20e91f2f3df4?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


