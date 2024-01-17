---
title: "Programmable Syringe Pump"
excerpt: "Programmable Syringe Pump that can adapt to various flow rates and barrel size."
header:
  teaser: assets/img/syringe-pump-rendering.png
gallery:
  - url: assets/img/syringe-pump-rendering.png
    image_path: assets/img/syringe-pump-rendering.png
    alt: "rendering of Syringe Pump"
  - url: assets/img/syringe-pump-real-life.png
    image_path: assets/img/syringe-pump-real-life.png
    alt: "real image of syringe pump"
  - url: assets/img/circuit_diagram.png
    image_path: assets/img/circuit_diagram.png
    alt: "circuit diagram of electronics"
---

Syringe Pumps are a useful tool when dispensing liquids, especially in regard to accuracy when compared to a human hand. Their reliability and diversity have made them a staple in the medical industry, laboratories, and beyond. While basic applications can be done with a low-priced, one-speed pump with a specialized size syringe, pumps that can be adapted to various sizes and flow rates drastically increase in price when requiring these specifications. The goal of this design was to create an accurate, cost-effective, programmable pump that could effectively be introduced into a medical situation with ease. This includes adaptability to various sizes of syringe pumps and flow rates without the need for tools or alterations to the pump.

{% include gallery caption="Above is a rendered and real image of the pump, and a circuit diagram." %}

## Autodesk Fusion 360 Model
#### (May take a couples seconds to load)
<iframe src="https://myhub.autodesk360.com/ue2df3503/shares/public/SH56a43QTfd62c1cd96832754d64d89c2831?mode=embed" width="600" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>  
# Input my link from fusion in here

## Operation Instructions 
The syringe pump is easy and intuitive to use. Once the Arduino is programmed with its respective flow rate for the operation, the syringe barrel flange is inserted into its respective slot (5mL syringe in the protruding slot closest to the end of the pump, 20 mL syringe in the other slot). The barrel should be pressed down fully into the slot and feel very secure. The carriage is then manually maneuvered (by hand turning the screw) such that the plunger fits in the cutout of the carriage. The motor is plugged in and checked to ensure the syringe is ready for use (the LED should be yellow at this time). The syringe pump can now be started by pressing the on button (the LED will turn green). The pump will dispense a uniform amount of liquid until the syringe is empty, at which point the kill switch will be hit and the pump will stop (the LED will turn red).  At that point, the pump can be turned off and unplugged, and the syringe removed.


## Materials
### Off-the-Shelf Parts

| Quantity | Part name |
| ------------ |--------------|
| 1 | 250 mm lead screw with 2 mm pitch and 8 mm lead |
| 1 | 1/4" x 8mm Flexible Coupling |
| 2 | 200 mm linear rod with 8 mm diameter |
| 2 | LM8UU Linear bearing for 8 mm diameter rod |
| 1 | 2040 Aluminum Extrusion 1' Length |
| 1 | Nema 17 Stepper Motor |
| 1 | MEAN WELL RQ-65D AC-DC Power Supply Quad (Output 5V 12V 24V 12V 4 Amp) |
| 1 | Arduino Uno |
| 1 | A4988 Stepper Driver |
| 1 | Small Breadboard |
| 1 | Panel Mount Latching Push Buttons |
| 1 | Limit Switch |
| 1 | RGB Common Cathode LED |

### 3D printed Parts

| Quantity | Part name |
| ------------ |--------------|
| 1 | [Front of Barrel Stabilizer](https://github.com/z-marshall/z-marshall.github.io/blob/main/assets/drawings/Front%20of%20barrel%20stabilizer.png)  |
| 1 | [Back of Barrel Stabilizer](https://github.com/z-marshall/z-marshall.github.io/blob/main/assets/drawings/back%20of%20barrel%20stabilizer.png) |
| 2 | [Breadboard Fastener](https://github.com/z-marshall/z-marshall.github.io/blob/main/assets/drawings/breadboard%20fastener.png)  |
| 1 | [Carriage](https://github.com/z-marshall/z-marshall.github.io/blob/main/assets/drawings/carriage.png) |
| 1 | [Enclosure](https://github.com/z-marshall/z-marshall.github.io/blob/main/assets/drawings/enclosure.png) |
| 1 | [Lid](https://github.com/z-marshall/z-marshall.github.io/blob/main/assets/drawings/lid.png) |
| 1 | [Motor Mounting Plate](https://github.com/z-marshall/z-marshall.github.io/blob/main/assets/drawings/motor%20mounting%20plate.png) |


## Code
With all the aspects to this syringe pump, the code is what allows all of it to flow smoothly together. There are two switches and one LED indicator on the assembly, along with a motor whose flow rate and precision is determined by the code uploaded to the arduino. The code runs the pump once the start/stop button is pressed, and will stop when either the start/stop button is pressed again or when the syringe hits the second indicator on the barrel support to inform that the syringe is empty. When the syringe is paused (start/stop button is in the stop position), the LED indicator will shine yellow. When the pump is in motion, the LED indicator will shine green. When the barrel support switch is supressed (meaning that the barrel is empty), the LED will shine red.

You can view the [syringe pump code here](https://github.com/z-marshall/syringe_code/blob/main/syringe_pump_code.ino)
