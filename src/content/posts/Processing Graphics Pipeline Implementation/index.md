---
title: Processing Graphics Pipeline Implementation
published: 2026-01-13
description: ''
image: './cover.PNG'
tags: [Graphics]
category: 'University Project'
draft: false 
lang: 'en'
---

#### [Graphics Pipeline](https://github.com/rdotzlaw/University-Projects/blob/main/Computer%20Graphics/GraphicsPipeline)

Implementation of a 2D/3D graphics transformation pipline with the following features:
- A matrix stack containing transformation matrices: Model, Camera, Projection, and Viewport
- Functions to manipulate the matrix stack
- Functions to apply transformations to the matrix stack
- A basic 2D scene constructed using custom transformation functions
- A basic animated 3D scene that extrapolates the previous 2D implementation of the graphics pipeline to 3D



The following controls are used when running the code:
- `[`: Rotate Clockwise
- `]`: Rotate Counter-Clockwise
- `=`: Zoom in
- `-`: Zoom out
- `O`: Switch between the following orthographic projection modes
    - Indentity: Projection, Camera and Model matrices are all identity
    - Center600: Centered on `(0,0)` with the side boundaries in the range `[-300,300]`
    - TopRight600: Bottom left is `(0,0)`, top right is `(600,600)`
    - FlipX: Same as Center600, but flipped through the Y-Axis
    - Aspect: Uneven aspect ratio, X-Range is `(-300,300)`, Y-Range is `(-100,100)`
- `D`: Switch between the following display modes
    - Pattern: A multicolored grid pattern
    - Scene: A basic drawing made using the custom graphics pipeline and functions for rotation, translation, etc.
    - Shapes: An animated 3D scene featuring squares moving away from the camera utilizing orthographic projection.

Code written in `Processing`
