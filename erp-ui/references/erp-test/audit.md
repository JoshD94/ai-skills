# Dummy ERP prototype: self-audit

The builder's self-audit for the screens in this folder (E1–E37; E22 is left out because it shows a team table with email addresses). 37 shots were captured with headless Chromium, desktop and phone, light and dark, plus a loading (skeleton) state. Every name, number, email and phone number in them is invented. The critique of this build is in `../../feedback.md` under "Test build: a dummy ERP".

## Never list
1. AI-slop captions: pass. No eyebrows, subtitles, meta lines or corner text. The only thing under a title is a control.
2. Number + title + caption triple: pass.
3. Dividing lines: pass. No row lines or rules anywhere. Rows use a hover background and attention items are soft cards.
4. Sharp shapes: pass. Every corner is a squircle: cards 16, buttons 12, inner rows concentric (card − 8).
5. Glued to the edge: pass. The sidebar, phone tab bar, sheet and toasts all float with margin.
6. One typeface: pass. System stack only (Noto Sans on the capture machine, whose "1" has no foot).
7. Random colour: pass. Greys plus one blue, used only on primary buttons and the Add button. Charts, active nav and numbers stay neutral. Cancelled isn't coloured.
8. Text acting as a button: pass. Every action is a styled button. Metric cards and rows that click lift or highlight on hover.
9. Inconsistent buttons: pass. All 36 px, one radius, icons on all buttons in a group or on none.
10. Square avatars: pass. People are circles; shops are rounded squares. The profile is a bare avatar circle bottom-left that opens a menu, copied from the app-chrome reference.
11. Clutter: pass. No badges and no tags. The Orders count in the nav is plain grey text.
12. Logo and language picker: pass. The logo is a plain letter tile plus the product name. The language picker is a flag plus the name, opening a dropdown. [Later changed: short codes, not names.]
13. Device mockups: none used.

[The reviewer still found eight problems that this audit passed: see the feedback. A self-audit is a floor, not a verdict.]

## Where a rule was bent, and why
- Squircle radii are 1.5x in CSS (24/18 px) where `corner-shape` is supported. At equal radius a squircle looks much tighter than a circular arc, so the bump keeps the 16/12 px roundness that was picked. Without support it falls back to plain 16/12 px.
- Charts use neutral greys, not accent shades. "Visual system" says charts stay neutral, and that wins over the older "Always" line.
- Validation errors use one muted red with an icon. A grey error read like help text.
- The delta (for example "9,7%") has no "vs last Saturday" text, because of the corner-text ban. The comparison basis is only in a tooltip.
- Toasts: bottom centre on desktop, where there are no actions (they sit in the page header). On phone they go above the tab bar, left of the Add button.
- No count-up: none of the data is real-time. There are no submenus, so no safe triangle was needed. Every dropdown opens on click and works with the keyboard.
- Skeletons are the real DOM with text turned into pulsing blocks. A script measured 201 and 785 boxes in loaded vs loading views, with 0 differences.

## Made-up placeholders (all invented)
- A fashion brand with 6 shops plus two marketplace stores.
- 40 products: names, SKUs, prices, costs at 42% of price, and stock levels. Low stock means fewer than 4; the 8 low items are fixed on purpose.
- 10 team members, emails and roles. Sale numbers, member phone numbers, masked buyers, couriers and order numbers.
- All sales come from a seeded generator with "now" fixed at a Saturday, 14:20. Days 8–30 are aggregates only.
- Comparisons: Today is compared with the previous Saturday at the same time; Week with the previous 7 days. Month is a fixed +6% placeholder.
- The "Synced 2 min ago" tooltip, the suggested SKU, and every toast message.
