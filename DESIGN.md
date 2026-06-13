---
name: Ceremonial Tea Name Generator
description: A dark-lacquer-and-gold novelty generator that issues absurd "ceremonial grade" green-tea names with a straight face.
colors:
  bg: "#0b0d08"
  bg2: "#15160f"
  card: "#191b12"
  gold: "#e0bd6f"
  gold-dim: "#ab8e50"
  title-gold: "#eccf85"
  jade: "#7fd3a0"
  jade-deep: "#356f53"
  text: "#f1efe6"
  text-dim: "#a8a596"
  text-faint: "#6b6757"
  danger: "#e07a5a"
typography:
  display:
    fontFamily: "Noto Sans Thai, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif"
    fontSize: "27px"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "0.5px"
  headline:
    fontFamily: "Noto Sans Thai, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif"
    fontSize: "19px"
    fontWeight: 600
    lineHeight: 1.45
    letterSpacing: "normal"
  body:
    fontFamily: "Noto Sans Thai, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "normal"
  label:
    fontFamily: "Noto Sans Thai, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif"
    fontSize: "12px"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "4px"
rounded:
  sm: "10px"
  md: "12px"
  lg: "14px"
  xl: "20px"
  full: "999px"
spacing:
  xs: "7px"
  sm: "11px"
  md: "18px"
  lg: "24px"
  xl: "40px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "#1a130a"
    rounded: "{rounded.lg}"
    padding: "17px"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.text-dim}"
    rounded: "{rounded.md}"
    padding: "12px"
  button-ghost-active:
    backgroundColor: "{colors.danger}"
    textColor: "#1a130a"
    rounded: "{rounded.md}"
    padding: "12px"
  card-stage:
    backgroundColor: "{colors.card}"
    textColor: "{colors.text}"
    rounded: "{rounded.xl}"
    padding: "40px 24px 34px"
  chip-rank:
    backgroundColor: "rgba(224,189,111,0.06)"
    textColor: "{colors.gold}"
    rounded: "{rounded.full}"
    padding: "5px 16px"
---

# Design System: Ceremonial Tea Name Generator

## 1. Overview

**Creative North Star: "The Forbidden Tea Scroll"**

The interface is a single warm-lacquer panel that behaves like an ancient ceremonial scroll, lit by candlelight: honey-gold leaf, soft matcha-jade ink, and a slow rotating glint of warm light passing over its surface. It exists to deliver one joke with total sincerity. A user taps a button, and the scroll solemnly proclaims an absurdly grandiose green-tea name (`Forbidden Imperial Ceremonial Jade Phoenix`), its Thai twin wrapped in 「」, and a deadpan "ceremonial grade" rank. The humor lives entirely in the gap between the ridiculous content and the reverent, precious presentation. The warmth keeps it cozy and lovable rather than grim; the design plays the ceremony straight so the words can be silly.

This is a toy, not a tool. It is Thai-first: the chrome, the controls, and the rank are Thai, and the English title is decorative flourish that serves the gag. Density is near zero. One stage, one big "อัญเชิญ" (summon) button, a small row of secondary actions, and a short history log. Everything is centered, mobile-first, and built so the *result* looks good the instant it is screenshotted and posted. Surfaces feel lit-from-within and a little expensive, but the interaction is toy-like and bouncy, never corporate.

It explicitly rejects the generic SaaS dashboard (no card grids, no settings-panel chrome, no eyebrow kicker stamped on every section), English-first layout, cold sterile minimalism, and anything mean or genuinely grim. The "เบียวสุด" (max-chuunibyou) chaos toggle is opt-in spice, signaled by the lone terracotta accent; it is not the resting mood.

**Key Characteristics:**
- Warm dark canvas with honey-gold-leaf and matcha-jade-ink accents; candlelit, not flat.
- Thai-first chrome; the solid honey-gold English title is decorative.
- One dominant action ("summon a new name") that must feel instant and re-spinnable.
- Output optimized to be screenshotted: the live stage and the 800x600 share-card are designed in parallel.
- Playful, lifted interaction over a precious, ceremonial surface.

## 2. Colors

A warm dark ground carrying two precious accents, honey gold and matcha jade, with a single terracotta reserved for the chaos state. Warmth is the cozy half of the personality; it lives in the body wash, the gold, and the glow, never in a cream/beige background.

### Primary
- **Ceremonial Gold** (`#e0bd6f`): The voice of the system. A warm honey gold. Used for the primary "summon" button fill, the rank pill text and hairline, and all gilt borders. Gold means "this is the ceremonial object."
- **Title Gold** (`#eccf85`): A brighter honey for the English title only, carrying a soft warm glow (`text-shadow`) in place of the old gradient. Solid, never gradient-clipped.
- **Gold Dim** (`#ab8e50`): The quiet gold, for the eyebrow label and footer mark. Gold turned down so it recedes without leaving the palette.

