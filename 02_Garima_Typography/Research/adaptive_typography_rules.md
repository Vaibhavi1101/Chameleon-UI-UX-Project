# Adaptive Typography – Adaptive Rules

## 1. Purpose

This document defines the proposed adaptive rules for the **Adaptive Typography module of Chameleon**.

The rules translate the typography problem and goals defined in the previous stage into specific interface behaviours that can be demonstrated through the Figma prototype.

The rules focus on how typography can adapt through changes in text size, font weight, line height, letter spacing, and hierarchy while keeping the existing dashboard structure consistent.

For this project, these adaptive behaviours will be demonstrated through **Normal and Adaptive states in Figma** rather than implemented as a real-time automatic detection system.


---
## 2. Typography State Model

The Adaptive Typography experience is defined through two states:

| **State**          | **Description**                                                                                                                                                              |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Normal State**   | Standard dashboard typography with default text size, weight, spacing, and hierarchy.                                                                                        |
| **Adaptive State** | Adjusted typography with increased text size and controlled changes in weight, line height, and letter spacing while maintaining the same hierarchy and dashboard structure. |

The transition from Normal to Adaptive represents the proposed typography adaptation within the same dashboard.

---
## 3. Adaptive Typography Rules

### Rule 1 — Selective Type Scaling

**Condition**

Adaptive Typography is activated and the interface needs stronger text visibility.

**Adaptive Behaviour**

Increase text size selectively according to the importance and role of the content. Larger adjustments can be applied to prominent information, while secondary text can receive smaller changes.

**Purpose**

To make important information easier to notice without enlarging every piece of text equally.

---

### Rule 2 — Preserve Typography Hierarchy

**Condition**

Typography sizes or other text properties are changed in the Adaptive state.

**Adaptive Behaviour**

Maintain clear differences between different levels of information. Changes should strengthen the existing hierarchy rather than flattening it.

**Purpose**

To ensure users can still understand what is most important and what is supporting information.

---

### Rule 3 — Controlled Font Weight

**Condition**

Typography size increases and additional visual definition is required.

**Adaptive Behaviour**

Adjust font weight selectively where needed. Weight changes should support the existing hierarchy instead of making all text appear bold.

**Purpose**

To give important text stronger visual definition while keeping the overall interface balanced.

---

### Rule 4 — Adjust Line Height

**Condition**

Text becomes larger in the Adaptive state.

**Adaptive Behaviour**

Increase line height where necessary to provide enough vertical space between lines. The spacing should remain proportional to the updated text size.

**Purpose**

To prevent larger text from appearing crowded and maintain a clear reading structure.

---

### Rule 5 — Controlled Letter Spacing

**Condition**

Certain text becomes visually dense after typography changes.

**Adaptive Behaviour**

Apply small adjustments to letter spacing where required. The change should remain subtle and consistent with the text size.

**Purpose**

To maintain clear character separation without making the interface feel unnecessarily spaced out.

---

### Rule 6 — Maintain Layout Stability

**Condition**

Typography properties change within the existing dashboard layout.

**Adaptive Behaviour**

Keep text within its intended boundaries and prevent overflow, overlap, clipping, or broken alignment. Components should accommodate typography changes without unnecessarily changing the overall dashboard structure.

**Purpose**

To ensure that adaptive typography does not disrupt the usability or visual structure of the dashboard.

---

### Rule 7 — Maintain Consistent Typography Behaviour

**Condition**

The same typography role appears in multiple areas of the dashboard.

**Adaptive Behaviour**

Apply the same adaptive treatment to the same typography role wherever it appears. Similar text should respond in a consistent way across the interface.

**Purpose**

To create predictable typography behaviour and support a reusable approach across the dashboard.




---

## 4. Typography Value Mapping

The following values will be used as the initial direction for the Adaptive Typography prototype:

| **Typography Property** | **Normal** | **Adaptive** |
| ----------------------- | ---------: | -----------: |
| Font Size               |      16 px |        20 px |
| Font Weight             |    Regular |       Medium |
| Line Height             |      24 px |        30 px |
| Letter Spacing          |       0 px |       0.2 px |
| Heading Size            |      32 px |        40 px |

These values provide a starting point for demonstrating the difference between the Normal and Adaptive states.

The values can be refined during Figma testing to maintain readability, hierarchy, and layout stability within the dashboard.

---

## 5. Normal and Adaptive Comparison

The following comparison shows the overall difference between the Normal and Adaptive typography states:

| Aspect              | Normal State                | Adaptive State               |
| ------------------- | --------------------------- | ---------------------------- |
| Typography          | Default typography settings | Adjusted typography settings |
| Text Size           | Standard                    | Increased selectively        |
| Font Weight         | Standard                    | Adjusted where required      |
| Spacing             | Default                     | Increased where required     |
| Hierarchy           | Standard                    | Preserved                    |
| Content             | Same                        | Same                         |
| Components          | Same                        | Same                         |
| Dashboard Structure | Standard                    | Kept consistent              |

The Adaptive state changes the typography treatment while keeping the same content, components, hierarchy, and overall dashboard structure.

The exact typography values used for the prototype are defined in the **Typography Value Mapping** section.

---

## 6. Figma Implementation

The rules will be demonstrated through two dashboard states in Figma.

### Normal Dashboard

The dashboard uses the standard typography settings and existing interface structure.

### Adaptive Dashboard

The same dashboard uses the adaptive typography settings defined in this document.

The two states will be connected in the prototype to demonstrate the typography transition while keeping the underlying interface consistent.

---

## 7. Validation

Before finalising the UI, the typography behaviour will be checked across the dashboard.

The design should demonstrate that:

* Typography changes are clearly visible
* Hierarchy remains understandable
* Text stays within its intended boundaries
* Similar typography roles behave consistently
* Spacing remains balanced
* Dashboard alignment is maintained
* The Adaptive state still looks like the same dashboard

---

## 8. Design Constraints

The adaptive typography behaviour should follow these constraints:

### Do Not Change the Overall Dashboard Structure

The Adaptive state should use the same dashboard layout, navigation, components, and content as the Normal state.

### Do Not Remove or Hide Information

Typography adaptation should not reduce the visibility or availability of important dashboard information.

### Do Not Break Component Layouts

Changes in font size, line height, weight, or letter spacing should remain within the intended component boundaries and should not cause overflow, clipping, or overlap.

### Do Not Flatten Typography Hierarchy

Adaptive changes should maintain clear visual differences between different levels of information so that the existing hierarchy remains understandable.

### Do Not Apply Typography Changes Excessively

Adaptation should be controlled and selective. Typography properties should not be increased unnecessarily when a smaller adjustment is sufficient.

### Do Not Claim Automatic User Detection

The Figma prototype will demonstrate the Normal and Adaptive states as a simulated interaction. It will not claim to detect a user's actual reading condition or automatically determine their typography requirements.

---

## 9. Next Step

The next stage is to apply the defined typography behaviour to the dashboard wireframes.

The wireframes will establish the normal typography first and then demonstrate how typography adapts while the dashboard structure, content, and components remain consistent.

These wireframes will provide the foundation for the high-fidelity UI and final interactive prototype.

---

## 10. Conclusion

The defined typography rules establish how the dashboard can move from a Normal state to an Adaptive state without changing its overall structure.

By controlling text size, hierarchy, font weight, and spacing, the proposed approach keeps typography flexible while maintaining a consistent dashboard experience.

These rules will guide the next stage of wireframing and high-fidelity UI development.

