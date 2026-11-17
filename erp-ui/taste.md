# UI taste: the rules

Where this file disagrees with `principles.md` or generic best practice, this file wins.

**Read `feedback.md` next to this file as well.** It has the full critiques and the reasons, in the reviewer's own words, plus how they talk: direct, "AI slop", "random captions", "border radius should sync", "too blocky", "classy", "for ERP…" trade-offs. When a case isn't covered here, decide from those notes. Write critiques and summaries in that plain, direct voice.

Evidence:
- The critique of two AI-made landing pages, screens A–J in `references/ai-site-critique/`. A–E are site one and F–J are site two. Site one was liked much more; F was "even more terrible".
- The picker answers in `references/answers.md`.
- Landing-page reference: `references/landing-page-reference/style.md`.
- App-chrome reference: `references/app-chrome/` ("copy [the reference app] for this if needed").
- A dummy ERP built with this skill and then critiqued (E1–E37): `references/erp-test/`.

How to use it:
- **Redesign or new build:** these are rules. Any item in the Never list is a hard failure.
- **Editing an existing tool:** the product's current look still wins. List any violations you notice as short suggestions; don't silently restyle.

## Landing pages are a different mode
The first test build was a landing page. It followed every rule and was called "extremely tasteless". The rules below are about restraint, and restraint alone makes an ERP, not a landing page.
- A landing page needs **flair**: a concept, a running theme, a storyline from screen to screen, and a signature graphic or illustration. The landing-page reference is the model: a fixed line-art portrait, handwritten headlines, one story per screen, and one colour per project.
- Keep the restraint rules: no slop captions, no lines, matching radii, few fonts and colours. But never ship a landing page that is only a clean app UI on a white page. Decide the concept, theme and signature visual first, and show them before building.
- An ERP or app screen is the opposite: calm, dense, no decoration. Apply the visual system below.

## Editing an existing tool: change only what was asked
- When asked to tidy an existing page, such as "remove a lot of random text", change only that. Keep the layout, colours and structure. A dashboard tidy-up that also put two panels side by side and changed the theme was rejected: "I like the old one."
- "Less text" means much less: one plain fact per line, each fact shown once. Raw system or debug strings ("CPU headroom 5.02 cores < need 6.00", "| pressure normal | heartbeat 32s ago") move into hovers.
- Redesign only when asked for a redesign. Editing is the default for anything that already exists.
- When asked for a "UI pass" on a new page, tightening spacing isn't enough: look at where each control lives (page header, view switch, toolbar, filters, side lists) and propose a reorganized layout.

## Never (critical failures)
1. **AI-slop captions.**
   - Eyebrow or kicker labels above titles: "01 · Today's totals", "— Customer stories", "THE SHOP-OWNER PERSPECTIVE". (E, G, J)
   - Subtitle paragraphs that restate the title. (A, F)
   - Reassurance micro-copy under buttons: "No card needed · About 15 minutes per shop · Help on WhatsApp". (A, F, I)
   - Meta lines under page titles: date · number of shops · Live. "As of" lines, references disclosures. (C, H)
   - Small grey text in card corners: "vs last Saturday", "5 items · 3 shops". (H, I)
2. **The number + title + caption triple** repeated across three columns. (B)
3. **Dividing lines.** None between list items, table rows, stats, footer sections or columns. No decorative rules next to headings, no lines tying sections together, and no line above a profile. Separate with space, or give each item its own card with a soft background. (A, B, C, E, F, J)
4. **Sharp or square shapes.** No square cards, sharp ticket or receipt shapes, zigzag torn-paper edges or blocky rules. Nothing in the UI has small or zero radii. (A, D, F, J)
5. **Elements glued to the page edge.** Strips and bars float with margin and full rounding; they don't stick to the bottom or sides. (A)
6. **More than one typeface.** No serif, no italic accent words, no display-font mixing, and no mismatched contrast between font sizes. One sans family. (F, G, H, I, J)
7. **Random colour.**
   - Only black, white and one accent, with shades of that accent. It must work in both light and dark.
   - No green + yellow pairing, no multi-colour cards, no rainbow tags.
   - Don't colour negatives loudly. Highlight only the primary card, not "Cancelled", and no error banner sitting on top of a card. (D, G, H, I, J)
