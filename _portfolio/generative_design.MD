---
title: "Generative Design Skateboard Truck"
excerpt: "Lightweight generative design of a skateboard truck hanger with an integrated motor mount."
header: 
  image: /assets/img/FullSizeRender (2).jpeg
  teaser: /assets/img/FullSizeRender (5).jpeg
gallery:
  - image_path: assets/img/IMG_9310.jpeg
  - image_path: assets/img/Rendering2.png
  - image_path: assets/img/Rendering3.png
  - image_path: assets/img/Rendering4.png
  - image_path: assets/img/Rendering1.png
  - image_path: assets/img/Rendering5.png
  - image_path: assets/img/FullSizeRender (5).jpeg
  - image_path: assets/img/FullSizeRender.jpeg
  - image_path: assets/img/FullSizeRender (3).jpeg
  - image_path: assets/img/FullSizeRender (4).jpeg
  - image_path: assets/img/FullSizeRender (7).jpeg
  - image_path: assets/img/FullSizeRender 2.jpeg
  - image_path: assets/img/str (24 x 18 in) (9).gif
  - image_path: assets/img/str (24 x 18 in) (12).gif
  - image_path: assets/img/str (24 x 18 in) (10).gif
  - image_path: assets/img/str (24 x 18 in) (11).gif
---
## Powder Bed Fusion and Generative Design 
Generative design and powder bed fusion are changing how engineers approach design by making it easier to create parts that are both efficient and practical to manufacture. Generative design helps find the best shape for a part based on real-world loads and constraints, while powder bed fusion makes it possible to actually build those complex shapes. Together, they allow parts to be lighter and often combine multiple components into one, which simplifies assembly and improves overall performance—especially in aerospace and automotive applications where weight and efficiency matter most.


## Powder Bed Fusion and Generative Design impact on Automotives 
The combination of generative design and powder bed fusion is particularly effective in automotive engineering because it allows components to be redesigned for performance rather than manufacturability. Generative design identifies efficient load paths and removes unnecessary material, while powder bed fusion enables the production of complex geometries that cannot be made using traditional methods. This pairing not only reduces weight but also allows multiple parts in an assembly to be consolidated into a single component, improving structural efficiency and reducing manufacturing complexity.

A relevant example is presented by [Markovits and Szederkényi (2022)] (https://doi.org/10.1016/j.jmapro.2022.05.058), where a Formula Student race car suspension rocker was redesigned using generative design and produced with powder bed fusion. The original multi-part assembly was replaced with a single optimized component by defining key connection regions, applying realistic loading conditions, and using iterative generative design followed by validation with finite element analysis. The final design achieved approximately 40% weight reduction and significantly higher load capacity, demonstrating improved performance and reduced part count. This case highlights how generative design and additive manufacturing can simplify assemblies and enhance mechanical performance in real automotive applications (Markovits & Szederkényi, 2022
).
## Applying the Proper Load Cases
Applying proper load cases is essential in generative design because the final geometry depends entirely on the forces and constraints defined. Unrealistic or missing loads can lead to weak or overly heavy designs, while accurate loads ensure material is placed efficiently.

In this project, forces were selected based on real skateboard use conditions. A vertical load represents rider weight, torque at the motor mount simulates propulsion, and lateral forces account for turning. Additional loads, such as braking and impact forces, were included to capture more extreme scenarios. These were determined by analyzing how the skateboard is used in practice and estimating values using average rider mass and motor specifications. This process could be improved by using experimental measurements, dynamic simulations, or more detailed analytical calculations to better reflect real-world conditions.

## Comparing AlSi10Mg and 17-4 PH
The generative design results for AlSi10Mg and 17-4 PH stainless steel show clear differences due to their material properties. AlSi10Mg, being less dense, produces a lighter design but typically requires more material distribution to meet strength requirements, resulting in more complex and organic geometries. In contrast, 17-4 PH stainless steel has higher strength and stiffness, allowing the design to use less material in critical areas and appear more compact, though the overall part is often heavier due to its higher density. As a result, AlSi10Mg is better suited for applications where minimizing weight is the priority, while 17-4 PH is more appropriate when higher strength and stiffness are required.

## Critiques to Generative Design. 
Generative design is a useful tool for creating lightweight and efficient parts, especially when combined with additive manufacturing. It works well in industries like aerospace and automotive, where reducing weight and improving performance are important. It can also combine multiple parts into one, which simplifies designs and reduces assembly.

However, it has some drawbacks. The results depend heavily on the inputs, such as loads and constraints, so poor assumptions can lead to bad designs. The shapes it produces can also be very complex, making them harder to manufacture or use in practice. It also requires time, computing power, and engineering judgment to get good results.

Generative design is most useful for complex, high-performance parts where optimization matters. It is less useful for simple or mass-produced components, where traditional design methods are usually cheaper and more practical.

## Applied Forces 
| Force Name    | Magnitude                    | Location (Applied At) | Rationale                                                                 |
| ------------- | ---------------------------- | --------------------- | ------------------------------------------------------------------------- |
| Rider Load    | 800 N total (400 N per side) | Axle ends             | Represents rider weight distributed across both wheels with safety margin |
| Impact Load   | 1400 N (applied on one side) | Single axle end       | Simulates shock from terrain such as hitting a curb or landing            |
| Motor Torque  | 15 Nm                        | Motor shaft interface | Represents torque transmitted from motor through belt drive               |
| Braking Force | 300 N total (150 N per side) | Axle ends             | Simulates deceleration forces during braking                              |
| Lateral Load  | 300 N total (150 N per side) | Axle ends             | Represents forces generated during turning/carving                        |


<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028114c1df3092b30a034?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Stainless Steel 17-4 PH 

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811e34c6d7e6754b6fa?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Edited Stainless Steel 17-4 PH Model with Nylon 
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b6028115a5d8bca9ec784cd?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Assembly with Nylon 

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281156d5f3e5195d9289?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Skate Board GD Gallery" %}

# References 
[Markovits, T., & Szederkényi, B. (2022). Investigation of generative design for powder bed fusion technology in case of Formula Student race car components using Ti6Al4V alloy. Journal of Manufacturing Processes, 80, 220–231.](https://doi.org/10.1016/j.jmapro.2022.05.058)


