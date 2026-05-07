# material-design-skill
# Material 3 Expressive — Design Engineering Skill

A 4,600-line reference for AI coding agents implementing Material 3 Expressive UI across any platform. All token values verified against official source code.

## Scope

Covers Web, Android/Compose, iOS/SwiftUI, Flutter, Desktop (ImGui/egui/Qt), and game engines (Unity/Godot). For frameworks without M3E support, provides from-scratch implementation algorithms.

## Contents

| # | Section | Coverage |
|---|---------|----------|
| 1 | Motion System | 10 easing tokens, 16 duration tokens, 6 spring tokens, 5 motion patterns, spring solver |
| 2 | Color & Dynamic Theming | HCT/CAM16 pipeline, 9 scheme variants, 49 color roles, tonal elevation, harmonization |
| 3 | Shape, Elevation & States | 10 shape tokens, 6 shadow levels, state opacities (0.08/0.1/0.1/0.16), focus ring (3px/2px) |
| 4 | Component Anatomy | 13 component families with dp-precise specs, states, and per-platform notes |
| 5 | Container Transform | 5 transition patterns, FLIP algorithm, gesture-driven transitions, per-platform strategies |
| 6 | Animation Decision Framework | Pattern/easing/duration decision trees, asymmetric timing, reduced-motion rules |
| 7 | Platform Translation | Spring conversion formulas, API mapping across 6 platforms, minimum viable M3E subset |
| 8 | Adaptive Layout | 5-class breakpoints, 3 canonical layouts, foldable patterns, navigation adaptation |
| 9 | Accessibility | Reduced motion, touch targets, WCAG contrast, focus indicators, semantic markup |
| 10 | Performance | GPU-safe properties per platform, Framer Motion caveat, rendering cost table |
| 11 | Debugging & Verification | Slow-motion testing, token verification scripts, cross-device testing matrix |
| 12 | Review Checklist | 33-item review table, 10-point quick audit, Before/After/Why format |

## Verification

Token values sourced from Material Web v34.0.21, Material Components Android `tokens.xml`, and `@material/material-color-utilities`. Key corrections from prior versions: 10 easing tokens (not 18), state layer focus/press opacity 0.1 (not 0.12), focus ring 3px thick / 2px offset (not 2px/3px), `easing-emphasized` equals `easing-standard` on web.

## Minimum Viable Subset

For custom engines: 12 color roles, 3 radii, 2 surface tones, 2 states, 2 curves. Yields ~80% spec compliance at ~20% implementation cost.

## License

Material Design 3 Expressive specification is copyright Google LLC. Token values sourced from Material Components repositories under Apache 2.0.