8. **Text that acts as a button without looking like one**, for example bare "Review" or "Check". (C, H)
9. **Inconsistent buttons.**
   - Buttons in one view have different radii or sizes.
   - An arrow on one button and not on its sibling. (A, F, I, J)
10. **Square avatars for people.** People are always circles. Avoid the profile picture + name + caption stack; copy the reference app's profile area instead (a bare avatar circle that opens a menu). (E, H)
11. **Clutter.** Tag clouds, nested badges ("2 months free" inside a toggle), tier labels in corners ("1–3 shops"), rating badges in corners, extra calculators, back-to-top buttons. (G, I, J, E)
12. **A sloppy logo or language picker.** The logo is simple and clean. The language picker is a flag plus a short language code (EN, ID, CN), never the full name. (F)
13. **Badly made device mockups** (laptop or phone). Either make them well or leave them out. (G)

## Always
- **Radii:**
  - Generous: buttons clearly rounded, 12 px. Cards are 16 px.
  - The same radius for every button in a view.
  - Nested radii are concentric: outer radius = inner radius + padding.
  - Tabs, segmented controls, dropdowns and icon-button hover states are rounded too.
  - Charts in one view share the same bar radius.
- **Compact and sized to content.**
  - Metric cards are only as wide as their number needs; a cancelled-sales count needs a small card.
  - Lists and tables don't stretch across the screen.
  - Long text truncates cleanly.
- **Tables:**
  - Dense rows, without wasted padding between items.
  - No row lines. Use row backgrounds or spacing.
  - Columns sized to their data.
- **Lists that need attention** (low stock and the like): each item is its own small soft card. They are not separated by lines.
- **Spacing:**
  - Clear, even vertical gaps between rows of cards.
  - Labels sit right next to their controls.
  - Dropdowns have tight padding around the value.
- **Charts:** slim bars in shades of the single accent.
- **Under a title, only useful things:** a control, real data, an icon-led point, or nothing.
- **Copy:** headlines sound human and specific, never generic AI wording. Fewer words everywhere.
- **Icons:**
  - Feather, 1.75 stroke, round ends, 16 px beside 14 px text, the same colour as the text, bare (no containers).
  - Never oversized in lists.
  - Icon + label in navigation.
  - The active nav item is shown by the row highlight, not by a filled icon.
- **Empty states:** one big Feather icon (about 40 px, 1.5 stroke) and a short title. No sentence, no button, no illustration.
- **Language picker:** a flag plus a short code (EN, ID, CN), opening a dropdown. No full language names ("English", "Bahasa Indonesia"), in the trigger or the list.
- **Pricing:** simple and focused. Plan name, price, one list of features and one button style. Nothing else.
- **Testimonials:** all the same card size, font and colour.
- **Footer:**
  - Calm, grouped by spacing, with no lines.
  - Privacy, terms, language and copyright are fine.
  - The same type scale as the rest of the page.

## Visual system (for ERP and app UI)
- **Type:**
  - The system font stack, with tabular figures for numbers.
  - Headings weight 600. Big numbers 24 px: they are bold already, so they don't need size.
  - Body 13 px. Labels grey and regular weight, one standard style.
  - The digit "1" must be plain, with no foot serif. Avoid fonts whose 1 has a base line.
- **Colour:**
  - Light by default, because older clients like white. Dark mode also exists.
  - Off-white page (about `#fafaf9`) with white cards on a soft shadow. Cool greys.
  - Accent blue by default (it varies per product), medium strength.
  - Accent only on primary or key action buttons, such as "Add". The active nav state, charts and numbers stay neutral.
  - Nothing changes colour when clicked.
- **Continuous corners:**
  - Every rounded corner is a continuous curve (squircle), never a plain circular arc that kinks where it meets the straight edge.
  - Web: `corner-shape: squircle` with `border-radius` as the fallback where unsupported (check support).
  - iOS: `RoundedRectangle(cornerRadius:style: .continuous)` / `cornerCurve = .continuous`.
  - Android: a smooth-corner shape.
  - No abrupt changes in curvature anywhere.
