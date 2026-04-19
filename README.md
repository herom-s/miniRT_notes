# MiniRT Notes

A comprehensive collection of notes and documentation for the **MiniRT project** from 42 School — a ray tracing renderer implementation in C.

## Project Overview

MiniRT is a ray tracing project that requires:
- **Language**: C
- **Graphics Library**: miniLibX
- **Input**: Structured scene files (.rt format)
- **Output**: Computer-generated images

The program renders 3D scenes by parsing scene descriptions and applying advanced rendering techniques including ray tracing, transformations, and lighting calculations.

## Repository Structure

### 📐 Math/

Mathematical foundations and concepts essential to ray tracing and 3D graphics:

- **Core Concepts**: Vector, Matrix, Linear Algebra
- **Transformations**: Translation, Rotation, Transformations
- **Geometric Shapes**: Plane, Sphere, Cylinder, Conic sections, Quadric Surfaces
- **Mathematical Tools**: Polynomial, Quadratic equations, Homogeneous coordinates
- **Matrix Operations**: Matrix form, Symmetric matrix
- **Advanced Topics**: Euclidean Space, Surface equations

### 🎨 MiniRT/

Project-specific documentation for the ray tracing renderer:

- **Rendering Concepts**:
  - Ray tracing fundamentals
  - Rendering pipeline
  - Scene file format (.rt files)

- **Lighting Model**:
  - Ambient lighting — base uniform illumination
  - Diffuse lighting — angle-dependent surface scattering
  - Spot brightness — light source intensity
  - Hard shadows — occlusion shadows

- **Implementation Details**:
  - miniLibX graphics library integration

## Getting Started

These notes serve as:
- A reference guide for mathematical concepts
- Documentation of the ray tracing algorithm
- Implementation guidelines for the MiniRT project
- Quick lookup for specific topics

Navigate to specific folders based on what you need to understand:
- Start with `MiniRT/MiniRT.md` for project overview
- Refer to `Math/` folder for theoretical foundations
- Use `MiniRT/` for implementation details

## Notes

This is a study/reference repository. For the actual MiniRT implementation, visit the 42 School project repository.
