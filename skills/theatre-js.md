# Theatre.js Skill

## Purpose
Reference for using Theatre.js as a high-fidelity motion-design and animation system for web experiences.

## Covers
- Theatre.js projects, sheets, sheet objects, props, and sequences
- Visual keyframe authoring with Theatre Studio
- Timeline / dope-sheet sequencing and graph-based easing refinement
- HTML/CSS/SVG animation through JavaScript values
- THREE.js and React Three Fiber cinematic animation workflows
- Coordinating UI motion, 3D scenes, camera movement, lighting, and shaders
- Programmatic playback and animation control
- Audio-synchronized animation workflows
- Studio extensions and custom editing workflows
- Advanced frame-driving / render / performance scenarios
- Coordinating Theatre.js with other animation systems such as GSAP

## Recommended workflow
1. Use Theatre.js when an animation benefits from detailed keyframe authoring, timeline control, or designer/developer iteration in the browser.
2. Keep the animated state explicit by defining Sheet Objects and only the props that actually need animation.
3. Use Sheets and Sequences to organize related motion into reusable timelines rather than scattering animation state across components.
4. Use Theatre Studio during development for visual tuning; keep production behavior and runtime playback cleanly separated from authoring concerns.
5. For THREE.js / React Three Fiber, use Theatre.js for cinematic object, camera, and scene motion while keeping rendering responsibilities in the 3D stack.
6. When combining Theatre.js with GSAP or another animation library, avoid competing writers for the same properties and synchronize frame loops where appropriate.
7. Respect `prefers-reduced-motion` and avoid motion that is purely decorative when it harms usability or performance.
8. Treat Theatre Studio extensions as an advanced API surface and verify compatibility against the current Theatre.js documentation before relying on them.

## Useful packages
- `@theatre/core` — runtime animation engine and core API
- `@theatre/studio` — visual animation editor / authoring UI
- `@theatre/r3f` — official React Three Fiber extension

## Official references
- https://www.theatrejs.com/
- https://www.theatrejs.com/docs/latest
- https://github.com/theatre-js/theatre

The official documentation describes Theatre.js as a JavaScript animation library with a professional motion-design toolset. It supports workflows for React Three Fiber, THREE.js, and HTML/CSS/SVG, with a sequence editor and graph editor for detailed animation authoring.
