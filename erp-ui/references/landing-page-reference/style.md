# Landing-page reference style

A personal portfolio site that the landing-page mode is modelled on: one long dark page with seven sections, measured at desktop 1440×900 and phone 390×844. It is the landing-page taste reference, not the app reference. No screenshots are included.

## Tokens (measured)
- **Background:** `#0a0a0a`, flat, with no gradient anywhere (`background-image: none` on every element).
- **Text:** warm off-white `rgb(233,228,218)`, never pure white. Muted text is cool grey `#9a9aa4` / `#8f8f9a`, with dimmer `#63636c`–`#75757e`.
- **Accents:** one colour per project, used only in the small project label and its progress dashes, for example purple `#8b7bff`, green `#5fd39a`, pink `#d96bb1`, orange `#f0a150`, blue `#6fb3f2`, and red `#f26d5f` for a chart.
- **Type:** three voices.
  1. **Caveat** handwriting, 500–600 weight, for the name, the section titles ("selected work") and the first-person headlines.
  2. System sans (`-apple-system, Helvetica Neue`) for body text, 13.5–16 px.
  3. Monospace (`ui-monospace, SF Mono`), 9–11 px, UPPERCASE with 1.1–1.8 px tracking, for meta labels, dates, nav and links.
- **Radii:** almost none. 0 everywhere, with 2–3 px on small chips, 7–10 px on photo tiles, and circles for dots.
- **Shadows:** none at all.
- **Borders:** hairlines only, on small chips and section dividers.
- **Layout:** the text column is about 540 px max, on the left third. A large single-line portrait drawing is fixed on the right. Each work item fills one viewport.
- **Navigation:** a fixed right rail of tiny mono labels, each with a bar whose width marks position. The active item is a white 28 px bar. No top nav bar.
- **Motion:** opacity and transform only, 0.25–0.35 s with the default ease, on the rail labels and hover. No scroll-jacking, no entrance animations, no infinite animations.

## What defines the look (top 10)
1. **Dark, flat and almost empty.** One colour plane, no cards, no boxes, no shadows.
2. **A handwritten headline voice.** Caveat for titles and claims gives warmth against the technical mono.
3. **First-person claims as headlines:** "I turned one client into a company." Short and concrete, with a number where there is one.
4. **A line-art self-portrait** as the only illustration. Continuous strokes, no fill, and it stays put while the content scrolls.
5. **Mono uppercase meta labels**, small and tracked, in the project's accent colour: `COMPANY · ROLE`.
6. **Colour is a signature, not decoration.** Each project gets one hue, used in two tiny places only.
7. **One idea per screen.** Each project gets a full viewport, with a lot of empty space.
8. **Quiet navigation.** The right-edge rail with position bars replaces a header.
9. **Real logos and real store badges** instead of generic icons.
10. **Data shown honestly:** a thin-line chart with direct labels and no gridline clutter.

## Where it breaks from SaaS template defaults
- No gradient hero, no glow, no glassmorphism, no rounded cards, no drop shadows, no icon grid of features.
- No top nav bar, no CTA button. Contact is a plain mono link list.
- No stock photos. The only photos are real event photos, as small tiles.
- Copy is personal, in the first person and specific, not "Empowering teams to…".
- Small type everywhere except the headlines. The hierarchy comes from the typeface, not from size jumps.

## Use in the skill
Carry over: the restraint (flat, no cards or shadows), the warm off-white on near-black, the mono meta labels, one accent per subject, concrete first-person copy, and one idea per screen.
Caveat handwriting is a personal-site signature; ask before using it in products.
