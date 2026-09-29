---
name: Pavan & Pooja — Moonlit Celebration
description: A midnight-teal wedding invitation with editorial typography and luminous arched imagery.
colors:
  night: "#102c31"
  deep: "#092126"
  surface: "#17383d"
  paper: "#f4efdf"
  rose: "#e5b7ad"
  muted: "#b4c7c6"
  line: "#416065"
typography:
  display:
    fontFamily: '"Bodoni Moda", "Times New Roman", serif'
    fontSize: "clamp(60px, 7.8vw, 96px)"
    fontWeight: 400
    lineHeight: 0.94
    letterSpacing: "-0.03em"
  headline:
    fontFamily: '"Bodoni Moda", "Times New Roman", serif'
    fontSize: "clamp(34px, 4.7vw, 62px)"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "-0.025em"
  body:
    fontFamily: '"Manrope", Arial, sans-serif'
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: '"Manrope", Arial, sans-serif'
    fontSize: "12px"
    fontWeight: 400
  blessing:
    fontFamily: '"Noto Serif Devanagari", serif'
    fontSize: "14px"
    fontWeight: 400
rounded:
  action: "8px"
  media: "12px"
  sound: "28px"
  seal: "50%"
  hero-arch: "48% 48% 12px 12px"
spacing:
  compact: "12px"
  inset: "20px"
  mobile-gutter: "24px"
  section-gutter: "max(24px, 8vw)"
components:
  button-primary:
    backgroundColor: "{colors.rose}"
    textColor: "{colors.deep}"
    rounded: "{rounded.action}"
    padding: "12px 22px"
  text-link:
    textColor: "{colors.rose}"
    typography: "{typography.label}"
  event-row:
    textColor: "{colors.paper}"
    padding: "30px 0"
  countdown:
    backgroundColor: "{colors.rose}"
    textColor: "{colors.deep}"
    padding: "70px max(24px, 8vw)"
  portal-action:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.paper}"
    rounded: "{rounded.action}"
    padding: "15px 20px"
---

# Design System: Pavan & Pooja

## Overview

**Creative North Star: "Moonlit Celebration"**

The implemented evening world pairs midnight teal with warm moonwhite lettering and blush accents. Editorial type, open programme rows and framed origami imagery make the invitation intimate and ceremonial without obscuring practical details.

**Key Characteristics:**

- Dark, tonal surfaces with one contrasting countdown band.
- Expressive serif names beside quiet, legible sans-serif information.
- Arched imagery and a glowing doorway as recurring signatures.

This records the invitation in `index.html` and `styles.css`; it does not prescribe a redesign of the separate wedding-world route.

## Colors

### Primary

Rose is the warm accent for actions, dates, italic emphasis and the countdown surface.

### Neutral

Night is the main canvas; deep distinguishes cinematic passages and the finale. Surface lifts small controls. Paper carries primary text, muted carries supporting copy, and line separates navigation and programme rows.

**The Evening Rule.** Keep the invitation's midnight-teal foundation; the earlier burgundy/gold and Comic Sans glass treatment is superseded.

## Typography

Bodoni Moda supplies names, headings, day numbers and countdown numerals; Manrope supplies navigation, times, descriptions and actions. Noto Serif Devanagari preserves the blessing's script. Font stacks and base sizes live in the frontmatter.

Names use tightly tracked display type; italic blush words provide selective emphasis. Event titles scale from 26px to 35px, while descriptions use 14px. Labels are generally 12px; uppercase tracking is reserved for date and countdown labels. Tabular numerals stabilize times and the countdown.

## Layout

The desktop hero uses a 1:1.1 split grid, a 7% gap and a 1280px maximum width: invitation text on the left, arched illustration on the right. Programme content reaches 1440px; film, venue and gateway compositions share a 1120px maximum. Sections use generous vertical spacing and fluid side gutters.

At 800px and below, the countdown stacks and programme columns narrow. At 580px and below, the hero stacks with centered names above its illustration, day headings sit above open event rows, venue copy precedes imagery, and the gateway centers. Mobile content generally uses 24px gutters (22px in the hero). Keep the countdown separate from the hero and retain the two-day programme hierarchy.

## Elevation & Depth

Depth comes primarily from tonal backgrounds, fine borders and inset image frames, not floating cards or decorative blur. The portal alone has a warm ambient glow; the fixed music control has a small practical shadow. Exact shadow values live in the sidecar.

## Shapes

Soft rectangular actions and media frames coexist with ceremonial arches. The hero arch and narrower sanctum arch echo the glowing doorway. The opening seal is circular; the music control is pill-shaped on desktop and compact on mobile. Programme entries remain unboxed, separated by fine rules.

## Components

- **Navigation:** serif monogram, understated date and a 44px-minimum celebration link; hide the date at the intermediate breakpoint.
- **Actions:** blush-filled directions button and underlined text link; arrows move 4px on hover. Keyboard focus uses a 2px blush outline with a 6px offset.
- **Programme rows:** time, serif event name, supporting description and optional icon; the icon disappears below 800px. Preserve the two day groups.
- **Countdown:** blush band, deep text, four evenly spaced numeral/label cells; stack its introduction above the numbers on smaller screens.
- **Portal:** arched golden light above an outlined action and explicit tap cue. It links to the separate wedding world; it is not a decorative dead end.
- **Motion:** restrained entrance, door-opening and portal animations. Honor reduced motion by disabling CSS animations/transitions, removing petals and showing a static sanctum poster.

## Do's and Don'ts

### Do:

- Do preserve the evening palette, serif/sans hierarchy and arched image language.
- Do keep programme text, keyboard focus and touch targets clear on mobile.
- Do respect reduced-motion preferences and retain usable media controls.

### Don't:

- Don't restore the superseded burgundy/gold or Comic Sans glass styling.
- Don't turn the open programme into a grid of elevated cards.
- Don't spread portal glow, blur or ornamental animation across ordinary content.