### Secondary
- **Jade Spirit** (`#7fd3a0`): The Thai name. A soft, warm matcha green, the one place green goes bright and alive, the "spirit" of the tea speaking in Thai. Reserved almost exclusively for `name-th`.
- **Jade Deep** (`#356f53`): Structural jade for muted green moments; a darker companion to Jade Spirit, used sparingly.

### Tertiary
- **Chaos Terracotta** (`#e07a5a`): The accent that breaks the gold/jade duotone. It appears *only* as the active fill of the "เบียวสุด" toggle, signaling the absurdity has been cranked up. Its rarity is its meaning.

### Neutral
- **Scroll Dark** (`#0b0d08`) / **Scroll Dark Lifted** (`#15160f`): The body ground, a radial wash from the lighter `bg2` at the top to the deep `bg`, topped by a warm amber candlelight glow. Warm near-black, never pure `#000`.
- **Panel Lacquer** (`#191b12`): The stage surface, a warm dark lacquer one step up from the ground.
- **Ink White** (`#f1efe6`): Primary readable text, a warm off-white.
- **Ink Muted** (`#a8a596`): Secondary text, ghost-button labels, the grade sub-label, and the footer.
- **Ink Faint** (`#6b6757`): The faintest tier, decorative only.

### Named Rules
**The Duotone Rule.** The system speaks in gold and jade only. Terracotta is the single exception and is forbidden anywhere except the active chaos toggle. Introducing a fourth hue dilutes the ceremony; if something needs emphasis, reach for gold, scale, or glow, never a new color.

**The No-Faint-Body Rule.** Ink Faint (`#6b6757`) is decorative, not for reading. Never set body copy, button labels, or anything a user must read in Ink Faint. Readable secondary text (grade sub-label, footer, ghost labels, log) uses Ink Muted (`#a8a596`), which clears 7:1 on the lacquer ground.

## 3. Typography

**Display / Body Font:** Noto Sans Thai (with the system stack `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif` as fallback).

**Character:** One family, doing everything, through weight and treatment rather than a second typeface. Noto Sans Thai keeps Thai and Latin visually unified, which matters in a Thai-first interface where English and Thai sit one line apart. Personality comes from weight contrast (400 to 700), letter-spacing, and the gold gradient on the title, not from font pairing. This is deliberate: a single confident family reads as composed; competing display faces would read as costume.

### Hierarchy
- **Display** (700, 27px, line-height 1.3, +0.5px tracking): The English ceremonial title (`name-en`), solid Title Gold (`#eccf85`) with a soft warm `text-shadow` glow and `text-wrap:balance`. The loudest element on the stage. Reserve a `min-height` so the stage doesn't jump between one-line and two-line names.
- **Headline** (600, 19px, line-height 1.45, jade): The Thai name (`name-th`), wrapped in 「」. The emotional center for the Thai-first audience.
- **Body** (600, 14px, line-height 1.4): Ghost-button labels and the history-log entries. Quiet, functional.
- **Label** (600, 11-12px, +3 to +4px tracking, UPPERCASE): The eyebrow (`ceremonial grade tea`) and the grade sub-label. The *only* place uppercase and wide tracking are allowed.

### Named Rules
**The One-Family Rule.** Noto Sans Thai carries the entire system. Do not add a second display or decorative typeface to "elevate" the ceremony; elevation comes from the gold gradient, weight, and spacing. Mono is not used and should not be introduced.

**The Uppercase-Label-Only Rule.** ALL CAPS and wide letter-spacing are reserved for the two short labels (eyebrow, grade). Never set Thai content, names, or any sentence in uppercase; it is for ≤4-word labels exclusively.

## 4. Elevation

Depth is glow-lit, not shadow-stacked. The system reads as a lacquered object lit by warm candlelight rather than a stack of paper cards. At rest, the stage carries a soft ambient drop shadow, a warm amber outer glow, and an inset gold top-highlight that makes the surface feel like polished lacquer catching light; a slow conic-gradient glint rotates behind it. On interaction, the feel turns playful and lifted: the primary button rises and its gold glow blooms on hover, then presses in on click. The doctrine is glow at rest, lift on touch.

### Shadow Vocabulary
- **Ambient Stage** (`box-shadow: 0 18px 50px rgba(0,0,0,0.45), 0 0 90px rgba(196,142,72,0.12), inset 0 1px 0 rgba(224,189,111,0.10)`): The stage panel. A soft shadow grounds it, a warm amber halo makes it glow, and the inset gold hairline is the lit-from-within highlight.
- **Gold Lift, rest** (`box-shadow: 0 6px 24px rgba(224,189,111,0.25)`): The primary "summon" button at rest, a warm gold glow beneath it.
- **Gold Lift, hover** (`box-shadow: 0 8px 30px rgba(224,189,111,0.4)`): The same glow intensified as the button rises `translateY(-1px)`.

### Named Rules
**The Lit-From-Within Rule.** Depth comes from glow (ambient halos, inset highlights, gold blooms), never from hard grey drop-shadows. If a surface looks like it has a 2014-app gray box-shadow, it's wrong; the light is warm and diffuse, or it isn't there.

