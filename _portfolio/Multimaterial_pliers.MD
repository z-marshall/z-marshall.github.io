---
title: "Multimaterial Pliers"
excerpt: "Design movable pliers using multiple materials."
header:
  teaser: /assets/img/pliers_holding_hairtie.jpg
gallery:
  - url: /assets/img/pliers_at_rest.jpg
    image_path: assets/img/pliers_at_rest.jpg
    alt: "picture of finished, usable pliers"
  - url: /assets/img/pliers_holding_hairtie.jpg
    image_path: assets/img/pliers_holding_hairtie.jpg
    alt: "picture of finished pliers in use"
---
{% include gallery caption="Finished MultiMaterial Pliers." %}

### What is a multmaterial extrusion project and why use multiextrusion?
If we can think it, we’re going to want to be able to print it. But not everything that we think of is going to be made of one material, with one mechanical property, and one simple component. Oftentimes, to create anything of use, there are multiple components with varying properties that all coalesce to create something much more than their individual pieces could ever be. This project is no different, as a pair of pliers requires moveable components that retain their shape after compression. 

The goal of this project was to design and print needle nose pliers that had the utility and range of motion of standard pliers. This includes the ability to pick things up, close when pressure is applied, and return to their naturally open resting state after use.  With these requirements, we turn to a multimaterial part. In order to have secure jaws for holding and handles for holding and squeezing we need a rigid material like PLA. For a flexible pressure converting piece to allow for movable components when pressure is applied, we will be using a 95A TPU flexible center. 

So how do we create a multimaterial part? One of the best ways is to use a multiextruding printer like a MakerGear. This printer utilizes two print heads each with a different material, that can switch off printing per layer. While there are some drawbacks with this method like increased material used do to having a wipe tower and increased time per print, the variety of parts you now can print are increased dramatically. This allows us to experiment with various combinations of materials, applications, and properties that would have been impossible with just one material.

Often times the most useful combinations of materials are opposing mechanical properties. Like for the project, we are using a rigid and elastic component to get the most out of the usefulness of the pliers. Other more robust combinations include strong structural components like igumid P150 with a smooth flexible component like TPU (1). For best adhesion and mechanical aspects at the joints, you want to use similar materials in order to get best fusion between the materials. These similar properties include similar melting temperatures, flexibility, and polymer composition (1).

One of the most useful applications of multimaterial printers and 3D printers, in general, is the ability to print in place. This means the part is preassembled and ready to go off the print bed. There are multiple uses of this including moveable joints and actuators. An example of this is a print-in-place spring-loaded box, which allows for these pieces to intertwine during printing, which would not have been possible to assembly with this model post printing (2). An extension of this is using multiple materials over multiple components. These components can be printed such that they are mechanically intertwined, which can dramatically increase mechanical strength at the seems, and allow for seamless integration between materials.
 

(1)	https://blog.igus.eu/design-tips-multi-material-parts-from-the-3d-printer/

(2) https://www.instructables.com/Print-in-Place-Spring-Loaded-Box/



### About this design and specifications
 The original design utilized pegs on the four connecting joints of the pliers to secure the PLA/ridged material to the TPU/flexible material. Both handles and jaws each had a peg and a cutout for the flexible centerpiece to slide into to have a mechanical securing point between the two materials. A TPU flexible center was used as the center of the pliers to be able to effectively transfer the pressure applied to the handles to the jaws of the pliers. The spring component was used as the connection piece between the four ridged components and was created as a solid body in Fusion360, but then adjusted for flexibility in the SuperSlicer gcode set up. This will be covered in depth in the Printer Settings and Specification section.
 
This design underwent two major iterations. The primary issues with the original design was that the infill selected was not enough, thus the flexible component was not able to transfer the pressure from the handles through to the jaws properly and didn't close. This was compounded with too large of an angleon the flexible component, which did not properly transfer the pressure to the other end of the pliers. These issues were fixed in the next iteration be correcting the angle of the flexible component to be 90 degrees in order for the grid pattern to properly transfer pressure, and to increase the infill to be stronger and again transfer the pressure from the handles properly. The second issue was the clearances, as the original model was designed to be printed separately and then assembled afterward. This was fixed with the use of the MakerGear Multiextruder Printing in the following iteration, as all the parts were printed in place, with no assembly required.
![Book logo](/assets/img/iter1_rest.jpg)
![Book logo](/assets/img/iter1_closed.jpg)
First iteration pliers photos 


## Autodesk Fusion 360 Model
#### (May take a couples seconds to load)
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e71755eaf1d0103a4?mode=embed" width="800" height="600" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


### Print Settings and Specification
A great aspect of the SuperSlicer gcode creator is the ability to adjust infill densities and geometries in the SuperSlicer platform, rather than having to design it with particular infills and densities in the CAD model itself. This was utilized in this model for the flexible component, as the CAD model was a solid body, but in SuperSlicer, was adapted to have a grid infill of 25% density for best flexibility with the soft TPU material. All other infills and geometries were standard. 

  

## Video of Pliers in use
  <video src='https://youtube.com/shorts/qCgoobhTQss?feature=share' width=180/>

[![microfluidic device video](https://www.youtube.com/shorts/qCgoobhTQss)](https://www.youtube.com/shorts/qCgoobhTQss "microfluidic operating video")
