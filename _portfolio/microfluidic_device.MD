---
title: "μFluidic Device"
excerpt: "Sorting particles by size using Pinch Flow Fractionation into different streams."
header: 
  image: /assets/img/PhoneCase-1.png
  teaser: /assets/img/PhoneCase-1.png
---

This microfludic device, created through VPP printing, allows particles to be sorted based on size due to Pinch Flow Fractionation (PFF). Due to detailed reisn printing, a mold of the device is created and then finalized with PDMS casting. As the particles flow into different streams based of fludic mechanics, the design is flexiable and scalable to fit various sized particles and different solutions. 

# Introduction
  Pinch flow fractionation, also know as PFF, is a technique used to separate particles, by size, which is useful for many different applications. It is a passive microfluidic technique, meaning it does not require external forces to separate particles.

  PFF works using a pinched section which is a narrow channel where a buffer flow will compress the particle stream, forcing the particles toward one side of the channel. Because particles have different sizes, larger particles cannot move as close to the wall as smaller particles. 

  When the flow enters the broader section, the particles follow different streamlines based on their positions in the pinched region, allowing them to exit through different outlets. These streamlines can be calculated to help predict particle trajectories. So, this process greatly relies on hydrodynamic flow and the geometry of the microfluidic device.

Although it was first introduced by Yamada in 2004, PFF is now applied in fields such as medicine, polymer science, and other industries. a major use of microfluidic devices is for blood analysis as different cell types (red and white cells) and biomarkers (circulating tumor cells, pathogens) can be applied to diagnose diseases (anemia, cancer, and more). 

With the use of PFF, these small blood cells are able to be tested without clogging or with extensive preparation compared to the traditional methods which can include centrifuging and filtering. Therefore, PFF, being more compact and quicker, would be able to handle low volume samples while maintaining efficiency without requiring external energy in this situation. 

# Design
## Design Process 
• Briefly list the most important steps for creating a μfluidic device with resin printing.
1. understanding the basic area and expectations of this project. Brainstorm, read, research. 
  since a template was given with set plan on the sizes and the device, these were constraints or things that would be accounted for during the design
the project was difficult to understand at first, with the need to refresh on fludic mechanics and terminology. Therefore, a lot of reserach was needed. Especially when looking for something in particular like a PFF design, many papers will not upfront will not explain all of the detail and even have missing parts so that the experiment cannot be done again in a replicate. This made it difficult to find a design that was unquie while having evidence of something similar working prior since equation have to be told to estimate the outlet height. 
2. 
## Design Approach 
• Did you choose a symmetric or asymmetric approach?
A symmetric approach was taken due to the difficulty of that the asymmetric design would be since there are other factors that need to be taken account for such as the flow rate, elevation of the device and more had the asymmetric approach been done. Also, with the symmetric design, it is more predictable to understand the flow of the particles and to calculate where they could end. 
##Outlet Boundaries 
• How did you decide where to place the outlet boundaries for small particles, large
particles, and buffer flow?
The inlet sizing was based on the original design of the model; however, it was decided that the length and area of the solution first and then from there, knowing that the design that wasnted to mirror based on this journal had other dimensions also the 3mm buffer to the edge, there was a need to scale the deign, so once these were determined. The outlet following (equation) helped with the vetical from the bottom of the design space while there needs to be a total of 11 mm between the centers of inlets and outlets. Therefore, the outlets adjusted so that the smaller particle outlet and the larger particle outlet is based on the predicted flow while shortening the samller one to have the required distance from each. For the buffer flow, the outlet is less important in where as long as there is the 11 mm distance, but it is better when the outlet is shorter and wider, so to the large particle one it is farther than 11 mm. 
## Imbalanced Flow 
• How did you attempt to solve the flow balancing problem discussed in the beginning of
this document?
The balance issue stems from (), therefore, with adjusting the channels widths and lengths based on what material is being separated. The particle channel for example would have to be large enough for either of them due to the requirement that the channel width restriction is not allowed to stop and separating the particles. The width of the pinch width affected the broad zone where it separates the particles. The larger to smaller at the outlets helps direct the flow towards outlets due to the fluid mechanics. Wanting laminar flow to allow the particles to passively move in the direction that they are suppose to is the key of PFF. However, since there is more of the bulk solution, the bulk is made to be shorter and wider in order to balance out the issues that could cause turbulent flow and rearranging the expectations. The larger particle channel is farther away to also balance the flow due to more time to blah blah. 
## Improvements to Iterated Design
o What would you change about your outlet geometry if you could iterate on this
design?
This design was based on the paper does by the person's name. However, the dimensions of the base that was used was longer than the one provided in class. since this was the case, the design had to be readjusted and calculated due to the given constraints. A possible change is to have a longer base if possible in order to replicate the design to its fullist potential. The efficient PFF does this with the piece within the area; however, without being able to previous test the fludic device, it was difficult to know whether the particles would follow the equations provided. With the experiment changing from what is mathematically proven, the changes could be detrimental to the design and restrict the large particles, change bulk. Once the edit of the extra effective material is changed to match the dimensions and with tests of the first, the next iteration based on that. 

# Discussion
• Why resin printing compared to other manufacturing techniques?
• How could your design be scaled up or modified to handle a wider range of particle
sizes?
• What factors set the lower limit on the particle size that can be separated with pinchflow fractionation?

# Multimedia
o Sketch showing critical dimensions of channels (hand drawn or from CAD)
o Picture of Testing setup (syringe pumps, device, etc.)
o Picture of the mold
o Picture of Plasma treating process (image supplied)
o Picture of casted device
o Embedded YouTube video of the device working.

# Interactive Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811ccc104ca4ac1f161?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Pliers Gallery" %}

# References 
[Ashrafizadeh, S. N., Zare, M., & Khatibi, M. (2025). A comprehensive review of pinch flow fractionation in microfluidics: From principles to practical applications. Chemical Engineering and Processing: Process Intensification, 208, 110087.] (https://doi.org/10.1016/j.cep.2024.110087)

[Torres‑Castro, K., Acuña‑Umaña, K., Lesser‑Rojas, L., & Reyes, D. R. (2023). Microfluidic blood separation: Key technologies and critical figures of merit. Micromachines, 14(11), 2117.] (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10672873/)
