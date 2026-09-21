# Adaptive Typography — Research

## 1. Module Overview

**Project:** Chameleon: Algorithmic Accessibility Engine

**Module:** Adaptive Typography

**Focus:** Making information easier to read by allowing typography to adapt to different reading and viewing conditions.

### Main Question

> **How can we make information easier to read through adaptive typography?**

### Project Direction

The Chameleon project explores an adaptive interface instead of relying only on fixed accessibility settings.

For this module, the focus is on making the reading experience more flexible according to different user needs and viewing conditions.

The goal is to improve readability without creating a completely different interface.

---

# 2. The Problem with Fixed Typography

Most interfaces use fixed typography values across the entire interface. This can create limitations when reading conditions or user needs change.

* **Fixed Font Size:** Text usually stays at the same size even when a user may need larger text.
* **Fixed Font Weight:** Users cannot easily adjust how light or heavy the text appears.
* **Fixed Text Width:** The width of characters remains the same, which may not work equally well in every situation.
* **Fixed Spacing:** Line height and letter spacing often remain unchanged.
* **Limited Accessibility Controls:** A simple “Large Text” option usually changes only the font size.
* **Layout Challenges:** Increasing text size or spacing can cause content to overflow, overlap or become difficult to use in dense dashboards.

This creates an opportunity to explore a typography system that can adapt multiple properties while keeping the dashboard structure and information architecture consistent.

---

# 3. What Is Adaptive Typography?

Adaptive Typography focuses on making text easier to read by adjusting its presentation according to different viewing and reading needs.

The main properties that can be adjusted are:

* Font Size
* Font Weight
* Font Width
* Optical Size
* Line Height
* Letter Spacing

Instead of using the same typography settings for every situation, an adaptive system can change these properties while keeping the overall interface and content structure consistent.

The important idea is that **the interface does not need to be redesigned just because the typography changes.**

---

# 4. Key Research Findings

## Finding 1 — Text Spacing Supports Readability

W3C's WCAG guidance includes requirements around text spacing, including line height, paragraph spacing, letter spacing and word spacing.

This shows that readable text is not only about font size. The space around and between text is also important.

### Design Implication

For Chameleon:

* Line height should be adjustable.
* Letter spacing should be adjustable.
* Text groups should have comfortable spacing.
* Increased spacing should not break cards, tables or other UI components.

**Source:** W3C — Understanding SC 1.4.12: Text Spacing

---

## Finding 2 — Variable Fonts Allow Flexible Typography

Variable fonts allow different variations of a typeface to exist within a single font file.

Instead of using separate font files for Regular, Medium and Bold, a variable font can provide a range of values between these styles.

Common axes include:

* Weight
* Width
* Optical Size

This allows typography to change more gradually instead of switching only between fixed styles.

### Design Implication

For Chameleon, the typography system will explore controlled changes in **Weight, Width and Optical Size** instead of depending only on fixed font styles.

**Source:** Microsoft Learn — OpenType Font Variations Overview

---

## Finding 3 — Optical Size Can Adapt the Typeface

Optical Size (`opsz`) is a variable font axis that allows a typeface to change its design for different text sizes.

A font can therefore use different letterform characteristics at smaller and larger sizes instead of simply scaling the same design.

### Design Implication

For Chameleon, Optical Size can be adjusted along with text size so that typography adapts as a complete system rather than only becoming larger.

**Source:** Microsoft Learn — OpenType Font Variations / opsz Axis

---

## Finding 4 — Weight and Width Provide More Control

Weight (`wght`) controls the relative thickness of the typeface, while Width (`wdth`) controls how narrow or wide the text appears.

Both properties can be adjusted independently in a variable font.

### Design Implication

For the Chameleon dashboard:

* Weight can be adjusted for stronger or lighter emphasis.
* Width can be adjusted when text needs more or less horizontal space.
* These changes can be tested without changing the dashboard structure.

**Source:** Microsoft Learn — OpenType Font Variations / wght and wdth Axes

---

## Finding 5 — Typography Needs a Clear Hierarchy

Typography helps users understand different levels of information.

In a dashboard, headings, body text, labels and data values should not all have the same visual importance.

A clear hierarchy helps users understand what information is important and what they should read first.

### Design Implication

For Chameleon:

* Headings should remain clearly distinguishable.
* Body text should remain comfortable to read.
* Labels and supporting information should have lower visual priority.
* Data values should have a strong but consistent hierarchy.
* Adaptive changes should not destroy the original hierarchy.

**Source:** UXDT — UI/UX Guidelines: Typography

---

## Finding 6 — Text Should Remain Usable at Larger Sizes

WCAG 2.2 includes guidance related to presenting text at larger sizes while maintaining access to content and functionality.

This is particularly important for interfaces containing dense information such as dashboards, tables and data cards.

### Design Implication

For Chameleon:

* Test typography at larger scales.
* Check that cards do not overlap.
* Check that table content remains readable.
* Ensure buttons and navigation remain usable.
* Maintain layout stability when text becomes larger.

**Source:** W3C — WCAG 2.2, Success Criterion 1.4.8: Visual Presentation

---

# 5. Important Typography Parameters

The Adaptive Typography system uses six main parameters. Each one controls a different part of how text appears and behaves.

| **Parameter**      | **What it controls**                | **Use in Chameleon**                              |
| ------------------ | ----------------------------------- | ------------------------------------------------- |
| **Font Size**      | Overall size of text                | Adjusts text scale according to the reading state |
| **Font Weight**    | Thickness of characters             | Controls visual emphasis and text strength        |
| **Font Width**     | Horizontal proportion of characters | Controls how wide or compact text appears         |
| **Optical Size**   | Typeface design for different sizes | Helps the font adapt to the intended text size    |
| **Line Height**    | Vertical space between lines        | Gives text more breathing space                   |
| **Letter Spacing** | Space between individual letters    | Controls character spacing                        |

These parameters can work together to create different typography states.

---

# 6. Variable Typography in Chameleon

Variable Typography is the main technical direction for the Adaptive Typography module.

In a traditional font system, different styles are usually provided as separate options such as Regular, Medium and Bold.

A variable font can provide a range of values for properties such as weight, width and optical size within a single font file.

### Main Variable Font Axes

* **Weight (`wght`):** Controls how light or heavy the characters appear.
* **Width (`wdth`):** Controls how narrow or wide the characters appear.
* **Optical Size (`opsz`):** Adjusts the design of the typeface for different text sizes, when supported by the font.

### Why It Is Useful for Chameleon

Variable fonts give the system more control over typography.

For Chameleon, they can help create a gradual change between the normal and adaptive reading states.

### Normal State

The normal state represents the standard dashboard typography.

* **Heading:** 32px, Medium
* **Body Text:** 16px, Regular
* **Labels:** 14px, Regular
* **Data Values:** 24px, Medium
* **Line Height:** Default
* **Letter Spacing:** Default
* **Font Width:** Default
* **Optical Size:** Default

### Adaptive State

The adaptive state changes typography properties to provide a more comfortable reading experience.

* **Heading:** 40px, Semibold
* **Body Text:** 20px, Medium
* **Labels:** 16px, Medium
* **Data Values:** 30px, Semibold
* **Line Height:** Increased
* **Letter Spacing:** Slightly increased
* **Font Width:** Slightly wider
* **Optical Size:** Adjusted for the larger text size, when supported by the font

These are **initial design values for the prototype** and can be refined during the Figma design and testing stage.

The dashboard content, components and information architecture remain the same while the typography adapts.

---

# 7. Typography in Data-Heavy Dashboards

Dashboards contain several types of information in a limited space:

* Headings
* Metric values
* Labels
* Charts
* Tables
* Filters
* Navigation
* Supporting information

Because of this density, typography needs to communicate hierarchy clearly.

The adaptive typography system should therefore change the reading experience without changing the information architecture.

The user should still be able to understand:

**What is important?**

**What belongs together?**

**What should I read first?**

---

# 8. Proposed Adaptive Typography System

The research findings will be translated into a reusable typography system for the Chameleon dashboard.

The system will define typography tokens for different UI elements, including:

* Headings
* Body text
* Labels
* Data values
* Navigation
* Supporting text

The system will also define how typography changes when the adaptive state is enabled.

The main goals are:

* Improve readability
* Maintain clear hierarchy
* Keep the interface structure consistent
* Prevent text from breaking the layout
* Make typography changes reusable across components

The exact values can be refined during the Figma design and testing stage.

---

# 9. Normal vs Adaptive Typography

The Normal and Adaptive states use the same dashboard content and structure.