- **Nested menus:**
  - Submenus use a safe triangle or area so a diagonal move toward the submenu doesn't close it (Costa Alexoglou, Smashing Magazine 2023, after Amazon/Ben Kamens).
  - The safe area expires when the pointer stops (debounced) and is dropped when the pointer goes back to the parent, like macOS and Radix.
  - Every hover menu also opens on click, tap and keyboard.
- **Shape and density:**
  - Cards 16 px radius (24 is preferred, but it wastes space in an ERP). Buttons 12 px.
  - Rows 36–44 px, matched to the radius.
- **Status:** a small dot centred on the text, then the text, by default. A soft coloured pill is sometimes worth it, for the one status that needs attention. Never a different loud colour per status.
- **Sidebar:** dark, contrasting with the light page.

## Copy
- **Headlines:** short, snappy bold claims, not AI-sounding. For example "All-in-one Shopee and TikTok ERP".
- **Voice:** neutral ("2 shops haven't synced yet"). No emoji in product UI or copy, with two exceptions: emoji reactions under comments, and an emoji picker in rich text editors, so users can add emoji to their own content. Nowhere else.
- **Money:** full `Rp 12.400.000`. Short `Rp 12,4 jt` only when space is tight.
- **Dates:**
  - Relative smart dates ("Today, 14:05").
  - Otherwise write the month out: "7 Nov 2026". Never 07/11/2026. This applies when showing and when choosing dates.
- **Help text under fields:** none. Make the field clear instead. Show validation errors, and help text only when it's truly needed.
- **Feedback after saving:** a toast that never covers buttons, especially bottom-right actions.

## Motion
- About 220 ms with ease-out.
- **Presses:** a small shrink, and nothing else on the page moves.
- **Pages:** slide, only for real page changes. Sheets ease out.
- **Lists:** staggered, but fast enough that nobody waits.
- **Tabs:** the segmented-control pill slides.
- **Hover:** cards lift slightly.
- **Totals:** count up only where the data really is real-time.
- **Loading:** a pulsing skeleton (no spinners).
  - Every skeleton matches the final layout exactly: the same boxes, sizes and positions, so nothing shifts when the data arrives.
  - Check before, during and after loading.

## Phone
- Bottom tabs with icon + label, and a floating button for the main action.
- **Header:** the shop picker itself is the header (may vary per app).
- **Choosing a shop:** a full-screen list.
- **Details:** open as full pages.
- **Filters:** dropdowns.
- **Nested and focused:** one concern per screen, with options nested rather than crammed together.
- **Tables:** compact rows, never cards, because cards scroll too much. Avoid big tables on phone; often a summary is better.

## Components (from the dummy ERP test)
- **Detail and create views on desktop** open in a side pane or a modal, never a full page. This covers item details and "New product". Phone still uses full pages.
- **Toggles:** a circular thumb inside a pill track. Never a square inside a pill; the shapes must match.
- **Menus and popovers** opened from the dark sidebar (account, workspace) use the sidebar's dark surface, not a white card next to it.
- **Error and alert icons** align with the first line of text, never centred on a two-line message.
- **Dropdowns:**
  - Every dropdown is custom, built as one reusable component used everywhere. Never the native `<select>` look.
  - It matches the 12 px controls and continuous corners.
- **Save buttons:**
  - If the form fits on one screen, Save goes at the bottom, not the top right.
  - If it scrolls, unsaved changes must be obvious, for example a sticky save bar at the bottom. Leaving with unsaved changes asks first.
- **Toasts:** at the far right edge, placed so they never cover action buttons.
- **Brand mark:** no generic letter-in-a-square or stock icon as the logo. Use a clean wordmark or a real mark.
- **Skeletons:** measure each element, including small cards in a row. The cards in one row must be the same size as their loaded versions. E28 failed this on the transaction, basket, cancelled and to-ship cards.

## Things that were liked
- C: a real product screenshot as the hero of a section. The dashboard layout.
- B: the "Live total today" card and the small cards under it.
- G: rounded bento cards of varied sizes. "Very modern."
- J: the closing "Tomorrow at 7 a.m." call-to-action card.
- H: the Today / Week / Month segmented selector. The app view itself.
- A: an illustration on the right of the hero.

