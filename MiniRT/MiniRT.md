This is a collection of notes about the MiniRT project of 42 School
### What is needed?

To understand the scope of this project, we must first break down what the subject demands from us. We are required to use [[miniLibX]] as the graphical front-end and the C programming language as our primary implementation language.

The program takes a [[rt file]] as a command-line argument, which contains a structured description of a scene. Using a rendering technique known as [[Ray tracing]], the program must process this file and output a computer-generated image that accurately represents the described scene.

The renderer must support 3 basic geometric objects: [[Plane]], [[Sphere]], and [[Cylinder]]. Their intersections and insides must be handled correctly, and each object must respect its unique properties — such as the diameter for [[Sphere]], and the width and height for [[Cylinder]]. The program must also support [[Translation]] and [[Rotation]] [[Transformations]] applied to objects, lights, and cameras.

Finally, lighting must be managed through the following components:

- [[Ambient lighting]] — a base level of light applied uniformly to the scene
- [[Diffuse lighting]] — light that scatters based on the angle of a surface
- [[Spot brightness]] — the intensity of a defined light source
- [[Hard shadows]] — sharp, defined shadows cast when light is blocked by an object


