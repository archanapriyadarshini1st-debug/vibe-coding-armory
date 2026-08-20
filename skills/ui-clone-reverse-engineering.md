# UI Clone / Reverse-Engineering Skill

## Purpose
Given a live website URL and an existing project, reverse-engineer the target site's visual language and interaction model, then adapt those findings to the existing project instead of blindly copying the target site's content or branding.

Inspired by the public `voidmatcha/ui-clone-skills` project. This file is an original project-local workflow, not a copy of that repository's implementation.

## Workflow

1. **Inspect the target URL**
   - Load desktop and mobile views when possible.
   - Identify page structure, typography, spacing, colors, borders, shadows, imagery, icons, containers, grids, and responsive breakpoints.
   - Record initial, hover, focus, active, scroll, menu, loading, and reduced-motion states.

2. **Reverse-engineer motion**
   - Identify whether motion appears to use CSS, GSAP, Framer Motion, Webflow interactions, native scrolling, or canvas/WebGL.
   - Estimate durations, delays, easing, distances, opacity/scale changes, stagger patterns, and scroll thresholds.
   - Reproduce observable behavior with maintainable code, not screenshot/video fakery.

3. **Extract the design system**
   - Create a compact inventory of fonts/weights, type scale, colors, radii, spacing rhythm, container widths, grid rules, buttons, cards, icons, and imagery.
   - Separate reusable design DNA from target-specific copy, logos, and branding.

4. **Apply the design DNA to the existing project**
   - Inspect its component tree, routing, styling system, dependencies, and current visual identity.
   - Preserve existing functionality unless replacement is explicitly requested.
   - Translate target layout and interaction patterns into the project's existing architecture.
   - Keep the project's own content and branding.

5. **Implement progressively**
   - Global typography/tokens first.
   - Layout/responsive behavior second.
   - Interactions/animation third.
   - Advanced canvas/WebGL only when it materially improves fidelity and is practical.

6. **Visual QA**
   - Compare matching viewport sizes.
   - Check alignment, typography metrics, section heights, whitespace, animation timing, hover states, and responsive behavior.
   - Fix the largest visual mismatches first.
   - Do not claim pixel-perfect fidelity without actual visual verification.

## Rules

- Treat the target as design/interaction inspiration, not permission to copy proprietary branding, private source code, or copyrighted content wholesale.
- Prefer real DOM/CSS/JS behavior over static screenshots.
- Keep animation performant and accessible; honor `prefers-reduced-motion` where practical.
- Avoid viewport-specific hacks when responsive rules can express the same result.
- If the target uses a recognizable library, reproduce observable behavior with an appropriate implementation rather than assuming access to private source.

## Expected output

When given a target URL, produce:

1. A concise reverse-engineering report.
2. A design-token and visual-system summary.
3. An interaction and animation inventory.
4. A mapping from target patterns to existing project components.
5. The implementation changes.
6. A visual QA pass with remaining mismatches identified.

## Natural-language triggers

- `Reverse engineer https://example.com and apply its design language to this project.`
- `Study this site and make my existing homepage use the same interaction quality.`
- `Clone the visual behavior of this URL, but keep my content and branding.`

## Upstream reference

https://github.com/voidmatcha/ui-clone-skills
