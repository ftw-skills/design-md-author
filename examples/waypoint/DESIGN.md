---
version: alpha
name: Waypoint
description: A field-note page for preparing a short waterfront walk.
colors:
  primary: "#245c48"
  on-primary: "#ffffff"
  paper: "#f7f5ee"
  surface: "#ffffff"
  ink: "#24342d"
  muted: "#52655d"
  outline: "#bac5be"
typography:
  headline-display:
    fontFamily: Georgia
    fontSize: 48px
    fontWeight: 700
    lineHeight: 1.12
  headline-md:
    fontFamily: Georgia
    fontSize: 24px
    fontWeight: 700
    lineHeight: 1.2
  body-md:
    fontFamily: Arial
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.55
rounded:
  control: 8px
  card: 12px
spacing:
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
components:
  page:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
  helper-text:
    textColor: "{colors.muted}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.control}"
    height: 44px
  button-secondary:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.primary}"
    rounded: "{rounded.control}"
    height: 44px
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "{spacing.lg}"
---

## Overview

Waypoint lets walkers find tide and route notes quickly. A quiet paper background and a compact hierarchy make the directions easy to scan.

## Colors

Use dark ink for headings and notes. Use muted green-gray text on paper for introductory and footer copy. Reserve filled green for the main action. Use the same green for the outline, text, and focus indicator of secondary actions. Outline white cards with the subdued border color.

## Typography

Use Georgia for page and note headings. The page title is 48px on desktop and 36px at widths up to 680px. Set note headings at 24px and use Arial at 16px for body copy and actions.

## Layout

Keep page content within 960px and introductory text within 640px. Give the desktop content 40px of padding, with two equal note columns and a 16px gap. At widths up to 680px, use 24px of page padding and stack the notes in source order. Allow actions to wrap when space runs out.

## Elevation & Depth

Use white note surfaces and a thin border to separate notes from the paper background. Keep the panels flat.

## Shapes

Use an 8px radius for interactive controls and a 12px radius for note cards.

## Components

### Actions

Use one filled link for the page's main action. Place the outlined conditions link beside it as a secondary action. Keep both hit areas at least 44px high. Underline the label on hover. On keyboard focus, use a 2px green outline with a 3px offset.

### Note cards

Put tide information first and route information second. Each card has a short heading and one paragraph. Give both cards the same inner padding to keep their contents aligned.

## Do's and Don'ts

- Keep essential route details in the note itself so they remain visible without opening another control.
- Avoid using a second filled action in the introduction.