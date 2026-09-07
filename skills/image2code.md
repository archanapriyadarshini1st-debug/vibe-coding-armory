# Image2Code Skill

Turn a reference screenshot or image into a structured, high-fidelity frontend implementation by extracting layout, typography, spacing, components, visual hierarchy, interactions, and responsive behavior.

## Best for
- Screenshot-to-HTML/React implementation
- UI reconstruction from reference images
- High-fidelity landing pages and app screens
- Component and layout inference
- Responsive breakpoint planning
- Visual comparison and iterative refinement

## Workflow
1. Inspect the reference image carefully before coding.
2. Identify page structure, containers, grid/flex relationships, typography, spacing, colors, borders, shadows, imagery, icons, and motion cues.
3. Convert observations into a component/layout plan.
4. Implement semantic, responsive frontend code using the project's existing stack and design system.
5. Render the result and compare it against the reference.
6. Fix the largest visual mismatches first, then refine micro-details.

## Quality rules
- Match hierarchy and composition before decorative details.
- Do not fake a visual match with a single screenshot background when the target is meant to be real UI.
- Use reusable components and maintainable styles.
- Preserve responsive behavior rather than hard-coding one viewport.
- Use accessible semantics and interactions.
- Verify the final render visually when browser/screenshot tooling is available.

## Armory guidance
Combine with Vision for reference-image analysis and Screen Use/Open Computer Use or browser tooling for render verification. Combine with UI/UX Pro Max, Frontend Design, Web Design Guidelines, and UI Clone/Reverse Engineering when a project requires production-grade fidelity.
