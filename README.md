# Chameleon — Adaptive Accessibility Design System

Chameleon explores how a familiar dashboard interface can adapt to different user contexts while keeping its core layout, visual language, and essential information consistent.

The project uses a shared analytics dashboard as its baseline and demonstrates adaptive states through UI screens, wireframes, documentation, and Figma prototypes.

## Project Goals

- Explore context-aware accessibility adaptations.
- Keep a consistent dashboard structure across modules.
- Improve readability, focus, and interaction accessibility without unnecessarily changing the whole interface.
- Distinguish simulated prototype behavior from implemented functionality.

## Modules and Contributions

| Team member | Modules | Focus |
|---|---|---|
| **Vaibhavi Parmar** | Cognitive Accessibility; Sensor-Driven Interaction | Cognitive-friendly dashboard states, information hierarchy, and the adaptive hit-target interaction concept. |
| **Garima Saxena** | Adaptive Typography; Adaptive Color | Typography adaptation based on viewing context and adaptive color concepts. |

## Module Overview

### 1. Cognitive Accessibility

Explores how a dashboard can reduce unnecessary visual complexity and make important information easier to identify when higher cognitive load is simulated.

Design examples include:
- A Focus Mode indicator.
- Stronger hierarchy for key KPI values.
- Removal of redundant KPI sparklines.
- Clearer separation in the sales chart.
- Quieter secondary details while retaining important information.

**Prototype limitation:** Cognitive-load detection is simulated in Figma. Real cognitive-load or biometric detection is not implemented.

### 2. Sensor-Driven Interaction

Explores expanding selected invisible hit areas when unsteady cursor movement is detected, while keeping the visible controls and dashboard layout familiar.

The prototype demonstrates:
- A normal dashboard state.
- An interaction-adjustment notification.
- An adaptive interaction dashboard.
- Annotated target boundaries around selected controls, such as Overview and the date-range selector.

**Prototype limitation:** Detection and adaptive behavior are simulated in Figma. Real-time cursor sensing and dynamic hit-area expansion are not implemented as working software.

### 3. Adaptive Typography

Explores adapting typographic presentation in response to a simulated viewing-distance condition while preserving the dashboard's core structure.

**Prototype limitation:** Viewing-distance detection is represented as a Figma prototype scenario; real sensor detection is not claimed.

### 4. Adaptive Color

Explores adaptive color concepts as part of the wider Chameleon design system. Refer to the shared Figma file and module documentation for the final screens and design details.

## Shared Design Approach

The common dashboard includes:
- Navigation sidebar and header
- Overview and date-range control
- KPI cards
- Sales-performance chart
- Recent activity
- Recent-transactions table

The shared baseline helps keep modules visually consistent while allowing each one to demonstrate a different adaptive response.

## Tools

- **Figma** — UI design, wireframes, adaptive states, annotations, and prototype flows.
- **GitHub** — project files and supporting documentation.

## Scope and Limitations

This project primarily demonstrates design concepts and prototype behavior. Context detection and adaptive responses described above are simulated in Figma rather than implemented as real-time software functionality.

## Project Links

- **Figma:** [Add shared Figma link]
- **GitHub:** [Add repository link]

## Future Work

- Validate adaptive states with users.
- Test readability, target selection, and transitions.
- Implement and evaluate actual context-sensing mechanisms.
- Consolidate design tokens, state behavior, and handoff documentation.

---

*Chameleon — one familiar interface, different adaptive responses.*
