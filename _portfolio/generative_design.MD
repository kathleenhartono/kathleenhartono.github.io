---
title: "Generative Design Skateboard Truck"
excerpt: "Lightweight generative design of a skateboard truck hanger with an integrated motor mount."
header: 
  image: /assets/img/FullSizeRender (3).jpeg
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
Generative design are able to create the best shape for parts based on real world loads and constraints, and powder bed fusion actually makes it possible to build those complex shapes. Therefore, these methods are changing how designs can be approach design, making it easier to generate and optimized geometries with varying parameters based on what is targeted while being practical to physically manufacture. Usually, this combination allows parts to be lighter and combine multiple components into one. This makes assembly simpler and improves overall performance, especially in aerospace and automotive applications due to the importance of weight and efficiency matter most.

## Powder Bed Fusion and Generative Design impact on Automotives 
The combination of generative design and powder bed fusion is particularly effective in automotive engineering because it allows components to be redesigned for performance rather than how to actually manufacture the parts. With generative design identifing efficient load paths and removing unnecessary material and powder bed fusion printing complex geometries, which are harder to print than other traditional methods, the benefits like reduced weight, easier assembly, and structural efficiency align with many goals in the automotive industry. 

For example, [Markovits and Szederkényi (2022)] (https://doi.org/10.1016/j.jmapro.2022.05.058) discussed applying these methods to creating a Formula Student race car suspension rocker. It was redesigned using generative design and produced with powder bed fusion. The original multi-part assembly was replaced with a single optimized component by defining key connection regions, applying realistic loading conditions, and using iterative generative design followed by validation with finite element analysis. The final design achieved approximately 40% weight reduction per component and three times higher load capacity which improved performance and reduces the number of components in an assembly. 

## Applying the Proper Load Cases
Applying proper load cases is essential in generative design because the final geometry depends entirely on the forces and constraints defined. Unrealistic or missing loads can lead to weak or overlaying, heavy designs. With accurate loads, the material is expected to generate correctly and placed efficiently.

In this project, forces were selected based on real skateboard use conditions. A vertical load represents rider weight, torque at the motor mount simulates propulsion, and lateral forces account for turning. Additional loads, such as braking and impact forces, were included to capture more extreme scenarios. These were determined by analyzing how the skateboard is used in practice and estimating values using average rider mass and motor specifications. This process could be improved by using experimental measurements, dynamic simulations, or more detailed analytical calculations to better reflect real-world conditions.

## Comparing AlSi10Mg and 17-4 PH

The generative design results for AlSi10Mg and 17-4 PH stainless steel show clear differences due to their material properties. AlSi10Mg, being less dense, produces a lighter design but typically requires more material distribution to meet strength requirements, resulting in more complex and organic geometries. These designs often spread material along multiple load paths to compensate for lower strength.

In contrast, 17-4 PH stainless steel has higher strength and stiffness, allowing the design to use less material in critical areas and appear more compact. However, because it is denser, the overall component may still be heavier despite using less volume. This highlights the trade-off between strength and weight when selecting materials.

As a result, AlSi10Mg is better suited for applications where minimizing weight is the priority, such as aerospace or lightweight vehicles. On the other hand, 17-4 PH is more appropriate when higher strength, durability, and stiffness are required, even if it results in slightly higher mass. Material choice therefore plays a major role in determining the final geometry and performance of generative design outcomes.

## Critiques to Generative Design

Generative design is a useful tool for creating lightweight and efficient parts, especially when combined with additive manufacturing. It works well in industries like aerospace and automotive, where reducing weight and improving performance are important. It can also combine multiple parts into one, which simplifies designs, reduces assembly time, and can improve overall reliability.

However, it has some drawbacks. The results depend heavily on the inputs, such as loads and constraints, so poor assumptions can lead to bad or unrealistic designs. The shapes it produces can also be very complex, making them harder to manufacture, inspect, or integrate with other components. Even with additive manufacturing, there can be limitations related to print orientation, support structures, and post-processing requirements.

Generative design also requires significant computational resources and engineering judgment. It is not a fully automatic solution, as engineers still need to interpret results, verify performance, and make adjustments. In addition, for high-volume production, traditional manufacturing methods are often more cost-effective.

Generative design is most useful for complex, high-performance parts where optimization is critical and production volume is low to moderate. It is less beneficial for simple or standardized components where traditional design and manufacturing methods are faster, cheaper, and more practical. Overall, generative design is a powerful tool, but it is most effective when used alongside traditional engineering methods rather than as a complete replacement.

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


