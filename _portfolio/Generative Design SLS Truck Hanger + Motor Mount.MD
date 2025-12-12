---
title: "Generative Design SLS Truck Hanger + Motor Mount"
excerpt: "This project focuses on designing a lightweight longboard truck hanger with an integrated motor mount using Autodesk Fusion 360’s generative design workflow and powder bed fusion constraints."

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
Bar Holder
Phone Case
Rotating mechanism
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

| Component          | Material | Printing Method | Reason                                                           |
|:------------------:|:--------:|:---------------:|------------------------------------------------------------------|
| Bar holder         | PLA      | FDM             | High stiffness needed to resist vibration; PLA holds screws well |
| Rotating mechanism | PLA      | FDM             | High dimensional accuracy for detent mechanism                   |
| Phone Case         | TPU      | FDM             | Flexible pads protect the phone and create friction grip         |



### Assembly/use instructions

1. Clamp Installation
Open the clamp and place it around the bike handlebar (25.4 mm). Tighten 3 M3 screws using a hex key during initial installation. After installation, no tools are required for operation.

2. Attach Rotating Plate
The rotating plate engages the bar holder through 4 M3 screws. Ensure the detent ball and spring are inserted before closing the housing.

3. Mount the Phone Case
Using a M3 screw connects the phone Case and the rotating plate. 

4. Using the phone bike holder
Push the phone to rotate between portrait ↔ landscape. Detent mechanism will click and hold the orientation. Holder stays stable under road vibrations.

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


