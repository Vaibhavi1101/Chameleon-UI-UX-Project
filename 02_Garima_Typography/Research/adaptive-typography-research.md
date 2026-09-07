# Adaptive Typography Research

## 1. Introduction

Typography is an important part of an accessible user interface because the way text is presented affects how easily users can read and understand content.

**Adaptive Typography** is an approach in which typography properties can be adjusted according to different user needs, contexts, or display conditions.

For the **Chameleon — Algorithmic Accessibility Engine** project, Adaptive Typography is being researched as a way to create a flexible and accessible typography system.

---

## 2. What is Adaptive Typography?

Adaptive Typography refers to typography that can change its properties to support different readability requirements.

The main properties that can be adapted are:

| Typography Property | Purpose                                                     |
| ------------------- | ----------------------------------------------------------- |
| Font Size           | Controls how large or small text appears                    |
| Font Weight         | Controls the thickness of characters                        |
| Font Width          | Controls how condensed or expanded text appears             |
| Line Height         | Controls vertical space between lines                       |
| Letter Spacing      | Controls space between individual characters                |
| Word Spacing        | Controls space between words                                |
| Optical Size        | Adjusts type design for different text sizes when supported |

These properties can be adjusted individually or in combination depending on the requirements of the interface.

---

## 3. Accessibility and Readability

Accessible typography should allow users to read and interact with content without unnecessary difficulty.

WCAG includes requirements related to adaptable text presentation.

### Text Resizing

**WCAG 1.4.4 — Resize Text** requires that text can be resized up to **200%** without loss of content or functionality, with exceptions for certain captions and images of text.

### Text Spacing

**WCAG 1.4.12 — Text Spacing** specifies that content should remain usable when users increase text spacing to at least the following values:

| Property          | Minimum Requirement |
| ----------------- | ------------------: |
| Line Height       |     1.5 × font size |
| Paragraph Spacing |       2 × font size |
| Letter Spacing    |    0.12 × font size |
| Word Spacing      |    0.16 × font size |

These requirements demonstrate the importance of designing interfaces that can accommodate changes in text size and spacing.

---

## 4. Variable Typography

**Variable fonts** are fonts that can contain a range of variations within a single font file.

Instead of using separate font files for every variation, supported properties can be adjusted along defined axes.

This makes variable fonts useful for flexible typography systems.

### Important Variable Font Axes

| Axis   | Name         | Purpose                                                      |
| ------ | ------------ | ------------------------------------------------------------ |
| `wght` | Weight       | Controls the thickness of the typeface                       |
| `wdth` | Width        | Controls how condensed or expanded the typeface appears      |
| `opsz` | Optical Size | Allows the typeface to be optimized for different text sizes |
| `slnt` | Slant        | Controls the slant of the typeface                           |

**Note:** Not every variable font supports all of these axes. The available axes depend on the particular typeface.

---

## 5. Why Variable Fonts are Useful

Variable fonts provide more flexibility than using only fixed font styles.

They can allow a typography system to:

* Adjust weight within the range supported by the font.
* Adjust width when different text widths are required.
* Use optical sizing when supported.
* Reduce the need for multiple separate font files.
* Provide more control when creating responsive or adaptive typography.

---

## 6. Key Typography Parameters

The following parameters are important when designing an adaptive typography system:

| Parameter      | Design / Accessibility Purpose                                |
| -------------- | ------------------------------------------------------------- |
| Font Size      | Supports different viewing and readability needs              |
| Font Weight    | Provides appropriate text thickness and hierarchy             |
| Font Width     | Controls the horizontal space occupied by text                |
| Line Height    | Provides sufficient vertical space between lines              |
| Letter Spacing | Controls spacing between characters                           |
| Word Spacing   | Controls spacing between words                                |
| Optical Size   | Optimizes type design for different text sizes when available |

These parameters should be considered together rather than changing only one property in isolation.

---

## 7. Relevance to Chameleon

The Chameleon project explores an adaptive accessibility system rather than relying only on fixed typography settings.

For the **Adaptive Typography** module, the research focuses on how typography properties can be controlled and combined to support different readability needs.

Variable font technology is particularly relevant because properties such as **weight, width, and optical size** can provide additional flexibility when supported by the selected font.

This research will provide the foundation for defining typography rules and building the typography system in the next stages of the project.

---

## 8. Key Findings

1. Typography is an important part of an accessible user interface.
2. Text size and spacing should be able to accommodate different readability needs.
3. WCAG provides specific requirements for text resizing and text spacing.
4. Variable fonts can provide multiple typographic variations within a single font file.
5. Important variable font axes include **weight, width, optical size, and slant**, when supported by the font.
6. Adaptive Typography can provide a flexible foundation for creating interfaces that accommodate different readability requirements.

