---
name: Nishanth Kesavan
description: A precise, useful working studio for practical digital products.
colors:
  signal-cobalt: "oklch(47% 0.24 264)"
  signal-cobalt-deep: "oklch(40% 0.22 264)"
  working-paper: "oklch(97.5% 0.004 250)"
  white: "oklch(100% 0 0)"
  engineering-ink: "oklch(20% 0.035 250)"
  graphite: "oklch(40% 0.03 250)"
  highlighter-lime: "oklch(92% 0.2 116)"
  rule-line: "oklch(68% 0.025 250)"
typography:
  display:
    fontFamily: "Bricolage Grotesque, Arial Narrow, sans-serif"
    fontSize: "clamp(3.25rem, 8vw, 6rem)"
    fontWeight: 750
    lineHeight: 0.98
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "Bricolage Grotesque, Arial Narrow, sans-serif"
    fontSize: "clamp(2rem, 4vw, 3.5rem)"
    fontWeight: 720
    lineHeight: 1.03
  body:
    fontFamily: "Atkinson Hyperlegible Next, Segoe UI, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "Atkinson Hyperlegible Next, Segoe UI, sans-serif"
    fontSize: "0.8rem"
    fontWeight: 700
    letterSpacing: "0.035em"
rounded:
  sm: "4px"
  md: "8px"
  lg: "14px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
components:
  button-primary:
    backgroundColor: "{colors.signal-cobalt}"
    textColor: "{colors.white}"
    rounded: "{rounded.sm}"
    padding: "12px 20px"
  button-highlight:
    backgroundColor: "{colors.highlighter-lime}"
    textColor: "{colors.engineering-ink}"
    rounded: "{rounded.sm}"
    padding: "12px 20px"
  project-mark:
    backgroundColor: "{colors.signal-cobalt}"
    textColor: "{colors.white}"
    rounded: "{rounded.sm}"
    size: "54px"
---

# Design System: Nishanth Kesavan

## Overview

**Creative North Star: "The Builder's Field Kit"**

The site should feel like a well-used kit assembled by someone who understands the job: a clean working surface, clear labels, bright markers, and no ornamental parts. It is expressive through decisive scale and color, but every visual move still has a practical role.

The system is resourceful, precise, and dependable. It rejects generic dark developer portfolios, neon gradients, floating blobs, glass cards, emoji placeholders, generic card grids, startup slogans, inflated expertise claims, and copy that hides the role of AI.

**Key Characteristics:**

- High-contrast cobalt and lime used as confident working colors.
- Large, compressed display type paired with a highly legible body face.
- Ruled lists and asymmetric compositions in place of repetitive cards.
- Personal details presented as evidence, not decoration.
- Responsive layouts that become linear and calm on small screens.

## Colors

The palette takes its cues from engineering labels and highlighter marks, with a cool neutral surface rather than a warm paper effect.

### Primary

- **Signal Cobalt:** Carries the home and project heroes, primary actions, links, and active navigation states.
- **Deep Cobalt:** Used only for hover states that need a clear shift in depth.

### Secondary

- **Highlighter Lime:** Marks the portrait frame, hero action, status dots, selection, and important metadata. It always sits behind engineering ink or against cobalt.

### Neutral

- **Working Paper:** The main page surface. It is cool and nearly neutral, never beige.
- **White:** Used for clean content surfaces and inverse type.
- **Engineering Ink:** The default heading and dark-section color.
- **Graphite:** Body copy and secondary navigation.
- **Rule Line:** Structural dividers between projects and timeline entries.

**The Marker Rule.** Lime marks a decision or a live status. It is never used as ambient decoration.

**The No Gradient Rule.** All colors are solid. Gradients are prohibited throughout the interface.

## Typography

**Display Font:** Bricolage Grotesque (with Arial Narrow fallback)  
**Body Font:** Atkinson Hyperlegible Next (with Segoe UI fallback)

**Character:** Bricolage has enough oddness to feel personal while retaining a compact, engineered silhouette. Atkinson keeps long case-study copy easy to read and makes the site's accessibility visible through craft rather than claims.

### Hierarchy

- **Display** (750, fluid up to 6rem, 0.98): Home hero statements only.
- **Headline** (720, fluid up to 3.5rem, 1.03): Page and section headings.
- **Title** (720, fluid up to 2rem, 1.08): Project names and timeline roles.
- **Body** (400, 1.05rem, 1.55): Main copy, capped at roughly 65 characters where practical.
- **Label** (700, 0.8rem, 0.035em): Status and metadata. Sentence case by default.

**The One Loud Sentence Rule.** Every viewport may have one dominant typographic idea. Supporting text stays deliberately quieter.

## Elevation

The system is flat by default. Depth comes from surface color, rules, and overlap. The portrait is the one exception: an 8px hard offset shadow makes it feel like a physical print set on the page.

### Shadow Vocabulary

- **Portrait offset** (`8px 8px 0 engineering-ink`): Used only on the personal portrait.
- **Compact lift** (`0 3px 8px`): Reserved for small controls when state cannot be made clear through color alone.

**The Flat-By-Default Rule.** Cards and sections do not float. If a surface has both a visible border and a soft shadow, the treatment is wrong.

## Components

### Buttons

- **Shape:** Tight utility corners (4px), never pills.
- **Primary:** Signal cobalt with white text; lime with ink on cobalt or ink backgrounds.
- **Hover / Focus:** A 2px vertical lift on hover and a 3px lime focus ring with 4px offset.
- **Secondary:** Transparent with a 2px current-color outline; fills with ink on hover.

### Chips

- **Style:** Cool gray fill, graphite text, 4px corners, and compact padding.
- **State:** They describe technology or context and are never interactive-looking unless they really are controls.

### Cards / Containers

- **Corner Style:** 8px maximum for ordinary surfaces; project rows remain square and ruled.
- **Background:** White for contained CV groups, working paper for the main surface.
- **Shadow Strategy:** None at rest.
- **Border:** A 3px top rule may identify a skill group; project rows use full-width 1px dividers.
- **Internal Padding:** 24px on compact surfaces.

### Navigation

The navigation uses a compact cobalt monogram, plain-language links, and a single cobalt underline for the active route. On phones it becomes a full dark panel with large links and a visible lime close control.

### Work Index

Each project is a full-width ruled row with a two-letter mark, current status, concise evidence, technology tags, and a circular outbound arrow. Hovering commits the entire row to its own project color.

## Do's and Don'ts

### Do:

- **Do** use signal cobalt for decisive surfaces and highlighter lime for actions or live status.
- **Do** keep body copy within 65 to 75 characters per line.
- **Do** let project facts and maintained status provide credibility.
- **Do** use asymmetric spacing and full-width ruled lists to keep the composition human.
- **Do** respect reduced-motion settings and preserve visible content without JavaScript.

### Don't:

- **Don't** create generic dark developer portfolios, neon gradients, floating blobs, or glass cards.
- **Don't** use emoji placeholders, generic card grids, startup slogans, or inflated expertise claims.
- **Don't** hide the role of AI in the work or turn it into a novelty badge.
- **Don't** use gradient text, rounded cards over 14px, or repeated uppercase section eyebrows.
- **Don't** pair a 1px border with a wide soft shadow on the same component.
