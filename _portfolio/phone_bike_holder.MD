---
title:  "Bike Phone Holder"
excerpt: "A rotating, detent-based phone holder designed using top-down modeling for secure mounting on bicycle handlebars."
header: 
  image: /assets/img/IMG_0784.jpg
  teaser: /assets/img/IMG_0784.jpg
gallery:
  - image_path: assets/img/IMG_0757.jpg
  - image_path: assets/img/IMG_0758.jpg
  - image_path: assets/img/IMG_0762.jpg
  - image_path: assets/img/IMG_0763.jpg
  - image_path: assets/img/IMG_0783.jpg
  - image_path: assets/img/IMG_0784.jpg
  - image_path: assets/img/str (24 x 18 in) (1).gif
  - image_path: assets/img/str (24 x 18 in) (2).gif
  - image_path: assets/img/Screenshot 2026-04-21 at 15.33.21.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.33.43.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.35.05.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.35.46.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.36.08.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.36.47.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.37.11.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.37.49.png
  - image_path: assets/img/Screenshot 2026-04-21 at 15.39.39.png



---

This is a functional bike phone holder designed using a top-down modeling approach and 3D filament printing. The holder mounts securely to a given standard bicycle handlebars and allows for phone insertion and removal. K key component is the built-in detent mechanism allows the phone to go from portrait to landscape orientations with a clear “click,” which ensures stability during riding.

# Top-Down Modeling Approach

Top-down modeling was central to this project. Rather than designing individual parts independently, the entire assembly—including handlebars and phone geometry—was created first. The handlebars were modeled as a fixed reference component and anchored in place. A simplified phone model was then imported and positioned at a realistic viewing angle.

From this master layout, all components of the holder were designed in context. This included:

Handlebar clamp
Rotating base plate
Detent housing
Phone cradle arms

By projecting geometry from the handlebars and phone into component sketches, all parts maintained proper alignment and fit. This approach ensured that design changes—such as adjusting phone width or handlebar diameter—automatically propagated throughout the assembly.

Top-down modeling was particularly beneficial for the rotating interface, where precise concentric alignment between components was required. It also reduced assembly errors since all parts were designed in their final positions and assembled using as-built joints.

# Design Rationale

The design balances stability, adjustability, and manufacturability.

The clamp uses a split-ring design tightened with M5 fasteners and heat-set inserts. This allows secure attachment to handlebars while remaining removable.

The phone cradle uses flexible side arms that allow phones to snap in without tools. The geometry accommodates a range of phone widths by incorporating slight elastic deformation in the arms.

# Detent Mechanism

The detent mechanism was implemented using a spring-loaded ball bearing system. A small compression spring and steel ball are housed in the rotating plate. The mating component contains two recessed pockets corresponding to portrait (0°) and landscape (90°) orientations.

When the user rotates the phone, the ball compresses against the spring and snaps into the next recess, creating a distinct “click.”

This mechanism works effectively. It provides strong positional locking while still allowing manual rotation. Early prototypes had insufficient depth in the detent pockets, resulting in weak engagement. Increasing pocket depth and slightly stiffening the spring improved performance significantly.

# Dimensional Adjustments for 3D Printing

Several dimensional changes were necessary to account for FDM printing tolerances:

Clearances of 0.25 mm were added between rotating parts to prevent binding
Holes for M5 fasteners were oversized (~0.2 mm) for proper fit
The detent housing diameter was increased slightly to accommodate printer inaccuracies
Snap-fit arms were thickened to prevent layer-line failure



Multiple pictures of printed model – both standalone and in use
Writeup with
A description of top-down modeling and how it was leveraged in this assignment.
Rationale behind your design
Assembly instructions
Material choice


• What type of 3D printing did you use? Why?
▪ Brief Assembly/use instructions
in order to 
▪ Which printing technology and why did you use for each part?
3d filament printing with the majority of the print in PLA except the ball bearing component that is a wheel to be ABS because 

# Interactive Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811345fc0dda0a795df?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Figures
{% include gallery caption="Device Gallery" %}

# References 
Autodesk. Top-down modeling vs. bottom-up modeling in Autodesk Fusion. Autodesk. https://www.autodesk.com/products/fusion-360/blog/top-down-modeling-vs-bottom-up-modeling-autodesk-fusion/

Kennedy, K. Top-down vs. bottom-up modeling assemblies. Product Design Online. https://productdesignonline.com/tips-and-tricks/top-down-vs-bottom-up-modeling-assemblies/
