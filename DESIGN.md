---
name: Handled
description: Personal assistant services, Central Oregon — Your Extra Hand
colors:
  cream: "#f5f2ed"
  cream-2: "#faf8f4"
  paper: "#ffffff"
  ink: "#1a1a1a"
  ink-soft: "#3a3a3a"
  red: "#9b1b2e"
  red-bright: "#b9223a"
  gray: "#6b6b6b"
  line: "#e4ded3"
typography:
  display:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "clamp(2rem, 4.4vw, 3rem)"
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "clamp(2rem, 4.4vw, 3rem)"
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "1.2rem"
    fontWeight: 700
    lineHeight: 1.2
  body:
    fontFamily: "Inter, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "Archivo, system-ui, sans-serif"
    fontSize: "0.76rem"
    fontWeight: 600
    letterSpacing: "0.26em"
rounded:
  sm: "12px"
  md: "18px"
  lg: "26px"
  input: "10px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "26px"
  lg: "48px"
  section: "clamp(3.8rem, 7vw, 6rem)"
components:
  button-red:
    backgroundColor: "{colors.red}"
    textColor: "{colors.paper}"
    rounded: "{rounded.sm}"
    padding: "0.9rem 1.7rem"
  button-red-hover:
    backgroundColor: "{colors.red-bright}"
  button-dark:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    rounded: "{rounded.sm}"
    padding: "0.9rem 1.7rem"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "0.9rem 1.7rem"
  card-service:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: "1.7rem"
---

# Design System: Handled

## Overview

**Creative North Star: "Your Extra Hand"**

Handled is the person who actually shows up. The visual system is confident and personal — a cream-warm ground that feels like a home, not an office, with Archivo's heavy extrabold weight cutting through instantly in the hero. The red accent is precise and purposeful: it marks what matters and then stops. This isn't a loud design. It's the quiet confidence of someone who knows exactly what they're doing and doesn't need to announce it.

The hero wordmark is the system's signature moment: the Yellowtail script "Handled." at display size, with a deep red underline that draws itself into view over one second. It establishes personality first — the rest of the page earns trust through clear copy and warm cream-to-paper surfaces. The full-width ink pillars strip mid-page is the tonal pivot: from warmth to confident authority, before returning to warmth in the about and family sections.

Motion is direct and quick (700ms, 80ms stagger). This brand acts; it doesn't perform.

**Key Characteristics:**
- Yellowtail script wordmark with animated red underline — the personality in the first viewport
- Cream-warm ground throughout — a home, not a showroom
- Archivo extrabold (800) for all headings — strong, no hedging
- Red is the accent only: buttons, eyebrow rules, hover states, the `.dot-red` period
- Full-width ink pillars strip as the confident mid-page tonal break

## Colors

Cream and near-black, punctuated by a single deep-red accent.

### Primary
- **Handled Red** (`#9b1b2e`): Primary buttons, 26px eyebrow rule bar, nav hover underline, `.dot-red` accent period, service icon chip hover fill, CTA radial glow source.
- **Bright Red** (`#b9223a`): Button hover state, floating badge accent fill. Full intensity version of the accent.

### Neutral
- **Warm Cream** (`#f5f2ed`): Page background. A home's warmth — not a showroom's white.
- **Soft Cream** (`#faf8f4`): Section alternates, about section, hero radial gradient base.
- **Paper** (`#ffffff`): Card surfaces, form fields, hero card.
- **Deep Ink** (`#1a1a1a`): All headings and primary body text. Near-black, no tint — direct and confident.
- **Soft Ink** (`#3a3a3a`): Lead paragraphs, about section prose. One tone lighter than headline ink.
- **Gray** (`#6b6b6b`): Card descriptors, supporting text, footer links.
- **Warm Line** (`#e4ded3`): All borders and dividers. Slightly warm beige.

### Named Rules
**The Red Precision Rule.** Red appears on primary interactive elements and the single `.dot-red` period at the end of the brand name in headings. It is never a section background, never a tint, never appearing in more than one role per viewport simultaneously. Its scarcity is the point.

## Typography

**Display Font:** Archivo (system-ui fallback) at weight 800
**Body Font:** Inter (system-ui fallback)
**Script Accent:** Yellowtail — hero wordmark and `.sign` handwritten sign-off only

**Character:** Archivo at 800 is as direct as the brand — no serifs, no indirection, just confident weight. Inter softens the follow-through at body size, making the page readable without demanding attention. Yellowtail appears only as the large script wordmark in the hero and the handwritten sign-off in the about section, establishing personal warmth without softening the system's authority.

### Hierarchy
- **Script Display:** Yellowtail, clamp 3.6–6.6rem, lh 0.9 — the hero wordmark "Handled." with red animated underline. One instance, hero only.
- **Display** (800, clamp 2–3rem, lh 1.05, ls –0.01em): Section h2 and CTA h2. Archivo extrabold.
- **Title** (700, 1.2rem, lh 1.2, ls 0.12em, uppercase): Hero `.h1.sub` subtitle text.
- **Body** (400, 1rem, lh 1.7): Inter. Soft Ink for prose paragraphs; gray for card descriptors.
- **Label** (600, 0.76rem, ls 0.26em, uppercase, red): Eyebrow text. Always preceded by a 26px×2px red horizontal bar.

