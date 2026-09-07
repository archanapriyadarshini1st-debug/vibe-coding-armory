# GSAP Skill

## Purpose
Reference for using GSAP for production-quality web animation.

## Covers
- Core tweens: `to`, `from`, `fromTo`, `set`
- Timelines and sequencing
- ScrollTrigger and scroll-linked motion
- React integration and cleanup
- GSAP plugins and utilities
- Performance and reduced-motion practices

## Recommended workflow
1. Use transforms instead of layout-heavy properties where possible.
2. Use timelines for coordinated sequences rather than delay chains.
3. Use `gsap.context()` / `useGSAP()` patterns in React and clean up animations on unmount.
4. Use `gsap.matchMedia()` for responsive animation and `prefers-reduced-motion`.
5. Use ScrollTrigger for scroll-driven effects instead of hand-written scroll listeners when appropriate.

## Official source
https://github.com/greensock/gsap-skills

Official GSAP skills are MIT licensed and include specialized skills such as `gsap-core`, `gsap-timeline`, `gsap-scrolltrigger`, `gsap-plugins`, `gsap-utils`, `gsap-react`, and `gsap-performance`.
