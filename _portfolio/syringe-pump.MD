---
title: "Syringe Pump " 
excerpt: "A low-cost 3D-printed syringe pump resulting in precise, adjustable flow with safety features and LED indicators."
header:
  image: /assets/img/Slide-3.png
  teaser: /assets/img/Slide-3.png 
gallery:
  - image_path: assets/img/Slide-3.png
  - image_path: assets/img/Slide-2.png
  - image_path: assets/img/Slide-4.png
   
---
This syringe pump is a low-cost, 3D-printed device designed to deliver precise and adjustable fluid flow for laboratory and prototyping applications. It uses a stepper motor and lead screw mechanism to convert rotational motion into linear displacement of a syringe plunger, allowing accurate control of flow rate. The design supports both 10 mL and 20 mL syringes and includes adjustable flow control, LED status indicators, and safety features such as a limit switch and enclosed electronics. 

## Key Features

* Adjustable and Precise Flow Control

The syringe pump allows users to set flow rates between 1 and 10 mL/min using either a potentiometer or values defined in the Arduino code. This provides both real-time manual control and repeatable programmed operation. The stepper motor and lead screw provide the motion for the syringe plunger's linear movement. 

* Compatible with Multiple Syringes

The design supports both 10 mL and 20 mL syringes without extra tools. Due to the custom 3D-printed end support, the syringes are secured and are able to be swapped quickly without changes to alignment and stability.

* Safety and Limit Protection

A limit switch automatically stops the pump when the syringe reaches the end or runs out of fluid. This prevents overdriving the motor and protects both the syringe and mechanical components. LED indicators provide visuals through colors: running (green), paused (yellow), and stopped (red).

* Manual Positioning Controls

Two momentary buttons allow the user to move the plunger forward or backward at high speed. This makes loading, unloading, and positioning the syringe quick and easy without manually turning the lead screw.

* Enclosed Electronic Components 

All electronics, including the Arduino, motor driver, and power supply, are inside a 3D printed enclosure. This prevents potential contact with wiring and protects components from liquid exposure, making the device safer and more reliable.

* Compact, Integrated Design

The motor, syringe holder, electronics, and control buttons are all built into a single unit. This makes the pump easy to transport and use without needing other external materials.

## Off-the-Shelf Parts

| Part           | Description               | Quantity |
|----------------|---------------------------|----------|
| Stepper Motor  | NEMA 17 stepper motor     | 1        |
| Stepper Driver | Motor driver module       | 1        |
| Arduino        | Arduino UNO microcontroller   | 1        |
| Power Supply   | 12V DC power supply       | 1        |
| Lead Screw     | 2 mm pitch lead screw     | 1        |
| Linear Rod     | Guide rod for carriage    | 1        |
| Linear Bearing | Bearing for carriage      | 1        |
| Syringes       | 10 mL and 20 mL           | 2        |
| Potentiometer  | Flow rate control         | 1        |
| Push Buttons   | Momentary + latching      | 2      |
| Limit Switch   | Switch      | 1        |
| LEDs           | Red, green, blue          | 3        |
| Breadboard     | Electronics mounting      | 1        |
| Jumper Wires   | Electrical connections    | Multiple        |

## 3D-Printed Parts

| Part               | Quantity | 
|:------------------|:--------|
| Enclosure          | 1     | 
| Enclosure Lid      | 1     |
| Syringe End Support| 1     | 
| Carriage           | 1     |      
| Motor Mount        | 1     |

# [Arduino Code](https://kathleenhartono.github.io/_pages/syringe-pump-arduino-code.md)

## Operating Instructions

1. Insert the syringe  
   Place a 10 mL or 20 mL syringe into the holder, ensuring both ends are supported.

2. Prepare the syringe  
   Fill the syringe with fluid and remove any air bubbles by gently tapping and pushing the plunger.

3. Power the system  
   Connect the 12V power supply to the Arduino and motor driver.

4. Upload Arduino code  
   Open the Arduino IDE, upload the syringe pump code, and restart the system.

5. Set flow rate  
   Adjust the desired flow rate using the potentiometer. The current flow rate will display in the Arduino Serial Monitor if enabled.

6. Start the pump  
   Press the start button. The green LED will light, indicating the pump is running.

7. Monitor the pump  
   - Press the pause button to temporarily stop the pump; the yellow LED will light.  
   - If the syringe becomes empty or the plunger reaches its limit, the limit switch stops the motor and the red LED will light. Refill or replace the syringe before restarting.

8. Manual adjustment  
   - Press the clockwise button to move the motor faster in the clockwise direction.  
   - Press the counterclockwise button to retract the plunger or adjust the syringe position.  

9. Power off  
   Turn off the power supply and disconnect the wall plug. Ensure all LEDs are off before disassembly or cleaning.

10. Remove syringe  
    Once powered off and stopped, remove the syringe safely.

# Interactive Fusion 360 Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a48d6c4dbd4ad21763?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Syringe Pump Gallery" %}
