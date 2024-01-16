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

## Materials



## Code
With all the aspects to this syringe pump, the code is what allows all of it to flow smoothly together. There are two switches and one LED indicator on the assembly, along with a motor whose flow rate and precision is determined by the code uploaded to the arduino. The code runs the pump once the start/stop button is pressed, and will stop when either the start/stop button is pressed again or when the syringe hits the second indicator on the barrel support to inform that the syringe is empty. When the syringe is paused (start/stop button is in the stop position), the LED indicator will shine yellow. When the pump is in motion, the LED indicator will shine green. When the barrel support switch is supressed (meaning that the barrel is empty), the LED will shine red.

You can view the [syringe pump code here](https://github.com/z-marshall/syringe_code/blob/main/syringe_pump_code.ino)