**The Lift-On-Touch Rule.** Interactive elements are playful: they rise and brighten on hover and press in on `:active`. Static, dead-on-click controls break the toy feel. Every button earns a transform and a glow change on interaction.

## 5. Components

### Buttons
- **Shape:** Gently rounded. Primary 14px radius, ghost/secondary 12px radius.
- **Primary ("อัญเชิญชื่อใหม่" / summon):** Full-width gold-gradient fill (`linear-gradient(100deg, #e0bd6f, #f1da9e, #e0bd6f)`), near-black text (`#1a130a`), 700 weight, +1px tracking, 17px padding. Carries the Gold Lift glow.
- **Hover / Active:** Hover rises `translateY(-1px)` and intensifies the glow; active scales to `0.98`. Transitions: `transform .12s ease, box-shadow .2s ease`.
- **Ghost (secondary actions):** Transparent fill, 1px gold-translucent border (`rgba(224,189,111,0.18)`), Ink Muted label. Hover brightens text to Ink White, lifts the border to `rgba(224,189,111,0.4)`, and adds a faint gold tint background. Active scales to `0.98`. Laid out two-per-row.
- **Ghost Active (chaos on):** When "เบียวสุด" is toggled on, the button fills Chaos Terracotta (`#e07a5a`) with near-black text. The only terracotta in the system.

### Chips (rank pill)
- **Style:** Inline pill, full radius (999px), 1px gold-translucent border, faint gold tint background (`rgba(224,189,111,0.05)`), Ceremonial Gold text at 12.5px.
- **State:** Display-only; it states the absurd grade. Animates in with a `pulse` on each new name.

### Cards / Containers (the stage)
- **Corner Style:** 20px radius.
- **Background:** A warm dark lacquer gradient (`linear-gradient(160deg, #191b12, #11130c)`), 24px radius.
- **Shadow Strategy:** Ambient Stage (see Elevation). Plus a slow 14s conic-gradient glint rotating behind the content (`::before`, `overflow: hidden`).
- **Border:** 1px gold-translucent (`rgba(224,189,111,0.18)`).
- **Internal Padding:** `40px 24px 34px`.

### History Log
- **Style:** Stacked one-line entries, 10px radius, near-invisible white tint background (`rgba(255,255,255,0.02)`) and border (`rgba(255,255,255,0.05)`), Ink Muted text, truncated with ellipsis. Newest on top, capped at 5. Each enters with a `rise`.

### Signature: The Summoning Stage
The centerpiece. A lacquered scroll-panel that proclaims the name with choreographed reverence: the English title `flash`es in (letter-spacing collapsing from 8px), the Thai name `rise`s up through a blur a beat later (`.12s` delay), and the rank pill `pulse`s last (`.28s` delay). The staggered sequence is the ceremony; it must feel like a proclamation, not a form re-render. A parallel 800x600 canvas renders the same composition (gold frame, gold title, jade name, gold rank pill) as a shareable PNG.

## 6. Do's and Don'ts

### Do:
- **Do** keep the interface Thai-first. Chrome, controls, and the rank are Thai; the solid honey-gold English title is decorative flourish that serves the joke.
- **Do** present absurd names with sincere, ceremonial polish. The deadpan gap between silly content and reverent gold-and-jade presentation *is* the humor.
- **Do** keep depth glow-lit: ambient halos, inset gold highlights, warm blooms. Lift and brighten interactive elements on hover; press them in on `:active`.
- **Do** design the share-card (800x600 canvas) in lockstep with the live stage. Every output is built to be screenshotted and posted.
- **Do** stagger the reveal (flash title -> rise Thai name -> pulse rank). The choreography sells the proclamation.
- **Do** reserve uppercase + wide tracking for the two short labels only (eyebrow, grade).
- **Do** add a `prefers-reduced-motion` fallback. The 14s conic spin and the entrance choreography both need a calm alternative (crossfade or instant), and reveals must enhance an already-visible default, never gate content on a transition.

### Don't:
- **Don't** turn this into generic SaaS or a dashboard: no card grids, no settings-panel chrome, no tiny uppercase eyebrow kicker stamped above every section. It is a toy, not a tool.
- **Don't** make it English-first or English-only. Thai is the primary language.
- **Don't** let the chuunibyou energy go mean, cynical, or grim. The "เบียวสุด" mode is camp and lovable; warm beats cool, even at maximum chaos.
- **Don't** strip it into cold, sterile minimalism. The ceremonial richness and warmth are the soul; don't sand them off chasing "clean."
- **Don't** introduce a fourth hue. Gold and jade only; terracotta is the lone exception, allowed solely on the active chaos toggle.
- **Don't** set readable text in Ink Faint (`#6b6757`); its contrast on the lacquer ground is borderline. Readable secondary text uses Ink Muted (`#a8a596`).
- **Don't** gradient-clip the title (`background-clip:text` over a gradient). The English title is a solid Title Gold with a warm `text-shadow` glow; the metallic feel comes from the glow and weight, not a gradient.
- **Don't** add a second display typeface. Noto Sans Thai carries the whole system through weight and treatment.
