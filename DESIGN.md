---
name: Ahmad Baabod Portfolio
description: A software and AI portfolio developed like a carefully printed body of work.
colors:
  darkroom: "#211911"
  darkroom-deep: "#17120e"
  tray: "#30251b"
  safelight-amber: "#e6a14a"
  amber-light: "#f1bd72"
  print-paper: "#eee8dc"
  silver-print: "#c9c7c0"
  silver-dark: "#89877f"
  print-ink: "#211d18"
  caption-muted: "#c2b9ab"
typography:
  display:
    fontFamily: "Barlow Condensed, Impact, sans-serif"
    fontSize: "clamp(4.6rem, 8vw, 6rem)"
    fontWeight: 600
    lineHeight: 0.83
    letterSpacing: "-0.025em"
  headline:
    fontFamily: "Barlow Condensed, Impact, sans-serif"
    fontSize: "clamp(3rem, 6vw, 5.3rem)"
    fontWeight: 600
    lineHeight: 0.94
  body:
    fontFamily: "Source Sans 3, Segoe UI, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Source Sans 3, Segoe UI, sans-serif"
    fontSize: "0.8rem"
    fontWeight: 700
    letterSpacing: "0.15em"
spacing:
  sm: "0.5rem"
  md: "1rem"
  lg: "1.5rem"
  xl: "2.5rem"
components:
  button-primary:
    backgroundColor: "{colors.safelight-amber}"
    textColor: "{colors.print-ink}"
    padding: "0.7rem 1.2rem"
    height: "48px"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.print-paper}"
    padding: "0.7rem 1.2rem"
    height: "48px"
  print-mat:
    backgroundColor: "{colors.print-paper}"
    padding: "14px 14px 52px"
  project-tag:
    backgroundColor: "transparent"
    textColor: "#e1d8ca"
    padding: "0.25rem 0.55rem"
---

# Design System: Ahmad Baabod Portfolio

## Overview

**Creative North Star: "The Developer's Darkroom"**

The portfolio treats experience as a body of work brought into view one print at a time. Safelight amber warms a deep brown workroom; silver-gray type, paper-colored fields, enamel edges, and restrained grease-pencil captions carry information with a tactile photographic character.

The visual language is confident and precise, with the work itself kept legible. Project descriptions and credentials stay factual, navigation remains direct, and the large display lettering provides the main expressive gesture.

**Key Characteristics:**
- Amber light against deep brown, with paper and silver-print neutrals.
- Condensed uppercase display headlines paired with clear humanist body copy.
- Print mats, contact-sheet rows, and workbench-like dividers create structure.
- Square-edged controls and simple underlined links favor directness.

## Colors

The palette pairs safelight amber with darkroom browns and the pale tones of photographic paper and silver prints.