The comparison is intended to show how typography can change the reading experience without changing the overall interface.

### Normal Typography

The standard dashboard uses the default typography system and normal information density.

### Adaptive Typography

The adaptive version keeps the same:

* Dashboard structure
* Content
* Components
* Charts
* Tables
* Navigation

The typography-related properties are adapted while the overall interface remains consistent.

---

# 10. Typography Design Principles

### 1. Adapt More Than Font Size

The system should not behave like a basic “Large Text” toggle.

### 2. Use Variable Font Capabilities

Weight, width and optical size can provide more flexibility than fixed font styles.

### 3. Preserve Hierarchy

Typography changes should not remove the distinction between headings, body text, labels and data.

### 4. Maintain Comfortable Spacing

Line height and letter spacing should support a comfortable reading experience.

### 5. Protect the Layout

Typography changes should not cause overlapping, clipping or broken components.

### 6. Keep the Interface Consistent

The dashboard structure should remain familiar while typography adapts.

---

# 11. Research-to-Design Mapping

| **Research Finding**                      | **Design Response**                               |
| ----------------------------------------- | ------------------------------------------------- |
| Text spacing supports readability         | Add adjustable line height and letter spacing     |
| Variable fonts allow continuous variation | Use Weight and Width axes                         |
| Optical size can vary with text size      | Include Optical Size in the typography system     |
| Weight and width can vary independently   | Explore controlled weight and width changes       |
| Typography supports visual hierarchy      | Create clear typography levels                    |
| Text should remain usable at larger sizes | Test the dashboard at larger accessibility scales |

---

# 12. Planned Figma Designs

The research will be translated into a small set of Figma screens.

### 1. Normal Dashboard

The baseline dashboard using standard typography.

### 2. Adaptive Dashboard

The same dashboard with adaptive typography enabled.

### 3. Typography Control Panel

Controls for:

* Font Size
* Weight
* Width
* Optical Size
* Line Height
* Letter Spacing

### 4. Variable Font Playground

A visual demonstration of the variable typography axes.

### 5. Normal vs Adaptive Comparison

A side-by-side comparison showing how the same dashboard changes while the content and layout remain consistent.

---

# 13. Limitations

This project is a design concept and Figma prototype, not a clinically validated accessibility system.

It does not measure a user's actual visual condition or diagnose a reading difficulty.

The typography values proposed in the prototype will need further testing with real users to determine which combinations provide the best reading experience.

---

# 14. Conclusion

The research shows that accessible typography is not limited to increasing font size.

Text spacing, typography hierarchy and variable font properties can provide additional flexibility when designing readable interfaces.

Variable fonts are particularly useful because they can support continuous changes across axes such as weight, width and optical size.

For this project, these ideas will be explored through a dashboard that keeps the same information and layout while allowing its typography to adapt.

The next stage is to translate the research into the planned Figma screens and test how the typography changes affect readability and layout stability.

---

# 15. References


1. **W3C Web Accessibility Initiative — Web Content Accessibility Guidelines (WCAG) 2.2**
   [W3C — WCAG 2.2](https://www.w3.org/TR/WCAG22/?utm_source=chatgpt.com)

2. **W3C Web Accessibility Initiative — Understanding Text Spacing**
   [W3C — Understanding SC 1.4.12: Text Spacing](https://www.w3.org/WAI/WCAG22/Understanding/text-spacing.html?utm_source=chatgpt.com)

3. **W3C Web Accessibility Initiative — Understanding Visual Presentation**
   [W3C — Understanding SC 1.4.8: Visual Presentation](https://www.w3.org/WAI/WCAG22/Understanding/visual-presentation.html?utm_source=chatgpt.com)

4. **Microsoft Learn — OpenType Font Variations Overview**
   [Microsoft — OpenType Font Variations Overview](https://learn.microsoft.com/en-us/typography/opentype/spec/otvaroverview?utm_source=chatgpt.com)

5. **Microsoft Learn — OpenType Font Variations Table**
   [Microsoft — OpenType fvar Table](https://learn.microsoft.com/en-us/typography/opentype/otspec181/fvar?utm_source=chatgpt.com)

6. **UXDT — Typography Guidelines**
   [UXDT — Typography Guidelines](https://www.uxdt.nic.in/guidelines/design-system-overview/typography/?utm_source=chatgpt.com)

