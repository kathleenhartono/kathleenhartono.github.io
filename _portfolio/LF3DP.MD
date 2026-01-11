---
title: "Syringe Pump"
excerpt: "A 1 kg/hr pellet extruder and 1 cubic meter build envelope for printing furniture."
header:
  image: /assets/img/LF3DP-Banner-2.jpg
  teaser: /assets/img/Large-Format-3D-Printer-Thumbnail.png
gallery:
  - image_path: assets/img/Slide-3.png
  - image_path: assets/img/Slide-2.png
  - image_path: assets/img/Slide-4.png
   
---
# * Syringe Pump *
This syringe pump is a low-cost, 3D-printed device designed to deliver precise and adjustable fluid flow for laboratory and prototyping applications. It uses a stepper motor and lead screw mechanism to convert rotational motion into linear displacement of a syringe plunger, allowing accurate control of flow rate. The design supports both 10 mL and 20 mL syringes and includes adjustable flow control, LED status indicators, and safety features such as a limit switch and enclosed electronics.

# Key Features

Adjustable and Precise Flow Control
The syringe pump allows users to set flow rates between 1 and 10 mL/min using either a potentiometer or values defined in the Arduino code. This provides both real-time manual control and repeatable programmed operation. The stepper motor and lead screw convert rotational motion into precise linear movement of the syringe plunger, ensuring consistent fluid delivery.

Multi-Syringe Compatibility
The design supports both 10 mL and 20 mL syringes without requiring tools. A custom 3D-printed end support securely holds syringes by their neck, allowing different syringe sizes to be swapped quickly while maintaining alignment and stability.

Safety and Limit Protection
A limit switch automatically stops the pump when the syringe reaches the end of its travel or runs out of fluid. This prevents over-driving the motor and protects both the syringe and mechanical components. LED indicators provide clear visual feedback for running (green), paused (yellow), and stopped (red) states.

Manual Positioning Controls
Two momentary buttons allow the user to move the plunger forward or backward at high speed. This makes loading, unloading, and positioning the syringe quick and easy without manually turning the lead screw.

Fully Enclosed Electronics
All electronics, including the Arduino, motor driver, and power supply, are housed inside a protective enclosure. This prevents accidental contact with wiring and protects components from liquid exposure, making the device safer and more reliable during use.

Compact, Integrated Design
The motor, syringe holder, electronics, and control buttons are all built into a single compact unit. This makes the pump easy to transport, operate, and deploy on a benchtop without needing external modules.

# Off-the-Shelf Parts
| Part | Description | Quantity |
|------|------------|----------|
| Stepper Motor | NEMA 17 stepper motor | 1 |
| Stepper Driver | Motor driver module | 1 |
| Arduino | Arduino microcontroller | 1 |
| Power Supply | 12V DC power supply | 1 |
| Lead Screw | 2 mm pitch lead screw | 1 |
| Linear Rod | Guide rod for carriage | 1 |
| Linear Bearing | Bearing for carriage | 1 |
| Syringes | 10 mL and 20 mL | 2 |
| Push Buttons | Momentary + latching buttons | 3 |
| Limit Switch | End-of-travel switch | 1 |
| Potentiometer | Flow rate control | 1 |
| LEDs | Red, green, blue | 3 |
| Breadboard | Electronics mounting | 1 |
| Jumper wires | Electrical connections | — |


# 3D-Printed Parts
| Part | Material | Fabrication Method |
|------|----------|-------------------|
| Enclosure | PLA | 3D printed |
| Enclosure Lid | PLA | 3D printed |
| Syringe End Support | PLA | 3D printed |
| Carriage | PLA | 3D printed |
| Plunger Holder | PLA | 3D printed |
| Motor Mount | PLA | 3D printed |

Link to Arduino Code


## Operating Instructions

1. Insert a 10 mL or 20 mL syringe into the holder and ensure both ends are supported.
2. Fill the syringe and remove air bubbles.
3. Power the system using the 12V power supply.
4. Upload the Arduino code and restart the system.
5. Set the desired flow rate using the potentiometer.
6. Press the start button to begin dispensing.
7. Use the pause button to stop the pump.
8. When the syringe is empty, the limit switch will stop the pump automatically.
9. Turn off power before removing the syringe.


# Interactive Fusion 360 Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a48d6c4dbd4ad21763?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Large Format 3D Printer Gallery" %}
