# Image2ThreeJS Skill

Turn a reference image into a quality-gated, animation-ready procedural Three.js model built entirely in code.

## Best for
- Image-to-3D reconstruction
- Procedural Three.js props and objects
- Stylized character reconstruction
- Detail-accurate geometry and material studies
- Animation-ready `THREE.Group` hierarchies
- Visual self-correction through reference-vs-render comparison

## Workflow
1. Analyze the reference image before writing geometry.
2. Inventory macro, meso, and micro details, proportions, materials, and hidden/inferred regions.
3. Create a structured sculpt specification.
4. Generate the Three.js model in staged passes: blockout → structure → form → materials → surface → lighting → interaction → optimization.
5. Compare renders against the reference and refine until the quality gates pass.
6. Keep geometry procedural and editable rather than relying on downloaded meshes.

## Quality rules
- Preserve silhouette, proportions, camera relationship, and identity-defining details.
- Map details to real components or materials instead of adding arbitrary decoration.
- Be explicit about uncertainty where a single image cannot reveal hidden geometry.
- Expose pivots/sockets where animation may be needed.
- Prefer readable TypeScript and reusable geometry/material factories.

## Reference
https://github.com/img2threejs/img2threejs

## License
Apache-2.0

## Armory guidance
Use this when an agent has a reference image and needs to reconstruct it as editable Three.js code. Pair it with the Armory's Vision and Screen Use/Open Computer Use capabilities when the agent needs image inspection or browser-based render verification.
