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
A symmetric approach was chosen because an asymmetric design would introduce additional variables that are difficult to control, such as differences in flow rate, device elevation, and outlet resistance. Since this would require more precise tuning to ensure proper separation as well as a symmetrical design being more predictable, which simplifies calculating where particles of different sizes will exit the device.
##Outlet Boundaries 
• How did you decide where to place the outlet boundaries for small particles, large
particles, and buffer flow?
The inlet sizing was based on the original design of the model; however, it was decided that the length and area of the solution first and then from there, knowing that the design that wasnted to mirror based on this journal had other dimensions also the 3mm buffer to the edge, there was a need to scale the deign, so once these were determined. The outlet following (equation) helped with the vetical from the bottom of the design space while there needs to be a total of 11 mm between the centers of inlets and outlets. Therefore, the outlets adjusted so that the smaller particle outlet and the larger particle outlet is based on the predicted flow while shortening the samller one to have the required distance from each. For the buffer flow, the outlet is less important in where as long as there is the 11 mm distance, but it is better when the outlet is shorter and wider, so to the large particle one it is farther than 11 mm. 
Since the overall device dimensions were set, both the inlet and the outlets fit the required design constraints, including the 3 mm buffer from the device edge and the 11 mm center-to-center spacing between inlets and outlets. Because the reference journal design used different dimensions, the device had to be scaled accordingly. were based on Vig, (Vig & Kristensen, 2008)in order to design the inlet, in relation to the paper, the distance between the inlets were limited by the fixed requirements however the angle at which they are inserted 82.9 degrees compared to the 39.9 degrees of the original model. This increase in the angle allows for the inlets to be farther away while this makes the distance that the solutions have to travel prior to mizing to the shorter, it ensures that it follows the design showocased in the research related to the enhanced PFF. 

Once the overall geometry was defined, the streamline equation yPFF = (wb/wp)rp. 
Here, wb is the width of broadening segment and wp is the
width of the pinch segment.
In this one-dimensional for PFF was used to determine the vertical outlet positions from the bottom of the design space. The outlets for the small and large particle streams were positioned based on the predicted particle streamlines after the broad section. The smaller particle outlet was slightly adjusted to maintain the required spacing between outlets. The buffer outlet was placed with less strict positional requirements, as long as it maintained the required spacing. However, it was designed to be shorter and wider to allow it to carry a larger portion of the total flow. This was scaled accordingly to figure 2 of the paper in order to scale for the size difference of the particles that were being using in the paper and the particles used in the assignment everything was scaled by half. yEPFF = 
RE
Rs
+ 1 dE
wp
rp.
## Imbalanced Flow 
The flow balancing issue occurs because the buffer stream carries a much larger portion of the total flow than the particle streams. To address this, the channel widths and lengths were adjusted to control the hydraulic resistance in each outlet. The particle outlet channels were made longer and narrower, which increases resistance and prevents excess buffer flow from diverting into those outlets.

The pinched channel width also affects how particles are distributed in the broad section, which influences the outlet positions. Maintaining laminar flow is critical in PFF because particles passively follow streamlines determined by their position in the pinched region. The buffer outlet was designed to be shorter and wider, allowing it to naturally carry more flow with lower resistance. Additionally, the large particle outlet was placed farther away, increasing the channel length and helping balance the flow distribution between outlets.
## Improvements to Iterated Design
This design was based on a previously published PFF device. However, the base dimensions of the device used in that paper were longer than the design space provided for this project, so the geometry had to be scaled and adjusted to meet the course constraints. If the design could be iterated, one improvement would be increasing the base length of the device so the original design proportions could be more closely replicated.

Additionally, because the device could not be tested prior to fabrication, it was difficult to confirm whether the particles would follow the predicted streamlines exactly. Experimental conditions can deviate from theoretical predictions due to factors such as flow instability or fabrication tolerances. After testing the first device, the next iteration could adjust outlet spacing, channel lengths, and outlet widths to better match the observed particle trajectories and improve separation efficiency.

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
Ashrafizadeh, S. N., Zare, M., & Khatibi, M. (2025). A comprehensive review of pinch flow fractionation in microfluidics: From principles to practical applications. Chemical Engineering and Processing: Process Intensification, 208, 110087.
https://doi.org/10.1016/j.cep.2024.110087

Torres-Castro, K., Acuña-Umaña, K., Lesser-Rojas, L., & Reyes, D. R. (2023). Microfluidic blood separation: Key technologies and critical figures of merit. Micromachines, 14(11), 2117.
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10672873/

Vig, A. L., & Kristensen, A. (2008). Separation enhancement in pinched flow fractionation. Applied Physics Letters, 93(20), 203507.
https://doi.org/10.1063/1.3028652
