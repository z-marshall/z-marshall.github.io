---
title: "Generative Design Skateboard Truck"
excerpt: "Utilized Fusion 360 Generative Design software to create an weight and strength optimize skateboard truck"
header:
  teaser: assets/img/CAD powder print trucks.png
gallery:
  - url: assets/img/CAD powder print trucks.png
    image_path: assets/img/CAD powder print trucks.png
    alt: "picture of generative design CAD powder print truck"
  - url: assets/img/assembly img 1.png
    image_path: assets/img/assembly img 1.png
    alt: "picture of truck on assembly view 1"
  - url: assets/img/assembly img 2.png
    image_path: assets/img/assembly img 2.png
    alt: "picture of truck on assembly view 2"
  - url: assets/img/on skateboard pic 1.png
    image_path: assets/img/on skateboard pic 1.png
    alt: "picture of printed truck on skateboard"
  - url: assets/img/on skateboard pic 2.png
    image_path: assets/img/on skateboard pic 2.png
    alt: "picture of printed truck on skateboard view 2"
---
{% include gallery caption="Generative Design Skateboard truck" %}

### What is Generative Design and the benefits of pSLS
Generative design is a modeling optimization tool that specializes in making complex geometries for the most efficient and lightweight part of a given application. It's often difficult to estimate how the part will withstand its various applications, so the ability to incorporate its use into the design process is unique and a valuable aspect of the generative design process. The design can, in real-time, adjust to expected forces and add/subtract material based on its live-use predictions, which can save money, time, and materials by not having to print multiple iterations of the device and do repeated failure testing.

These geometries can be very intricate with difficult overhangs, curves, and edges that can't be conserved with other types of printing. This print was made using pSLS (powder selective laser sintering) 3D printing technology. Powder printing uses layer-by-layer fusing of fine powder pieces to create parts without the need for adherent support materials or limited complexity. This allows for excellent resolution and allows for the intricacy of the design to be maintained. In addition, the uniformity of the powder print allows for predictable part properties that ensure uniform part density and strength throughout the part. This ensures our prints correlate well with the predicted mechanical properties of the generative design as opposed to a filament-printed design which has drastically different mechanical properties based on how the forces are applied (between layers melting adhesion forces which is a weak plane vs along the strong plane where the plastic monomer chains take the force).

## Autodesk Fusion 360 Model
#### (May take a couples seconds to load)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6edb509cd53aceeedb?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

Generative design of powder printed Nylon 12 (FormLabs) skateboard truck

### Drawbacks
One of the drawbacks of generative design is the significant time it takes to create all the obstacle geometries, forces, and specifications necessary for the generative design to properly create the intended geometry. Generative Design is excellent at finding the one area that you meant to restrict, or slightly over-extrude into an obstacle geometry, so it is a significant learning curve of anticipating what the software will create, and adjusting your design accordingly. To ensure the generative outcome is what you are envisioning, multiple iterations are necessary which contributes to its significant time requirement. A study can anywhere from 1-12 hours to complete with extended time for extremely intricate designs and multiple manufacturing requirements or design type. 

For most applications (especially for hobbyist designs and applications) a generative design model would not be beneficial, because the required time and iterating in the generative design workspace is not worth the cost of materials or testing. For this particular truck, if I had a preconceived notion about the expected shape of the truck and the amount of material at certain portions to combat the moment, tension, and shear forces, I could have designed a first iteration model and printed it with a filament printer to ensure proper fits and dimensions in the time that it took be to get one generative design and no test fitting. This design underwent 6 iterations for various forces, tolerances, and fit iterations, whereas filament printing this design 2-3 times would have resulted in similar geometries and fits in roughly a quarter of the time. While the mechanical properties may have a better result with generative design, it heavily relies on extremely accurate estimations and positions of forces to create its geometries. If these forces are misplaced or insufficient, one may not know until moved to a simulation software or completely printed. This would undo the benefit of generative design by having to reprint and redo the insufficient forces. 

Finally, one of the major benefits of making the design as lightweight as possible is not necessary for most regular applications. Whether this skateboard truck was 35 grams or 33 grams was not going to make a significant impact on the usability of this design. However generative design still spends significant time calculating whether the truck can still perform optimally at 33 grams. While this may be crucial for a rocket piece where launching an extra kilogram of material into space can cost thousands of dollars extra, my skateboard is not going to perform noticeably differently with an extra 2 grams of weight.

### When it's useful
Though it takes a significant amount of work, time, and detail to ensure a model is accurately constructed, generative design is a master at optimization and customization. For applications where cost, weight, material used, and mechanical properties are critical, generative design can account for all these factors within one design, which many human-generated designs may not be able to. As mentioned earlier, aerospace is one arena that could benefit from the critical mass-minimizing features of generative design. Every gram matters and the parts need to be as strong as possible. Generative design goes through the painstaking process of shedding as much weight as possible and can iterate through various materials to give the best strength-to-mass ratio for a given part.

Automotive is another sphere where weight and strength are valuable. The more mass, the more force is required to obtain the same acceleration. This is critical for spheres like F1, NASCAR, and Supercross. But more important than minimized mass for speed and acceleration, is the safety of the driver. These components need to be strong in order to allow the driver to survive crashes at these high-speed events. This can be factored into the design with proper force attribution to simulate some of the forces of an impact. Finally, in both of these industries, these parts are extremely expensive to manufacture. Many of these parts are custom and could be thousands to hundreds of thousands of dollars to manufacture one iteration. This is not something you can manufacture multiple times so every small detail must be attributed to the first iteration, and generative design is a great way to ensure that everything gets accounted for.


## Autodesk Fusion 360 Model
#### (May take a couples seconds to load)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e6d3acaaba43fa452?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

Generative design of Aluminum AlSi10Mg skateboard truck