### Primary
- **Safelight Amber** (#e6a14a): Main action, availability indicators, and selected emphasis.
- **Amber Light** (#f1bd72): Secondary emphasis and links on dark surfaces.

### Secondary
- **Enamel Tray** (#30251b): Project feature and secondary work surfaces.

### Tertiary
- **Silver Print** (#c9c7c0): Secondary print-like detail and supporting visual treatments.

### Neutral
- **Darkroom Brown** (#211911): Main page background.
- **Deep Darkroom** (#17120e): Header and quiet dark section background.
- **Print Paper** (#eee8dc): Light sections, primary text, and portrait mat.
- **Print Ink** (#211d18): Text and foreground action text on light surfaces.
- **Caption Muted** (#c2b9ab): Supporting text on dark backgrounds.
- **Silver Shadow** (#89877f): Secondary neutral for print detail.

### Named Rules
**The Legible Print Rule.** Amber may mark emphasis, but body copy and supporting project details remain high-contrast and easy to scan.

## Typography

**Display Font:** Barlow Condensed (with Impact, sans-serif fallback)

**Body Font:** Source Sans 3 (with Segoe UI, sans-serif fallback)

**Label/Mono Font:** Source Sans 3; uppercase and letter spacing distinguish labels.

**Character:** Barlow Condensed gives names and section headings the tall, press-room quality of darkroom labels. Source Sans 3 keeps longer descriptions open, legible, and practical.

### Hierarchy
- **Display** (600, `clamp(4.6rem, 8vw, 6rem)`, 0.83 line-height): Main name in the first viewport.
- **Headline** (600, `clamp(3rem, 6vw, 5.3rem)`, 0.94 line-height): Section headings.
- **Title** (600, project title about 1.8rem–3.25rem): Project and course titles.
- **Body** (400, 17px, 1.55 line-height): Descriptions and explanatory copy, constrained by readable container widths.
- **Label** (700, 0.8rem, 0.15em tracking, uppercase): Project categories and short station labels.

### Named Rules
**The Caption and Print Rule.** Reserve uppercase condensed lettering for identity and labels; set explanations in the body face.

## Layout

Use a centered content frame capped at 1160px with fluid side gutters. The desktop introduction places copy and portrait print side-by-side; narrow layouts stack the portrait after the introduction and keep section navigation horizontally scrollable. Projects use one prominent featured print followed by ruled, content-led rows. Light and dark sections alternate to pace long-form browsing. At 760px and below, the page moves to one column and skill entries use a two-column ledger.

## Elevation & Depth

Depth is mostly tonal: deep room backgrounds, lighter trays, paper fields, and fine dividers establish the workspace. A soft offset shadow belongs to the physical portrait mat and featured print only. Avoid decorative glow and glass effects.

### Shadow Vocabulary
- **Portrait print:** `0 28px 80px rgba(0, 0, 0, .35)` gives the portrait mat a lifted photographic-paper edge.
- **Academic print:** `0 14px 32px rgba(33, 29, 24, .08)` separates the academic paper surface from the light field.

## Shapes

The system is predominantly square-edged. Controls, dividers, project rows, and paper surfaces use straight edges; the portrait mat is a clean rectangular print with an inset border. Prefer thin rules and paper framing over rounded card shells.

## Components

### Buttons
- **Shape:** Square corners.
- **Primary:** Safelight amber background with print-ink text; 0.7rem 1.2rem padding and 48px minimum height.
- **Hover / Focus:** Amber light on hover with a 2px upward shift; keyboard focus uses a 3px amber-light outline offset by 4px.
- **Secondary:** Transparent background, paper text, and a fine divider-colored border; tray background on hover.

### Chips
- **Style:** Transparent, square-edged tags with pale text and a thin print-colored outline.
- **State:** Static project and skill descriptors, not faux interactive filters.

### Cards / Containers
- **Corner Style:** Square corners.
- **Background:** Dark tray surfaces for featured work; print paper for academic detail.
- **Shadow Strategy:** Reserve offset, soft shadows for the portrait mat and light academic print; structure other sections with color and rules.
- **Border:** Fine neutral dividers.
- **Internal Padding:** 1.5rem for compact paper surfaces; featured project padding scales from 1.5rem to 3.2rem.

### Navigation
- **Style:** A compact sticky station index with plain text links. Links are muted at rest and amber-light on hover. At narrow sizes the station list scrolls horizontally rather than disappearing.

### Portrait Print
- A rectangular paper mat with an inset hairline, silver-toned portrait image, and a caption along the print edge; preserve the real portrait as the hero image.

### Project Record
- A ruled text-led record introduces the lead project, without implying a screenshot exists; subsequent projects use variable-height rows with type, truthful summary, technology tags, and a direct repository link.

## Do's and Don'ts

### Do:
- **Do** use the amber, paper, silver, and darkroom-brown palette consistently across light and dark sections.
- **Do** make the actual project, course, and certificate information the focus of each section.
- **Do** preserve clear keyboard focus and the mobile horizontal station index.
- **Do** use display lettering for short headlines and readable body text for longer copy.

### Don't:
- **Don't** use amber for long body passages or low-contrast labels.
- **Don't** wrap every section in an identical rounded card.
- **Don't** substitute glowing gradients, glass, or decorative motion for photographic-paper framing and tonal layers.
- **Don't** imply credentials, project outcomes, or language proficiency beyond the confirmed source material.
