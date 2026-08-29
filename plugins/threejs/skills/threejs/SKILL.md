---
name: threejs
description: Use Three.js for production-quality 3D graphics, animation, data visualization, cinematic scenes, and 3D visualizations. Use this skill when a task needs real 3D geometry, cameras, lighting, materials, particles, shaders, 3D charts, or Three.js integration with Remotion.
---

# Three.js Skill

Use Three.js to create production-quality 3D graphics and animations.

## Core principles

- Prefer official Three.js APIs and official addons.
- Build actual 3D geometry rather than fake or decorative 3D effects.
- Keep scenes visually clear and purposeful.
- Use proper cameras, lighting, materials, geometry, and animation.
- Keep numerical data accurate when creating charts or financial visualizations.
- Never replace requested data with a decorative grid or empty 3D scene.

## 3D data visualization

For charts and financial visualizations:

- Map data values explicitly to geometry.
- Use meaningful X, Y, and Z axes.
- Create visible bars, curves, points, or surfaces representing the actual data.
- Include readable labels and values when requested.
- Preserve proportions and numerical relationships.
- Use animation to reveal the data progressively.
- Use camera movement to emphasize important changes.

## Animation

- Prefer deterministic animation.
- Use frame/time-based animation when working with Remotion.
- Avoid animations that depend on uncontrolled real-time randomness.
- Make transitions smooth and intentional.
- Use easing where appropriate.

## Cinematic scenes

For cinematic 3D visuals:

- Establish a clear focal point.
- Use depth, perspective, lighting, and camera movement.
- Use materials and lighting to create visual hierarchy.
- Avoid unnecessary geometry.
- Use particles, glow, and effects only when they support the scene.

## Remotion integration

When Three.js is used with Remotion:

- Three.js is responsible for the 3D scene.
- Remotion is responsible for the video composition, timeline, and rendering.
- Make the Three.js animation deterministic and frame-accurate.
- Connect the current Remotion frame/time to the Three.js animation state.
- Design the scene so it renders consistently for every video frame.

## Recommended Three.js features

Use appropriate Three.js capabilities including:

- Scene
- PerspectiveCamera
- OrthographicCamera
- WebGLRenderer
- Mesh
- BufferGeometry
- Line
- Points
- MeshStandardMaterial
- MeshPhysicalMaterial
- Lights
- Groups
- InstancedMesh
- Text/3D labels where appropriate
- OrbitControls when interactive camera control is required
- GLTFLoader for 3D models
- Post-processing when visual effects require it

## Quality requirements

Before considering a scene complete:

1. Verify that the requested objects actually exist in the scene.
2. Verify that important objects are visible from the camera.
3. Verify that animation changes the intended objects.
4. Verify that data values map correctly to visual elements.
5. Verify that labels do not overlap important content.
6. Verify that the scene does not contain unnecessary empty space or decorative geometry replacing the requested visualization.
