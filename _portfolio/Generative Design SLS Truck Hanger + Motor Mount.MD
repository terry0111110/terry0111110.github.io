---
title: "Generative Design SLS Truck Hanger + Motor Mount"
excerpt: "This project focuses on designing a lightweight longboard truck hanger with an integrated motor mount using Autodesk Fusion 360’s generative design workflow and powder bed fusion constraints."

header:

  teaser: /assets/img/GD_header.png

---

### Introduction

This project explores the use of generative design to create a lightweight longboard truck hanger with an integrated motor mount. The design aims to reduce part count and material usage while preserving all critical mechanical interfaces. Multiple load cases and constraints were applied in Fusion 360 to ensure realistic structural behavior. The final outcomes compare Nylon 12 and AlSi10Mg to evaluate the trade-off between weight, stiffness, and deformation.

## Importance of Proper Load Case Definition in Generative Design

### Why Proper Load Cases Matter
Applying appropriate load cases is critical in generative design because the algorithm does not “understand” intent — it only responds to the loads and constraints provided. The resulting geometry is a direct consequence of how forces are applied and how the structure is constrained. Unrealistic or incomplete load cases can lead to designs that are either structurally inefficient or fail under real-world conditions.

### Determining Which Forces to Apply
The applied forces were identified by analyzing how the longboard truck and motor mount operate in real use. Instead of applying arbitrary loads, each force corresponds to a physical interaction:

- **Vertical loads** represent rider weight transferred through the deck to the truck during normal riding.
- **Lateral (side) loads** simulate turning maneuvers, where wheels generate side forces that introduce bending and torsion in the hanger.
- **Motor-related loads** include:
  - The motor’s gravitational load acting downward.
  - Belt tension forces acting tangentially at the motor pulley location.
  - Resulting moments caused by belt forces acting at an offset from the hanger centerline.

By mapping real mechanical interactions to simplified but representative loads, the model captures the dominant load paths without unnecessary complexity.

### Placement of Structural Constraints
Structural constraints were placed at interfaces where the truck is mechanically restricted by other components:

- **Axle interfaces** were constrained using pin-type constraints to allow rotation while preventing translation, reflecting how the axle supports the wheels.
- **Pivot and kingpin contact regions** were constrained to represent contact with bushings and the deck-mounted baseplate.

These constraints were applied only to preserve geometry, ensuring that functional interfaces remain unchanged while allowing the surrounding material to evolve.

### Effect of Constraint Placement on the Outcome
Constraint placement directly influences stiffness distribution and material flow in the generated design. Over-constraining the model would artificially stiffen the structure and suppress meaningful optimization, while under-constraining could lead to non-physical deformation modes. By placing constraints at realistic contact locations, the generative algorithm produces a geometry that efficiently transfers loads between wheels, motor, and deck, resulting in a structurally sound and manufacturable design.

### Improving the Load Case Definition Process
The load case definition process can be improved by:
- Separating different riding scenarios into multiple load cases (e.g., straight riding vs. turning).
- Using conservative but realistic load magnitudes instead of peak theoretical values.
- Validating load assumptions against physical intuition and simplified hand calculations.

This approach ensures that the generative design outcome is both optimized and representative of real-world performance.


## Generative Design and Powder Bed Fusion for Assembly Consolidation  
### Commercial Example: Bugatti Titanium Brake Caliper

A real commercial example of using generative design with powder bed fusion is the 
**Bugatti titanium brake caliper**, which was produced using laser powder bed fusion.

### Background
Conventional high-performance brake calipers are usually built from multiple machined 
aluminum or steel parts that are bolted together. While this approach works, it increases 
part count, assembly effort, and the number of potential failure points.

### Design Approach
Instead of modifying an existing design, generative design was used to define only the 
critical functional regions, such as mounting points, piston locations, and pad contact 
areas. The software then generated a geometry that efficiently carried braking loads while 
removing unnecessary material.

### Manufacturing and Results
The final design was printed as a **single titanium component** using powder bed fusion. 
This replaced a multi-part assembly with one continuous structure, eliminating fasteners 
and internal joints. The result was a lighter caliper with high stiffness and improved load 
transfer.

### Why This Matters
This example shows how generative design and powder bed fusion can be used to simplify 
mechanical assemblies. By combining multiple parts into a single printed component, 
manufacturers can reduce weight, improve structural performance, and simplify production, 
especially in high-performance automotive applications.

---

### Embedded CAD Model

An interactive version of the CAD model can be viewed below:  

It is made of aluminum (AlSi10Mg).
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811435715b47b7d609c?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
A rendering of the completed longboard assembly with the generative design
trucks.(AlSi10Mg)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811c4c46b86b57f9358?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
It is made of  Nylon 12.
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028111762e2d1921da00c?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
A rendering of the completed longboard assembly with the generative design
trucks.(Nylon 12)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811113278f7bcbcd161?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
---
## Comparison Between Aluminum and Nylon Outcomes

The aluminum and nylon generative design outcomes show clear differences in structural behavior, even though the overall geometry and volume are similar.

The aluminum (AlSi10Mg) design has a mass of 0.132 kg and exhibits very low deformation, with a maximum displacement of only 0.137 mm. The minimum safety factor is 16.7, which is far above the required limit of 2. This indicates that the aluminum outcome is significantly overdesigned in terms of strength and stiffness for the applied load cases.

In contrast, the Nylon 12 design is much lighter, with a mass of 0.05 kg, but experiences substantially higher deformation. The maximum displacement reaches 7.68 mm, and the minimum safety factor is reduced to 3.16. While this still satisfies the safety factor requirement, the increased flexibility reflects the much lower stiffness of nylon compared to aluminum.

Overall, the aluminum outcome prioritizes stiffness and structural rigidity, making it suitable for high-load or performance-critical applications. The nylon outcome favors weight reduction and compliance, which may be acceptable for prototyping or lower-load use cases but could be limited by deformation rather than strength.

### Picture Gallery

## Real-life picture
![Real-life picture](/assets/img/Assembled.png) 

## Working (GIF)
![Holder Rotating](/assets/img/GD.gif)


---

**Conclusion**

This project demonstrates how generative design can be used to create a structurally efficient longboard truck hanger while reducing part count and material usage. The comparison between Nylon 12 and AlSi10Mg highlights that material selection strongly affects stiffness and deformation, even when strength requirements are met. Overall, generative design is most effective when combined with realistic load cases and engineering judgment.
---

*Created by Letian Ren – CHBE 4200 Additive Manufacturing Project.*


