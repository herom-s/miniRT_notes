This is a collection of notes about the MiniRT project of 42 School

- ### What is needed?
  
  To understand the scope of this project, we must first break down what the subject demands from us. We are required to use [miniLibX](miniLibX.md) as the graphical front-end and the C programming language as our primary implementation language.
  
  The program takes a [rt file](rt%20file.md) as a command-line argument, which contains a structured description of a scene. Using a rendering technique known as [Ray tracing](Ray%20tracing.md), the program must process this file and output a computer-generated image that accurately represents the described scene.
  
  The renderer must support 3 basic geometric objects: [Plane](../Math/Plane.md), [Sphere](../Math/Sphere.md), and [Cylinder](../Math/Cylinder.md). Their intersections and insides must be handled correctly, and each object must respect its unique properties — such as the diameter for [Sphere](../Math/Sphere.md), and the width and height for [Cylinder](../Math/Cylinder.md). The program must also support [Translation](../Math/Translation.md) and [Rotation](../Math/Rotation.md) [Transformations](../Math/Transformations.md) applied to objects, lights, and cameras.
  
  Finally, lighting must be managed through the following components:
- [Ambient lighting](Ambient%20lighting.md) — a base level of light applied uniformly to the scene
- [Diffuse lighting](Diffuse%20lighting.md) — light that scatters based on the angle of a surface
- [Spot brightness](Spot%20brightness.md) — the intensity of a defined light source
- [Hard shadows](Hard%20shadows.md) — sharp, defined shadows cast when light is blocked by an object