# Product

## Register

brand

## Users

Thai-speaking internet users in a playful mood: matcha fans, meme-posters, and friends goofing off in a group chat. They arrive from a shared link or screenshot, spend thirty fun seconds spinning up ridiculous "ceremonial grade" tea names, and leave with an image to post. No account, no learning curve, no goal beyond delight and a laugh. Mobile-first, often one-handed, usually mid-scroll.

## Product Purpose

A single-page novelty generator that conjures absurdly grandiose green-tea names: an over-the-top English title (`Forbidden Imperial Ceremonial Jade Phoenix`), a Thai name wrapped in 「」, and a deadpan "ceremonial grade" rank that escalates to the cosmic and the forbidden. A "โหมดเบียวสุด" (max-chuunibyou) toggle cranks the absurdity further with a chaos suffix. Users can hear it read aloud (TTS, English then Thai) and copy a rendered image card to share.

Success is a laugh and a share: the user generates a name that's funny enough to screenshot and post, or reads it aloud to friends. The product wins on shareability and repeat-spin delight, not on retention or utility.

## Brand Personality

Meme-shareable and cozy-wholesome at its core, with a knowing wink. The humor comes from a soft, friendly matcha-lover charm colliding with deadpan, maximalist ceremonial pomp: the names are absurd, but they're delivered with a straight face and genuine warmth, never mean. Voice is Thai-first, casual, and quick. The "เบียว" (edgelord) energy is a deliberate, opt-in spice, the chaos mode, not the resting personality.

Three words: **playful, warm, deadpan-grand.**

## Anti-references

- **Generic SaaS / dashboard UI.** No card grids, no kicker-eyebrow-on-every-section, no settings-panel feel. This is a toy, not a tool.
- **English-first or English-only layout.** Thai is the primary language; English titles are flavor, not the interface.
- **Mean or genuinely edgy.** The chuunibyou mode is camp and self-aware, never cynical, grim, or hostile. Keep it lovable.
- **Cold, sterile minimalism.** Warmth and a little ceremonial richness are the point; don't strip the soul out chasing "clean."

## Design Principles

- **Thai-first, always.** Interface, copy, and primary content are Thai. English is decoration that serves the joke.
- **The spin is the product.** The single most important interaction is generating a new name; it must feel instant, satisfying, and worth repeating. Everything else is secondary.
- **Built to be screenshotted.** Every output should look good as a standalone shared image. Optimize the result card, not just the live page.
- **Deadpan delivers the joke.** Present absurd names with sincere, ceremonial polish. The contrast between earnest presentation and ridiculous content is the humor; don't undercut it with jokey UI.
- **Warm, not grim.** Even at "เบียวสุด," the feel stays inviting and fun. Cozy beats cool.

## Constraints

- **Single file, no build.** Ships as one `index.html`, deployable to Vercel as a static file with no build step. Preserve this; it's a feature, not an accident.

## Accessibility & Inclusion

Not a formal WCAG target, but baseline care expected: legible body contrast on the dark surface, honor `prefers-reduced-motion` for the spin/reveal animations (the ambient conic-gradient spin and entrance animations especially), and keep all controls keyboard-reachable and labeled. TTS is a progressive enhancement; the page must work fully without it.
