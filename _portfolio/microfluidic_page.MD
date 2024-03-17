---
title: "MicroFluidic device"
excerpt: "Designed a Resin Printed Microfluidic Mold to create a functioning microfluidic device."
header:
  teaser: assets/img/microfluidic_pic2.jpeg
gallery:
  - url: assets/img/microfluidic_pic2.jpeg
    image_path: assets/img/microfluidic_pic2.jpeg
    alt: "picture of finished microfluidic device"
  - url: assets/img/microfluidic_mold_and_device.jpeg
    image_path: assets/img/microfluidic_mold_and_device.jpeg
    alt: "picture of finished microfluidic device and mold"
---

### What are microfluidics and why use them?
  Microfluidic devices are devices that use a very small amount of some lab tests or operations. These devices are characterized by their small feature size and thus do not need the same volumes that are necessary for other devices. The device that I created was a microfluidic mixer, which has a variety of uses including DNA analysis, chemical synthesis and biosensor studies. For the example of DNA analysis, you may want to do an antibody test, but need to mix a certain liquid chemical with the small blood sample in order to get results. 

#### Challenges of microfludics
  There are two primary challenges to creating a microfludic device. The first is due to the nature of these pieces being so small. Microfluid devices as easily broken and thus a proper care must be taken to ensure the dimensioned selected in the CAD model will be printable and viable for the device. Secondly, due to the narrowness of the pathways, the liquids often do not mix as they travel down the paths. With a standard straight path, these liquids are so thinned and in such close proximity that the laminar flow and surface tension to their own material and path keeps the liquids from mixing, even when traveling side by side. To get proper mixing, obstacles must be introduced to overcome the liquid's low Reynolds number that the chamber size and liquid properties are inducing.

{% include gallery caption="Above are pictures of the device and the mold." %}


### Description of the Geometry
  A complex 3D path geometry was utulized in order to increase chaotic advection. The mixing path was split evenly into two sections along the length of the device. The first section employed a rectangular serpentine path to increase the path length that the fluid passed through. The path was a .2 mm extrusion from the mold base. An extruded cube rounded at two edges resembling a hump was patterned throughout the path. These features each had a height of .5 mm. And a cross-sectional area of .09 mm2. They were distanced .445 mm apart. This geometry was used in order to enhance chaotic advection by deliberately introducing obstacles and elongating the fluid path. This elongation of the path and introduction of complex, 3D geometry disrupts the natural laminar flow of the fluid, introducing initial perturbations and enhancing the mixing process.
  The second section is a spherical curving pattern to induce turbulent flow. This was done with a repeating half-cylinder with a width of .85 mm (diameter), thickness of .2mm, and extrusion of .7mm from the base. This path results in a volume of over 18mm^3 of space to mix due to its curving drops and snake-like path. There are areas of thin restriction that open into larger pooling areas which changes the direction of flow to be more random than straight paths, overcoming the laminar flow issues and separation that is normally seen. These obstacles induce circular flows in these pooling areas which then get reconstructed into the smaller paths. This process continues to repeat, inducing more and more mixing after each proceeding portion. The depth of these pooling areas was determined by the minimum feature size and aspect ratio that was able to be printed using the resin without risk of breaking or undeveloped parts. We also wanted to ensure the paths were as thin as possible to maintain proper pressure of the fluid through the path, require as little liquid as possible, and exaggerate the changes when it got to a larger pooling area.
  The reason a curving zigzag pattern was incorporated was to increase the time the liquid had to mix during the length of the device while maintaining plenty of space between rows to prevent resolution issues during casting. The more time the liquids are together going through these turns and drops, the more homogeneous the mixing of these two liquids can be by the end of the device. The curvature was important to ensure all liquid continued down the path, and didn’t get stuck at various points throughout the path, inducing unnecessary pressure, unwanted pooling, and dead zones in the device. Adequate spacing was ensured to ensure part development would not interfere with each other, and casting of the microfluidic would be successful.


## Autodesk Fusion 360 Model
#### (May take a couples seconds to load)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e12cd8210f025b9b8?mode=embed" width="1024" height="768" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Start to Finish of creating the Microfluidic Device
  The first step of creating a microfluidic device is creating the mold in which the device will be cast. As mentioned in the description of the Geometries, the process of ensuring proper mixing of the liquids throughout the length of the device is not a trivial task. Proper steps should be taken to maximize the mixing done throughout the device and ensure no dead zones or overlapping occurs during the liquid run pattern. This is all developed through CAD modeling software, and when ready converted to a STL file. 
  This model can then be SLA printed using a high-temperature resin on a FormLabs 3 Resin printer. Upload the SLT file to PreForm and ensure the mold is perfectly flat. The SLA printer has a 25 µm minimum layer resolution and 80 µm x-y resolution. After the print has finished, examine the part and ensure no parts are missing from your mold. You can then post-process the resin mold with two 5-minute baths in IPA, and allow it to air dry for 30 minutes prior to curing. Ensure that there is no uncured resin visible on the part and that the part has a homogenous finish, blowing off any debris if necessary. Then cure for 10 seconds to ensure the print is completed and ready for casting.
  Once the mold was completed, it was coated with parylene-C. PDMS was poured into the mold and degassed for 30 minutes followed by a 3-hour, 80°C oven curing period. Glass coverslips were bonded using a plasma cleaner after demolding.


### Operation
  The operation of a microfluidic device (once created) is quite easy. A programmable syringe pump was set up to push a small amount of liquid at a constant rate through the microfluidic. These syringes were connected to tubes that inserted into the posts, and two more tubes were inserted into the post on the opposite side to collect the liquid into a jar. The pump was then started, and could visibly see the liquid race through the device. It was difficult to tease out exactly where mixing was occurring, but mixing was evident by the color of the liquid in the exit tubes being a very mixed red-green color.


[![assets/img/microfluidic_model_in_holder.jpeg](assets/img/microfluidic_model_in_holder.jpeg)](https://youtube.com/shorts/tdT8q8riBro?feature=share)

