---
title: "Multiple Material Pliers " 
excerpt: "A functional pair of 3D printed pliers designed for gripping and reaching in tight spaces while using a combination of rigid and flexible parts."
header:
  image: /assets/img/Slide-3.png
  teaser: /assets/img/Slide-3.png 
gallery:
  - image_path: assets/img/Slide-3.png
  - image_path: assets/img/Slide-2.png
  - image_path: assets/img/Slide-4.png
   
---
A 3D-printed pair of unique needle nose pliers designed for grabbing smaller components such as resistors. The pliers consist of rigid PLA components, two handles and jaws each, and a flexible TPU center acting as a spring that allows the pliers to return to their original state once released. Instead of requiring additional parts to assemble the pliers, the design is based on a print-in-place mechanism that allows the five parts to be assembled without tools by pressing them into each other like puzzle pieces. 

## Print-In-Place Parts

**Print-In-Place parts** are 3D-printed assemblies that come off the printer already or nearly assembled and functional. This can include printing parts separately and putting them together later such as this case; however, there are built-in clearances that allow the parts to move after printing.

## Material Combinations
- PLA (rigid) + TPU (flexible) — easy to print, good for press-fit or compliant joints where you want some separability and a flexible spring element.

- PETG + TPU / ABS + TPU — stronger welds between rigid and flexible parts (useful when you want the flexible element to be a permanent bonded feature).

- Single-material print-in-place with geometry (e.g., PETG, PLA) — use careful clearances and compliant geometry (living hinges, flexure joints) when only one material is available.

- PETG/ABS + TPU tends to bond more permanently to TPU than PLA does — useful when you want a welded flexible feature instead of a removable press-fit.

- SLS (Nylon) or SLA (resin elastomers) provide tighter tolerances, isotropic strength, or powder support, which makes complex, fully articulated print-in-place parts more reliable at production scale.

**Other Applications of Print-in-Place Parts** 
- Adjustable wrenches
- Toys (i.e. snakes with moving segments) 
- Hinges
- Charger wrappers
- Gears


## Designing and the Iterative Process
### Materials used
A key point to these pliers are that they are made of multiple materials, allowing for both action and flexibility. 
- PLA was used for the handles and jaw tips due to its stiffness, dimensional stability, and ease of printing. 
- TPU was used for the central spring element because of its elasticity for smoother movements and resistance to fatigue, while enabling a self-returning motion. 

### Creating the Spring Component
The TPU spring is critical to the plier's design because as it used, it repeatedly gets worn down. A grid infill with no horizontal shells was used to increase flexibility, with the infill oriented parallel to the perimeters for consistent deformation. The spring geometry was iteratively refined by adjusting infill pattern and density to balance flexibility, durability, and jaw opening range.

### Retaining Parts in the Model
The pliers are assembled using interlocking, only pressing together features that require no additional tools, focusing on the use of the dovetail joints. The geometries were designed with tolerances in mind and tested through multiple iterations to allow easy hand assembly while maintaining secure retention. Parametric modeling in Fusion 360 was used to efficiently adjust dimensions between design iterations and achieve proper alignment and fit.


## Plier Specifications 
* Parts: 
* Maximum Jaw Opening: 
* Jaw length: 
* Jaw capacity: 

## Print Settings 

| Category | Setting | PLA – Tips & Handles | TPU – Center Piece |
|--------|--------|---------------------|--------------------|
| **Vertical Shells** | Perimeters | 3 | 4 |
|  | Wall Thickness (mm) | 0 | 0 |
| **Horizontal Shells** | Top & Bottom Solid Layers | 3 | 0 |
|  | Minimum Shell Thickness (mm) | 0.8 | 0 |
| **Infill** | Infill Pattern | Rectilinear | Grid |
|  | Top Infill Pattern | Monotonic | Monotonic |
|  | Infill Density (%) | 15 | 31 |
| **Quality** | Only One Perimeter on Top Surfaces | Enabled | Enabled |
| **Overhangs** | Overhang Detection | Enabled | Enabled |
| **Seam** | Seam Position | Corners | Corners |
| **Advanced** | Fuzzy Skin | Disabled | Disabled |
| **Supports** | Supports | Everywhere | Everywhere | 
| **Material** | Filament | PLA | TPU 95A |
| **Printer Setup** | Printer | Voron 300 | Voron 300 |
|  | Nozzle Diameter | 0.6 mm | 0.6 mm |

## Assembly & Operating Instructions
1. After printing is complete on the Voron 300 printers using the specified print settings, verify that all components are present: two PLA handles, two PLA jaw tips, and one TPU center spring.
2. Orient the TPU center so that it forms a diamond shape, which allows the flexible element to function as a spring.
3. Insert the PLA jaw tips into the appropriate cavities of the TPU center, ensuring that both tips are aligned symmetrically along the center so the jaws meet evenly and are capable of gripping small components.
4. Attach the PLA handles by pressing them into the remaining cavities, making sure the handles are oriented outward to provide a comfortable grip for the user and proper actuation of the pliers.
5. Once assembled, the flexibility of the TPU center allows the pliers to maintain their position. When no force is applied, the TPU spring returns the pliers to their default position.


# Interactive Fusion 360 Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b60281155c06b6c92d119f0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Pliers Gallery" %}

## References 

[Tom’s 3D Printing Filament Guide](https://toms3d.org/2024/12/06/try-these-filament-combinations-for-multi-material-and-supports/)

[Formlab's Guide to 3D Printing Materials: Types, Applications, and Properties](https://formlabs.com/blog/3d-printing-materials/?srsltid=AfmBOorgmIdkEi4M9s1keijOKeIPAqEbPcNzDKplmmMmlBabkTcFKH9h)

[Formlab's How to 3D Print Interlocking Parts and Assemblies](https://formlabs.com/blog/how-to-3d-print-interlocking-joints/?srsltid=AfmBOor_AacUit1dFaYq4Ng-rpGXmWWnX_Om8wYyvyozNJ-E8P7zEpGS)

