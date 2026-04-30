---
title:  "Bike Phone Holder"
excerpt: "A rotating, detent-based phone holder designed using top-down modeling for secure mounting on bicycle handlebars."
header: 
  image: assets/img/Screenshot 2026-04-30 at 00.33.13.png/
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
  - image_path: assets/img/Screenshot 2026-04-21 at 16.49.49.png


---

This is a functional bike phone holder designed using a top-down modeling approach and 3D filament printing. The holder mounts securely to a given standard bicycle handlebars and allows for phone insertion and removal. The key component is the built-in detent mechanism allows the phone to go from portrait to landscape orientations with a clear “click,” which ensures stability during riding.

# Top-Down Modeling Approach

Top-down modeling is a design approach where an assembly is created first, and individual components are then modeled within the context of that assembly in a single design file. This method allows all parts to reference each other, making it easier to ensure proper fit and function between components.

In this project, the bike handlebars were modeled first and used as a fixed reference component anchored in place. Additional components, such as the mount that holds the detent mechanism and connects to the handlebars, were then designed in relation to this reference geometry. The ball bearing and phone backing were created as separate components to allow rotational movement between them. Adjustable parts were subsequently modeled based on the positions of the existing components. A phone model was also imported and positioned within the assembly to guide dimensions and angles. Top-down modeling was particularly helpful withrotating components and reduce assembly errors.

# Design Rationale

## Detent Mechanism

The detent mechanism was implemented using a spring-ball bearing system. A small compression spring and stainless steel ball are located underneath the rotating circular plate, which has extruded ball positions to allow engagement. The mating component contains three recessed pockets corresponding to portrait (0°), angled (45°), and landscape (90°) orientations. When the user rotates the phone, the ball compresses against the spring and snaps into the next recess, creating a distinct click.

This mechanism works effectively and produces a clear sound that demonstrates the phone can withstand forces and remain in position. It provides strong positional locking while still allowing manual rotation. Early prototypes used a smaller detent mechanism with a 4 mm stainless steel ball, which was not deep or strong enough to withstand the force of the phone. The design was updated to use an 8 mm ball, and the circular plate was increased in size to account for this. Earlier versions also had insufficient depth in the detent pockets, resulting in weak engagement. Increasing the pocket depth and slightly stiffening the spring improved performance significantly.

## Dimensional Adjustments for 3D Printing

A clearance of 1 mm was between the circular plate and the back of the part that attaches to the bike handle. There was also a need to consider the circular plate extrusion for the ball to ensure that there is enough material to keep the phone steady while in position. For the M3 bolts, the diameter of the holes was 3 mm, which could fit the necessary parts, but if the design were further iterated, it should be increased. This is especially important because filament printing can introduce issues such as the material melting or deviating from the original model, as well as supports that may be difficult to remove.

## Filament Printing 
Filament printing was chosed since it was the more accessible and cost-effective, especially for rapid prototyping. Since this also allows for quick iterations and testing, like the detent mechanism and phone mechanisms, filament printing was the most reasonable to get parts quickly but with sufficient mechanical properties. Also, print setting made it easier to adjust according to varying components compiled. 

## Materials and Printing 
3D filament printing was used for all components. The majority of the parts were printed in PLA since it is easy to printing, has good dimensional accuracy, and is suitability for rapid prototyping. However, the circular plate component was printed in ABS because it requires higher toughness and improved resistance to wear and repeated motion where the ball is interacting and needs to have click. ABS typically provides better durability under stress compared to PLA, so it more suitable for moving parts.

# Assembly
All support material is first removed from the printed parts, especially in the holes and cavities of the clamp and detent housing. The spring (10 mm) is then placed into the detent mechanism, followed by the 8 mm ball bearing. 

Then, using M3 bolts, the rotating parts to the detent mechanism is made by attaching the phone holder to the circular plate and support component. 

The central bolt is a longer M3 (20 mm) bolt, which is used to connect through the support backing and previously mentioned parts of the detent mechanism. But, the ball bearing remains properly seated during this step.

Once the clamp is installed, the fixed base is aligned and secured to the design. The rotating circular plate is then placed onto the base, ensuring that the spring-ball bearing is properly at the detent housing. But, the detent system should be tested at this stage to confirm a clear click at each position.

Next, the phone cradle is attached to the top of the rotating phone holder. This design provides sufficient holding force so that another side supports are not needed. M3 bolts, one short and one long, are screwed to the adjustable section and rotating assembly, respectively, tied by a spring mechanism maintain phone stability.

To attachment to the handlebar, use four M3 bolts along with nuts, which are used to secure a tight and even clamp around the handlebar. This connection allows smooth rotation between portrait and landscape orientations while maintaining alignment with the detent positions. The user can rotate the phone by applying a moderate twisting force until the detent clicks into place, securely locking the orientation.

# Interactive Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH90d2dQT28d5b602811345fc0dda0a795df?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

# Figures
{% include gallery caption="Device Gallery" %}

# References 
Autodesk. Top-down modeling vs. bottom-up modeling in Autodesk Fusion. Autodesk. https://www.autodesk.com/products/fusion-360/blog/top-down-modeling-vs-bottom-up-modeling-autodesk-fusion/

Kennedy, K. Top-down vs. bottom-up modeling assemblies. Product Design Online. https://productdesignonline.com/tips-and-tricks/top-down-vs-bottom-up-modeling-assemblies/
