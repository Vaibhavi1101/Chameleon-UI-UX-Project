# Cognitive Accessibility — Adaptive Rules

## 1. Purpose

This document defines the proposed adaptive rules for the Cognitive Accessibility module of Chameleon.

The rules translate the problem and goals defined in the previous stage into specific interface behaviors that can be demonstrated through the Figma prototype.

The Chameleon project brief proposes that, when a high cognitive load is detected, the interface should automatically reduce motion and blur background noise.

For this project, these behaviors will be simulated through Figma states rather than implemented as a real cognitive-load detection system.

---

## 2. Adaptive State Model

The Cognitive Accessibility module will use two primary interface states:

| State | Description |
|---|---|
| Normal State  | The standard dashboard experience with normal motion, visual hierarchy, and background elements |
| Cognitive-Friendly State  | An adaptive state where unnecessary motion and background visual noise are reduced |

The transition between these states represents the proposed response to a change in the user's cognitive context.

---

## 3. Core Adaptive Rules

| Rule | Condition | Interface Adaptation | Purpose |
|---|---|---|---|
| COG-01 | Cognitive-friendly state is active | Reduce unnecessary animations | Reduce visual movement that may compete for attention |
| COG-02 | Cognitive-friendly state is active | Reduce or blur background visual noise | Keep the primary content visually focused |
| COG-03 | Cognitive-friendly state is active | Maintain emphasis on primary information | Ensure important information remains easy to identify |
| COG-04 | Cognitive-friendly state is active | De-emphasize secondary elements | Reduce competition between primary and secondary content |
| COG-05 | Cognitive-friendly state is active | Preserve essential controls and information | Avoid removing core dashboard functionality |
| COG-06 | State changes | Preserve the existing design system | Keep the adaptive state visually consistent with the rest of Chameleon |

---

## 4. Rule COG-01 — Reduce Unnecessary Motion

### Condition

The cognitive-friendly state becomes active.

### Adaptation

Unnecessary animations and motion within the dashboard should be reduced or disabled.

Examples may include:

- Decorative animations
- Non-essential transitions
- Continuously moving background elements
- Repeated visual movement

Meaningful feedback and essential interaction states should remain understandable.

### Purpose

The goal is to reduce visual movement that may compete with the user's attention.

---

## 5. Rule COG-02 — Reduce Background Visual Noise

### Condition

The cognitive-friendly state becomes active.

### Adaptation

Background or secondary visual elements should become less visually dominant.

The project brief specifically proposes **blurring background noise** as part of the cognitive accessibility behavior.

For the Figma prototype, this may be represented through:

- Background blur
- Reduced visual prominence
- Lower-detail background elements
- De-emphasis of secondary content

### Purpose

The primary information should remain visually clear while background elements create less competition.

---

## 6. Rule COG-03 — Preserve Primary Information

### Condition

The cognitive-friendly state is active.

### Adaptation

Primary information should remain visible and visually prominent.

The adaptive state should not simply hide information without considering its importance.

Possible design approaches include:

- Stronger visual hierarchy
- Clearer grouping
- Greater emphasis on primary dashboard content
- Reduced prominence of secondary information

### Purpose

Users should still be able to identify the information required for their main task.

---

## 7. Rule COG-04 — De-emphasize Secondary Elements

### Condition

The cognitive-friendly state is active.

### Adaptation

Secondary elements that are not immediately necessary for the primary task may be visually de-emphasized.

This could include:

- Secondary cards
- Supporting information
- Decorative elements
- Non-essential notifications
- Secondary actions

De-emphasis should not automatically mean removal.

### Purpose

Reducing the visual competition between elements can help establish a clearer hierarchy.

---

## 8. Rule COG-05 — Preserve Core Functionality

### Condition

The cognitive-friendly state is active.

### Adaptation

Essential dashboard functions and controls should remain available.

The adaptive state should primarily modify presentation rather than removing the user's ability to complete the main task.

### Purpose

Accessibility adaptation should simplify the experience without making the interface incomplete.

---

## 9. Rule COG-06 — Maintain Design-System Consistency

### Condition

The interface changes between normal and cognitive-friendly states.

### Adaptation

The adaptive state should continue using the shared Chameleon design system.

This includes maintaining consistency in:

- Typography
- Color system
- Spacing
- Components
- Labels
- Interaction patterns

Only the properties required for the adaptive behavior should change.

### Purpose

The transition should feel like the same product adapting to a different state rather than becoming a completely different interface.

---

## 10. Adaptive State Comparison

| UI Property | Normal State | Cognitive-Friendly State |
|---|---|---|
| Motion | Normal interface motion | Unnecessary motion reduced |
| Background | Normal visual treatment | Background noise reduced or blurred |
| Primary Information | Standard hierarchy | Stronger visual priority |
| Secondary Information | Normal prominence | De-emphasized where appropriate |
| Essential Controls | Available | Remain available |
| Design System | Shared system | Same system with adaptive changes |

---

## 11. Prototype Trigger

The project brief describes the cognitive-friendly behavior as occurring when **high cognitive load is detected**.

For the Figma prototype, the detection mechanism will be represented as a simulated condition rather than a real detection system.

### Prototype Flow

**Normal State**

↓

**High Cognitive Load Detected — Simulated**

↓

**Cognitive-Friendly State**

↓

- Reduce unnecessary motion
- Reduce or blur background noise
- Strengthen primary information hierarchy
- De-emphasize secondary elements
- Preserve essential functionality

---

## 12. Design Constraints

The adaptive behavior should follow these constraints:

### Do Not Remove Essential Information

Important information required for the user's main task should remain available.

### Do Not Create a Completely Different Interface

The cognitive-friendly state should remain recognizable as the same dashboard.

### Do Not Depend on Color Alone

Changes in state should be communicated through more than color changes.

### Do Not Add Unnecessary Complexity

The adaptive solution itself should remain simple and predictable.

### Do Not Claim Real Detection

The Figma prototype will simulate the condition. It will not claim to detect a user's actual cognitive load.

---

## 13. Figma Implementation Direction

The rules will be demonstrated using separate Figma states or variants.

### State 1 — Normal Dashboard

Show the standard dashboard with:

- Normal visual hierarchy
- Normal background elements
- Normal motion or transition behavior

### State 2 — Cognitive-Friendly Dashboard

Show the same dashboard with:

- Reduced unnecessary motion
- Reduced or blurred background noise
- Stronger primary-content hierarchy
- De-emphasized secondary elements
- Preserved essential functionality

The two states should be visually comparable so that the adaptive changes are easy to understand during the final review.

---

## 14. Rule Validation Checklist

Before finalizing the prototype, the following should be checked:

- Unnecessary motion is reduced.
- Background visual noise is reduced or blurred.
- Primary information remains prominent.
- Secondary elements are less visually competitive.
- Essential controls remain available.
- The same core dashboard structure is maintained.
- The shared design system remains consistent.
- The state transition is understandable.
- The prototype clearly indicates that cognitive-load detection is simulated.

---

## 15. Next Step

The next stage is to translate these adaptive rules into wireframes.

The wireframes will first establish the normal dashboard structure and then show how the interface changes when the cognitive-friendly state is activated.

The final prototype will use these states to demonstrate the proposed adaptive behavior.