## Live review rules: sales ERP (screens J1–J8 in feedback.md)
- Every product shown anywhere (lists, panes, merchandising, cancellations) has its picture. (J3)
- One search bar component and one custom dropdown component across the app. Same height, radius and focus style. (J6)
- Every button, including Filter, has a visible hover state.
- Data tables fill the screen height, and their rows are compact. Sticky headers must never overlap rows. (J1, J7)
- Summary rows (a "by reason" chart, totals) are clickable filters for the list under them. (J4)
- Never hide a data table inside a disclosure box; show it as a section. (J5)
- Sidebar items all have icons, sub-items included. (J8)
- A redesign keeps the columns people use to check numbers (money and difference columns) visible by default.
- Loading stays under 0.5 s, skeleton first.

## Report pages
- Reports are chart-first. Detail tables sit under the charts behind one segmented switch (a dropdown on phones), so only one table shows at a time.
- Every table longer than a page gets the standard bottom bar (count + pager, 50 per page). No "show 50 more" buttons, and no unpaged 200-row tables.
- When a table only repeats numbers that another table already shows, drop it.

## Live review rules: sales ERP, later passes (points 1–8 in feedback.md)
- One scrollbar style for the whole app, horizontal and vertical alike (thin, soft grey thumb, no track). Never restyle a scrollbar per element. (1)
- Popovers from one toolbar never stack: opening one closes the other. (2)
- Icon-only steppers (‹ › next to a period chip) say what they step to (label or tooltip with the range). (3)
- Money-check columns (differences) stay visible by default; colour green/red only when there is a difference. (5)
- Whole-row click opens the pane; no per-cell modals. Columns are sized so statuses don't truncate. (7)
- Fee rows say who pays (left icon + short label: Buyer, Platform, Seller) and are coloured by direction. (8)
- Focused fields, searches and dropdowns show a background tint only: no ring, no outline, no darker border. (6)
- Settings pages: titled groups of rows on soft cards (no lines), status as dot + text, whole row opens its dialog, facts shown as a section (not a disclosure), no "i" tips, quiet footer links. (6)

## Leads app, second pass
- Never cut features to simplify; group them. A card shows one primary action; secondary actions (DM, notes, AI analysis, history…) live in one grouped place, not a row of buttons.
- The page's main content comes first (a schedule, a list). Titles, captions, "why" explainers, stats, posting times and automation go below it or behind a click.
- An open/selected card is not marked with a tinted fill plus a left border stripe. Use a soft grey fill; no border or outline either.
- Calendar and list items never carry a heavy coloured left border; use a soft fill, a dot or the item's circle.
- Every control in one toolbar row shares one height and one vertical centre: search, buttons, title and segmented picker.
- Filters and toolbars use the app's shared components, never a page-local version.
- Spacing and padding benchmark: the best-spaced existing page in the same app.
- Every loading state has a skeleton shaped like the content it replaces.
- Clicking an item never navigates away to another tab.

## Plain language on ops screens
- Write for a non-technical reader: say what is happening and what they must do, in plain words.
- Hide technical details by default (hostnames, stack/step ids, logs, parameter paths, hashes, digests): behind one quiet "Details" disclosure, or drop them when nobody needs them.

## Alora Design review (design.alorawork.com)
- Dark mode is truly neutral near-black (no blue tint). The Alora Design library defaults to dark, neutral greys and a pink accent; products may choose otherwise.
- One padding scale for every pill, chip, filter bubble and segment, so siblings never look different.
- Numbers: short values (one or two digits) get their own treatment so they don't sit lost in a card; long values stay readable without stretching cards.
- Triggers (date, select) are sized to their value, not stretched.
- Alerts: a one-line alert centres icon, text and action on one line; multi-line keeps the icon on the first line.
- The site/app header sits in the same place and size on every page.
- Example apps never show a nav item that leads nowhere.
- Showcase pages present components natively, composed into a bento of real-use cards; never a grid of one labelled tile per component. (S24, S25)
