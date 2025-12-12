---
title: "Generative Design SLS Truck Hanger + Motor Mount"
excerpt: "This project focuses on designing a lightweight longboard truck hanger with an integrated motor mount using Autodesk Fusion 360’s generative design workflow and powder bed fusion constraints."

header:

  teaser: /assets/img/head_phone_bike_holder.png

---

### Introduction

This project focuses on designing and 3D printing a functional bike phone mount using a top-down CAD modeling approach. The goal was to create a holder that can be quickly attached to a bicycle handlebar, securely grip a smartphone, and rotate smoothly between portrait and landscape orientations using a detent mechanism—without requiring any tools during operation.

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
### Commercial Example: Bugatti Titanium Brake Caliper (Automotive)

A well-documented commercial example of combining **generative design** with **powder bed fusion (PBF)** for assembly consolidation is the **Bugatti titanium brake caliper**, developed in collaboration with additive manufacturing partners using laser powder bed fusion (LPBF).

### Background
Traditional high-performance automotive brake calipers are typically manufactured as multi-piece assemblies. These assemblies consist of several machined aluminum or steel components that must be bolted together, increasing part count, assembly time, and potential failure points.

### Role of Generative Design
Generative design was used to explore load paths within the caliper under braking conditions, including hydraulic pressure, clamping forces, and thermal loads. Instead of starting from an existing caliper geometry, the design process defined:
- Mounting interfaces
- Brake pad contact regions
- Hydraulic piston locations
- Required stiffness and strength constraints  

The algorithm generated an optimized geometry that efficiently transferred loads while eliminating unnecessary material.

### Application of Powder Bed Fusion
Laser powder bed fusion enabled the production of this complex, organic geometry in **titanium**, a material difficult to machine conventionally. The caliper was printed as a **single monolithic part**, replacing a multi-component assembly.

### Assembly Consolidation Benefits
- Reduction from multiple machined components to **one printed part**
- Elimination of fasteners and internal joints
- Improved structural stiffness due to continuous load paths
- Reduced mass while maintaining or improving braking performance

### Industrial Significance
This example demonstrates how the combination of generative design and powder bed fusion enables true **design-for-function**, allowing engineers to consolidate assemblies that were previously constrained by traditional manufacturing methods. The result is a lighter, stronger, and simpler component, particularly valuable in high-performance automotive applications.

---
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
### Embedded CAD Model

An interactive version of the CAD model can be viewed below:

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028117bb0e35a052504aa?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

---

### Picture Gallery

## Real-life picture
![Real-life picture](/assets/img/real%20picture.png)

## Bar Holder  
![Bar Holder](/assets/img/bar%20holder.png)

## Rotating Mechanism  
![Rotating Mechanism](/assets/img/Rotating%20mechanism.png)

## Phone Case Rendering  
![Phone Case](/assets/img/phone%20case.png)

## Cross-section View of Internal Rotation Mechanism  
![Cross-section](/assets/img/Cross-section%20view%20of%20internal%20rotation%20mechanism.png)  

## Additional Renderings  
![Rendering](/assets/img/rendering.png)

## Holder Rotating (GIF)
![Holder Rotating](/assets/img/holder%20rotating.gif)


---

## Conclusion

This project demonstrates how top-down modeling significantly improves design efficiency and assembly accuracy. By referencing real geometry (handlebar + phone), creating components in context, and using as-built joints, the final phone mount achieved excellent fit, mechanical reliability, and ergonomics. Material choices (PLA + TPU) ensured the mount is both rigid and phone-safe, providing a smooth and secure user experience.

---

*Created by Letian Ren – CHBE 4200 Additive Manufacturing Project.*


