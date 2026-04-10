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

  Although it was first introduced by [Yamada](https://pubs.acs.org/doi/10.1021/ac049863r)in 2004, PFF is now applied in fields such as medicine, polymer science, and other industries. a major use of microfluidic devices is for blood analysis as different cell types (red and white cells) and biomarkers (circulating tumor cells, pathogens) can be applied to diagnose diseases (anemia, cancer, and more). 

  With the use of PFF, these small blood cells are able to be tested without clogging or with extensive preparation compared to the traditional methods which can include centrifuging and filtering. Therefore, PFF, being more compact and quicker, would be able to handle low volume samples while maintaining efficiency without requiring external energy in this situation. 

# Design

## Design Approach 
  A symmetric approach was chosen because an asymmetric design would introduce additional variables that are difficult to control, such as differences in flow rate, device elevation, and outlet resistance. Since this would require more precise tuning to ensure proper separation as well as a symmetrical design being more predictable, which simplifies calculating where particles of different sizes will exit the device.

##Outlet Boundaries 
  Since the overall device dimensions were fixed, both the inlets and outlets were positioned to satisfy the required design constraints. The inlet geometry was inspired by the design presented by Vig and Kristensen (2008). However, because of the spacing limitations in the assignment model, the inlet angle was increased to approximately 82.9° compared to the 39.9° angle in the original design. Increasing this angle allowed the inlets to be positioned farther apart while still directing the streams toward the pinch region. Although this slightly shortened the distance the fluids travel before mixing, it preserved the key design features associated with enhanced PFF behavior described in the literature.

  Once the overall geometry was defined, the streamline relationship for pinch flow fractionation was used to determine the vertical outlet positions from the bottom of the design space:

y<sub>PFF</sub> = (w<sub>b</sub> / w<sub>p</sub>) r<sub>p</sub>

where w<sub>b</sub> is the width of the broad section, w<sub>p</sub> is the width of the pinched section, and r<sub>p</sub> represents the particle radius. This equation was used to estimate the expected particle streamlines after the flow expands into the broad section. The small-particle and large-particle outlets were positioned according to these predicted streamline locations, while the small-particle outlet was slightly adjusted to maintain the required spacing between outlets.

  The buffer outlet had less strict positional requirements as long as the 11 mm spacing constraint was satisfied. However, it was intentionally designed to be shorter and wider so that it would have lower hydraulic resistance and naturally carry a larger fraction of the total flow. The outlet locations were scaled based on Figure 2 from [Vig and Kristensen](https://backend.orbit.dtu.dk/ws/files/4832606/Asger.pdf)(2008) to account for the difference in particle sizes used in the reference study compared to those required in this assignment. 

  Since the particles used in this project were approximately half the size range used in the paper, the geometry was scaled accordingly using the enhanced PFF relationship based on figure 2a in [Vig and Kristensen](https://backend.orbit.dtu.dk/ws/files/4832606/Asger.pdf):

y<sub>EPFF</sub> = ((R<sub>E</sub> / R<sub>s</sub>) + 1)(d<sub>E</sub> / w<sub>p</sub>) r<sub>p</sub>
R<sub>E</sub> = Total hydraulic resistance of enhancing segment 
R<sub>s</sub> = Total hydraulic resistance of sink segment 
d<sub>E</sub> = Width of the wide section inside the enhancing segment 
w<sub>p</sub> = Width of the pinched section 
r<sub>p</sub> = Radius of particle 

  (R<sub>E</sub> / R<sub>s</sub>) was calculated from [Vig and Kristensen](https://backend.orbit.dtu.dk/ws/files/4832606/Asger.pdf) to be 2.14. This scaling, as well as extending the enhanced separator farther from the device's wall to ensure proper flow of the buffer and particle solution, allowed the outlet boundaries to better match the predicted particle trajectories for the particle sizes used in the experiment.

## Imbalanced Flow 
  The flow balancing issue occurs because the buffer stream carries a much larger portion of the total flow than the particle streams. To address this, the channel widths and lengths were adjusted to control the hydraulic resistance in each outlet. The particle outlet channels were made longer and narrower, which increases resistance and prevents excess buffer flow from diverting into those outlets.

  The pinched channel width also affects how particles are distributed in the broad section, which influences the outlet positions. Maintaining laminar flow is critical in PFF because particles passively follow streamlines determined by their position in the pinched region. The buffer outlet was designed to be shorter and wider, allowing it to naturally carry more flow with lower resistance. Additionally, the large particle outlet was placed farther away, increasing the channel length and helping balance the flow distribution between outlets.

  The calculated flow distribution for the three outlets is 61.5% for the buffer, 26.2% for the largest particle outlet, and 12.3% for the smallest particle outlet. This ensures the buffer carries most of the flow while the particle outlets receive enough to achieve proper separation.

## Improvements to Iterated Design
  This design was based on a previously published PFF device. However, the base dimensions of the device used in that paper were longer than the design space provided for this project, so the geometry had to be scaled and adjusted to meet the course constraints. If the design could be iterated, one improvement would be increasing the base length of the device so the original design proportions could be more closely replicated.

  Additionally, because the device could not be tested prior to fabrication, it was difficult to confirm whether the particles would follow the predicted streamlines exactly. Experimental conditions can deviate from theoretical predictions due to factors such as flow instability or fabrication tolerances. After testing the first device, the next iteration could adjust outlet spacing, channel lengths, and outlet widths to better match the observed particle trajectories and improve separation efficiency.

## Instructions
1. Understand the Project & Research
  The project began by defining goals and constraints, reviewing μfluidic principles, and conducting literature research, particularly on PFF designs. Missing details in papers required using equations and assumptions to estimate key parameters such as outlet height.
2. Design & Scale
  A design from the literature was sketched to match the provided mold/template and scaled using proportional ratios. Key features and potential functionality issues were considered.
3. CAD Modeling
  The sketch was converted into a 3D CAD model, optimized for resin printing by accounting for channel size, resolution, and support structures.
4. Printing & Post-Processing
  The device was printed once on a high-resolution resin printer. Supports were carefully removed, and the device was cleaned and post-cured to prevent blockages.
5. Testing & Evaluation
  Fluid flow and performance were evaluated, identifying design limitations despite producing only a single print.
6. PDMS Casting & Final Testing
  The resin print served as a mold to cast the device in PDMS, which was then sealed with glass and tested.

# Discussion
  Resin printing was chosen because it allows for high-resolution fabrication of small features, which is necessary for creating precise microfluidic channel geometries. Compared to techniques such as FDM printing or traditional machining, resin printing can produce smoother surfaces and finer details, which improves the quality of the PDMS mold and helps ensure proper bonding to the glass slide. Additionally, resin printing enables rapid prototyping, allowing multiple iterations of a design to be produced quickly and at relatively low cost.

  The design could be modified to handle a wider range of particle sizes by adjusting the width of the pinched section and the broad section of the channel. Since particle separation in PFF depends on the relationship between particle diameter and the pinch width, increasing or decreasing this width would shift the particle streamline positions. Another approach would be to add additional outlet channels, allowing more particle size ranges to be separated. The channel lengths and widths could also be adjusted to maintain proper flow resistance and streamline separation for different particle sizes.

  The lower limit of particle size that can be separated using PFF is mainly determined by the resolution of the fabricated microchannels and the surface roughness of the device. If the particles are smaller than the surface roughness of the channel walls, their trajectories become unpredictable and reliable separation becomes difficult. In addition, Brownian motion becomes more significant for very small particles, which can cause particles to deviate from their expected streamlines. Finally, the precision of the manufacturing process, such as the minimum feature size of the resin printer, limits how small the pinch channel can be fabricated and therefore limits the smallest particle sizes that can be effectively separated.

# Results of Enhanced PFF
  The result demonstrates an enhanced PFF (EPFF) device that improves particle separation through a snakelike structure in the broadening segment. It is noticeable that the particles are slightly lifted into the enhancing section, guiding the flow toward the particle outlets. The larger purple particles accelerate near the corner of the enhanced segment, allowing them to follow the streamlines closer to the enhancement rather than the device wall, directing them efficiently toward the large particle outlet.



# Multimedia
o Sketch showing critical dimensions of channels (hand drawn or from CAD)
o Picture of Testing setup (syringe pumps, device, etc.)
o Picture of the mold
o Picture of Plasma treating process (image supplied)
o Picture of casted device

[Full Youtube Video](https://youtu.be/pSMIe5w0k6k)

# Interactive Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811ccc104ca4ac1f161?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Pliers Gallery" %}

# References 
[Ashrafizadeh, S. N., Zare, M., & Khatibi, M. (2025). A comprehensive review of pinch flow fractionation in microfluidics: From principles to practical applications. Chemical Engineering and Processing: Process Intensification, 208, 110087.](https://doi.org/10.1016/j.cep.2024.110087)

[Torres-Castro, K., Acuña-Umaña, K., Lesser-Rojas, L., & Reyes, D. R. (2023). Microfluidic blood separation: Key technologies and critical figures of merit. Micromachines, 14(11), 2117.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10672873/)

[Vig, A. L., & Kristensen, A. (2008). Separation enhancement in pinched flow fractionation. Applied Physics Letters, 93(20), 203507.](https://backend.orbit.dtu.dk/ws/files/4832606/Asger.pdf)