### Named Rules
**The Wordmark Rule.** The Yellowtail "Handled." with its red underline animation appears only in the homepage hero. No other page uses the large script wordmark. The `.sign` in the about section uses Yellowtail at 2rem as a sign-off only.

## Layout

Container max-width 1160px, 26px padding. Hero: two-column grid (1.08fr / 0.92fr), copy left, visual right. At 920px visual comes first (order: -1). Section padding: `clamp(3.8rem, 7vw, 6rem)`. Pillars strip: four-column grid on full-width ink background (two at 920px, one at 600px). Services and family grids: three-column (two at 920px, one at 600px). About: reversed grid (0.9fr / 1.1fr, photo left). Form: 1.1fr / 0.9fr. Scroll-reveal: 700ms ease, 24px translateY, 80ms stagger.

Breakpoints: 920px (tablet — hero stacks, grids collapse), 600px (mobile — hamburger, single column).

## Elevation & Depth

Three neutral-dark shadows for hierarchy. All shadows use `rgba(26,26,26,...)` — the same ink as the headings, so depth feels like weight rather than atmosphere.

### Shadow Vocabulary
- **Surface** (`0 2px 10px rgba(26,26,26,.06)`): Hover warm-up on value cards.
- **Lifted** (`0 16px 40px rgba(26,26,26,.10)`): Form card, service cards on hover, value cards on interior pages.
- **Floating** (`0 30px 70px rgba(26,26,26,.16)`): Hero card at rest. One per page view.

## Shapes

Confidently rounded: small 12px, medium 18px, large 26px. Buttons use 8px radius — not the flagship's pill, not the catering brands' near-square. The 8px radius is the Handled signature: approachable but defined. Input fields use 10px (slightly more relaxed than buttons). Hero card: 26px radius, a warm container for the portrait. Badge floats: 14px radius on ink or red backgrounds. No pill-shaped interactive elements.

## Components

### Buttons
- **Shape:** 8px radius, Archivo 600, 0.92rem, ls 0.02em
- **Red Primary:** Handled Red (`#9b1b2e`) background, white text, 2px transparent border, 0.9rem×1.7rem padding, red shadow lift
- **Hover:** Bright Red background, –3px translateY, deeper shadow
- **Dark:** Deep Ink background, white text, same 8px radius
- **Ghost:** Transparent, 20%-ink border → red border and red text on hover; same 8px radius

### Cards / Containers
- **Service Card:** Paper white, 1px warm-line border, 18px radius, 1.7rem padding. Icon chip: 50px, 12px radius, cream background, red icon at rest → red background with white icon on hover (background and color transition).
- **Hero Card:** Paper white, 1px warm-line border, 26px radius, Floating shadow at rest, 1.3rem padding.
- **Badge Floats:** Ink background "Trusted" (top-left, 14px radius), Red "Elevated" (bottom-right, 14px radius). Archivo 700 white, red-bright icon.
- **CTA Block:** Ink background, 26px radius, red radial glow (`rgba(155,27,46,.25)`) at the top-center; no border.

### Pillars Strip (Signature Component)
Four-column grid spanning full viewport width on the ink background. Each pillar: 46px red-bright icon (centered), Archivo 800 uppercase heading with `.dot-red` period, Inter body in muted cream (62% opacity). Hover: icon translates up 4px (300ms). The strip is the darkest surface in the system outside the CTA block and the mid-page confidence anchor.

### Navigation
- **Style:** Frosted cream glass (85% warm-cream, 12px blur), 78px height, 1px warm-line bottom border
- **Links:** Archivo 500, 0.92rem, soft-ink → ink on hover; 2px red underline draws left-to-right
- **Logo:** Yellowtail script 1.7rem, ink
- **Mobile:** Hamburger at 600px

### Inputs / Fields
- **Style:** Cream-2 background, 1px warm-line border, 10px radius
- **Focus:** Red border, 3px red glow (`rgba(155,27,46,.13)`), white background
- **Label:** Archivo 600, 0.86rem, ink color (not red — labels are structural, not accented)

## Do's and Don'ts

### Do:
- **Do** animate the red underline on the hero wordmark on every homepage load — it's the brand's most memorable moment.
- **Do** use the ink pillars strip once per page to create the mid-page confident tonal break.
- **Do** let the service icon chip fill with red on hover — the color swap signals precision and care.
- **Do** append `.dot-red` (the red period) after "Handled" whenever it appears as a heading inside the site.
- **Do** use Archivo 800 for every h2 and h3 — no weight variation across headings.

### Don't:
- **Don't** use Yellowtail as a heading font. It appears only as the hero wordmark and the about section `.sign` sign-off.
- **Don't** use red as a section background or surface tint. Red is a point-light accent, never a surface.
- **Don't** use pill-shaped buttons — 8px radius is the Handled signature.
- **Don't** add the wordmark underline animation on interior page heroes — that animation belongs to the homepage only.
- **Don't** use gray for prose paragraphs — use soft-ink (`#3a3a3a`). Gray is for card descriptors and supporting text only.
