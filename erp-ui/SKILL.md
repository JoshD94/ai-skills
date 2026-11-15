---
name: erp-ui
description: "Run whenever the user says \"erp ui\" (alone or in a sentence, any case), or asks to build, redesign, edit, tidy or critique an ERP, admin, dashboard or app UI with this taste. One self-contained file: the rules (Part 1, these win), the reviewer's critiques in their own words (Part 2), and 93 chosen UI/UX principles (Part 3). Editing an existing tool changes only what was asked; redesign only when asked. Landing pages need a concept and flair first."
---

# ERP UI

An opinionated taste for ERP, admin and app interfaces: calm, dense, rounded, no clutter. It was written down from one product owner's picks and line-by-line critiques of real screens, so the rules are specific and tested, not generic best practice.

How this file is laid out:
- **Part 1, Rules:** modes, the Never and Always lists, visual system, copy, motion, phone, components, data pages. **These win over everything else.**
- **Part 2, The reviewer's words:** the critiques behind the rules, and how the reviewer talks. Read it whenever a case isn't covered by Part 1.
- **Part 3, Principles:** 93 UI/UX principles kept from 100 candidates. Background only; Part 1 wins.
- **Appendix:** the landing-page reference style.

Letters like A–J or E28 in Part 2 point to the screens that were critiqued. The screenshots aren't included; the text says what each one showed. The app-chrome reference is T3 Code (t3.codes).

No score-driven hill climb: rubric scores went up while the reviewer liked the result less, and a climb only polishes a UI that is already good.

## Pick the mode first
- **Edit an existing tool** (the default for anything that already exists):
  - Change only what was asked for, such as "remove the random text" or "fix the toggles".
  - Keep the layout, colours and structure.
  - Put any wider ideas in a short list; don't build them.
- **Redesign:** only when asked for a redesign or a new build. Part 1 is the spec, and every Never item is a hard failure.
- **Landing page:**
  - Restraint alone looks tasteless here. First propose a concept, a running theme and a signature visual (see the Appendix), and get an OK.
  - Then build with the restraint rules.

## Workflow
1. Read Part 1 and Part 2 in full, and the repo's AGENTS.md or CLAUDE.md if there is one.
2. Work on a branch or in an output folder for prototypes. Don't merge, release or deploy without the reviewer's OK.
3. **Self-audit once:**
   - Screenshot every changed screen and state with a headless browser, desktop 1440×900 and phone 390×844.
   - Check each screenshot against every Never and Always item.
   - Fix what fails.
   - Write `audit.md`, at most 40 lines: pass or fail per Never item, plus any placeholders or invented facts.
4. **Show the reviewer** one review page:
   - Lettered screenshots (E1, E2… or Q1…) so they can reply "for E6, …".
   - Before and after side by side when editing. Capture both within seconds of each other so the data matches.
5. **Write feedback back** into this file the same day:
   - Their words go in Part 2, under a dated heading.
   - New or changed rules go in Part 1.
   - Don't flatten an "it depends" into an absolute.

## Rules that always apply
- No production or client data in screenshots.
- Logic doesn't change in a UI pass unless asked: "only UI should have changed."
- Write plainly and briefly, in a direct voice. See "How the reviewer talks" in Part 2.

---

## Part 1: Rules
Where this part disagrees with Part 3 or generic best practice, this part wins.

- **Redesign or new build:** these are rules. Any item in the Never list is a hard failure.
- **Editing an existing tool:** the product's current look still wins. List any violations you notice as short suggestions; don't silently restyle.

### Landing pages are a different mode
A test landing page that followed every rule here was called "extremely tasteless". The rules below are about restraint, and restraint alone makes an ERP, not a landing page.
- A landing page needs **flair**: a concept, a running theme, a storyline from screen to screen, and a signature graphic or illustration. See the Appendix for the model.
- Keep the restraint rules: no slop captions, no lines, matching radii, few fonts and colours. But never ship a landing page that is only a clean app UI on a white page. Decide the concept, theme and signature visual first, and show them before building.
- An ERP or app screen is the opposite: calm, dense, no decoration. Apply the visual system below.

### Editing an existing tool: change only what was asked
- When asked to tidy an existing page, such as "remove a lot of random text", change only that. Keep the layout, colours and structure. A tidy-up that also rearranged panels side by side and changed the theme was rejected: "I like the old one."
- "Less text" means much less: one plain fact per line, each fact shown once. Raw system or debug strings ("CPU headroom 5.02 cores < need 6.00", "| pressure normal | heartbeat 32s ago") move into hovers.
- When asked for a "UI pass" on a new page, tightening spacing isn't enough: look at where each control lives (page header, view switch, toolbar, filters, side lists) and propose a reorganized layout.

### Never (critical failures)
1. **AI-slop captions.**
   - Eyebrow or kicker labels above titles: "01 · Today's totals", "— Customer stories", "THE SHOP-OWNER PERSPECTIVE".
   - Subtitle paragraphs that restate the title.
   - Reassurance micro-copy under buttons: "No card needed · About 15 minutes per shop · Help on WhatsApp".
   - Meta lines under page titles: date · number of shops · Live. "As of" lines, references disclosures.
   - Small grey text in card corners: "vs last Saturday", "5 items · 3 shops".
2. **The number + title + caption triple** repeated across three columns.
3. **Dividing lines.** None between list items, table rows, stats, footer sections or columns. No decorative rules next to headings, no lines tying sections together, and no line above a profile. Separate with space, or give each item its own card with a soft background.
4. **Sharp or square shapes.** No square cards, sharp ticket or receipt shapes, zigzag torn-paper edges or blocky rules. Nothing in the UI has small or zero radii.
5. **Elements glued to the page edge.** Strips and bars float with margin and full rounding; they don't stick to the bottom or sides.
6. **More than one typeface.** No serif, no italic accent words, no display-font mixing, and no mismatched contrast between font sizes. One sans family.
7. **Random colour.**
   - Only black, white and one accent, with shades of that accent. It must work in both light and dark.
   - No green + yellow pairing, no multi-colour cards, no rainbow tags.
   - Don't colour negatives loudly. Highlight only the primary card, not "Cancelled", and no error banner sitting on top of a card.
8. **Text that acts as a button without looking like one**, for example bare "Review" or "Check".
9. **Inconsistent buttons.** Buttons in one view with different radii or sizes; an arrow on one button and not on its sibling.
10. **Square avatars for people.** People are always circles. Avoid the profile picture + name + caption stack; copy T3 Code's profile area instead (a bare avatar circle that opens a menu).
11. **Clutter.** Tag clouds, nested badges ("2 months free" inside a toggle), tier labels in corners ("1–3 shops"), rating badges in corners, extra calculators, back-to-top buttons.
12. **A sloppy logo or language picker.** No generic letter-in-a-square or stock icon as the logo; use a clean wordmark or a real mark. The language picker is a flag plus a short code (EN, ID, CN), never the full name.
13. **Badly made device mockups** (laptop or phone). Either make them well or leave them out.
14. **Coloured focus or selection marks.** No blue focus highlight, no focus ring, no outline, no darker border on focus, keyboard included. No heavy coloured left border on cards, calendar items or selected rows. No tinted fill plus border stripe for a selected card.

### Always
- **Radii:**
  - Generous: buttons clearly rounded, 12 px. Cards are 16 px.
  - The same radius for every button in a view.
  - Nested radii are concentric: outer radius = inner radius + padding.
  - Tabs, segmented controls, dropdowns and icon-button hover states are rounded too.
  - Charts in one view share the same bar radius.
- **Continuous corners:** every rounded corner is a continuous curve (squircle), never a circular arc that kinks into the straight edge.
  - Web: `corner-shape: squircle` with `border-radius` as the fallback where unsupported.
  - iOS: `RoundedRectangle(cornerRadius:style: .continuous)` / `cornerCurve = .continuous`.
  - Android: a smooth-corner shape.
- **Compact and sized to content.**
  - Metric cards are only as wide as their number needs; a cancelled-sales count needs a small card.
  - Lists don't stretch across the screen. Long text truncates cleanly.
- **Lists that need attention** (low stock and the like): each item is its own small soft card, not separated by lines.
- **Spacing:**
  - Clear, even vertical gaps between rows of cards.
  - Labels sit right next to their controls.
  - Dropdowns have tight padding around the value.
  - Every control in one toolbar row shares one height and one vertical centre: search, buttons, title, segmented picker. Measure alignment; don't eyeball it.
- **Under a title, only useful things:** a control, real data, an icon-led point, or nothing.
- **Copy:** headlines sound human and specific, never generic AI wording. Fewer words everywhere.
- **Icons:**
  - Feather, 1.75 stroke, round ends, 16 px beside 14 px text, the same colour as the text, bare (no containers).
  - Never oversized in lists.
  - Icon + label in navigation; every sidebar item has an icon, sub-items included.
  - The active nav item is shown by the row highlight, not by a filled icon.
  - Use real brand logos (marketplaces, partners) where a brand is meant, not generic icons. Totals need no icon; bold them.
- **Empty states:** one big Feather icon (about 40 px, 1.5 stroke) and a short title. No sentence, no button, no illustration. When a page has no data, show one plain line ("Nothing here yet") and hide what can't act on nothing: search, filters, helper sentences, empty table headers, pager and row counts. Controls come back when there is data.
- **Pricing:** plan name, price, one list of features and one button style. Nothing else.
- **Testimonials:** all the same card size, font and colour.
- **Footer:** calm, grouped by spacing, with no lines, the same type scale as the page. Privacy, terms, language and copyright are fine.
- **Features:** never cut features to simplify; group them. A card shows one primary action; the rest (notes, history, analysis…) live in one grouped menu or behind the open card.
- **Main content first:** the schedule, the list, the table. Explainers, stats and "why" sections go below it or behind a click.

### Visual system (ERP and app UI)
- **Type:**
  - The system font stack, with tabular figures for numbers.
  - Headings weight 600. Big numbers 24 px: they are bold already, so they don't need size.
  - Body 13 px. Labels grey and regular weight, one standard style.
  - The digit "1" must be plain, with no foot serif. Avoid fonts whose 1 has a base line.
- **Colour:**
  - Light by default (older users like white). Dark mode also exists.
  - Off-white page (about `#fafaf9`) with white cards on a soft shadow. Cool greys.
  - Accent blue by default (it varies per product), medium strength.
  - Accent only on primary or key action buttons, such as "Add". The active nav state, charts and numbers stay neutral.
  - Nothing changes colour when clicked.
  - Popovers and previews sit on a darker surface than the page.
- **States:**
  - Hover and focus are the same lighter fill; click makes it a little whiter. No ring, outline or border change.
  - Search field darker at rest, lighter on hover and focus. List row lighter on hover, darker when selected.
  - A selected card gets a soft grey fill, no border.
  - A row's background and its children change at the same instant; no staggered inner boxes.
  - Every button, Filter included, has a visible hover state.
- **Nested menus:**
  - Submenus use a safe triangle so a diagonal move toward the submenu doesn't close it (Costa Alexoglou, Smashing Magazine 2023, after Ben Kamens/Amazon).
  - The safe area expires when the pointer stops and is dropped when the pointer goes back to the parent, like macOS and Radix.
  - Every hover menu also opens on click, tap and keyboard.
  - Popovers from one toolbar never stack: opening one closes the other.
- **Shape and density:**
  - Cards 16 px radius (24 looks better but wastes space in an ERP). Buttons 12 px.
  - Rows 36–44 px, matched to the radius.
- **Status:** a small dot centred on the text, then the text, by default. A soft coloured pill is fine for the one status that needs attention. Never a loud colour per status.
- **Sidebar:** dark, contrasting with the light page. Menus opened from it (account, workspace) use its dark surface, not a white card. No parent items with sub-items when the children can be top-level.
- **Scrollbars:** one style for the whole app, horizontal and vertical alike: thin, soft grey thumb, no track.
- **Charts:** slim bars in shades of the single accent. Run end to end; no 0–100% side labels; legend in a row above.

### Copy
- **Headlines:** short, snappy bold claims, not AI-sounding. For example "All-in-one Shopee and TikTok ERP".
- **Voice:** neutral ("2 shops haven't synced yet").
- **Emoji:** none in product UI or copy, with two exceptions: emoji reactions under comments, and an emoji picker in rich text editors.
- **Money:** full amounts (`Rp 12.400.000`). A short form (`Rp 12,4 jt`) only when space is tight. Missing values stay visible ("N/A" or "—"), never silently dropped.
- **Dates:** relative smart dates ("Today, 14:05"). Otherwise write the month out: "7 Nov 2026", never 07/11/2026, when showing and when choosing dates.
- **Help text under fields:** none. Make the field clear instead. Show validation errors, and help text only when it's truly needed.
- **Feedback after saving:** a toast at the far right that never covers buttons, especially bottom-right actions.
- **Icon-only steppers** (‹ › next to a period chip) say what they step to, with a label or a tooltip showing the range.

### Motion
- About 220 ms with ease-out.
- **Presses:** a small shrink, and nothing else on the page moves.
- **Pages:** slide, only for real page changes. Sheets ease out.
- **Lists:** staggered, but fast enough that nobody waits.
- **Tabs:** the segmented-control pill slides.
- **Hover:** cards lift slightly.
- **Totals:** count up only where the data really is real-time.
- **Loading:** a pulsing skeleton, no spinners, under 0.5 s to first content.
  - Every skeleton matches the final layout exactly: the same boxes, sizes and positions, including each small card in a row, so nothing shifts when the data arrives.
  - Every loading state has one. Check before, during and after loading.

### Phone
- Bottom tabs with icon + label, and a floating button for the main action.
- **Header:** the main context picker (for example the shop) can be the header; it varies per app.
- **Choosing a shop or similar:** a full-screen list.
- **Details:** open as full pages.
- **Filters:** dropdowns.
- **Nested and focused:** one concern per screen, with options nested rather than crammed together.
- **Tables:** compact rows, never cards, because cards scroll too much. Avoid big tables on phone; often a summary is better.

### Components
- **Detail and create views on desktop** open in a side pane or a modal, never a full page. Phone still uses full pages.
- **Toggles:** a circular thumb inside a pill track. Never a square inside a pill.
- **Error and alert icons** align with the first line of text, never centred on a two-line message.
- **Dropdowns:** every one is custom, one reusable component used everywhere. Never the native `<select>` look. It matches the 12 px controls and continuous corners.
- **Search:** one search bar component across the app, same height and radius everywhere.
- **Save buttons:**
  - If the form fits on one screen, Save goes at the bottom, not the top right.
  - If it scrolls, unsaved changes must be obvious, for example a sticky save bar. Leaving with unsaved changes asks first.
- **Settings pages:** titled groups of rows on soft cards, no lines, status as dot + text, the whole row opens its dialog, no "i" tips, quiet footer links.
- **Shared components:** filters, toolbars, table headers and page headers come from the app's shared set, never a page-local version.

### Data pages and tables
- **One page skeleton everywhere:** page header (title, then toolbar: search, source, Filter), the table, and a bottom bar with pagination and the row count. The header is identical in structure, size and position on every page.
- **Tables:**
  - Dense rows, no wasted padding. No row lines; use row backgrounds or spacing.
  - Columns sized to their data, so statuses and values don't truncate.
  - Fill the screen height. Sticky headers never overlap rows.
  - One header style across every table.
  - More than a page of rows gets the bottom bar (count + pager, 50 per page). No "show more" buttons, no unpaged 200-row tables.
- **Clicks:** a whole-row click opens the detail pane. No per-cell modals. Clicking an item never jumps to another tab.
- **Summaries are filters:** a "by reason" chart or a totals row filters the list under it.
- **No hidden tables:** never put a data table inside a disclosure box; show it as a section.
- **Product pictures:** every product shown anywhere has its picture.
- **Check columns stay:** columns people use to check numbers (money, differences) are visible by default. Colour a difference green or red only when there is one.
- **Money rows say who pays:** a fee or charge row gets a left icon or logo plus a short label (buyer, platform, company) and is coloured by direction.
- **Long reports:** charts and the summary first; detail tables behind one segmented switch (a dropdown on phones), one table at a time. Drop a table that only repeats numbers shown elsewhere.
- **Calendars:** fit the whole month, week or day on one screen without scrolling. Search sits at the top of the filter panel.

### Things the reviewer liked
- A real product screenshot as the hero of a section.
- A "Live total today" card with small cards under it.
- Rounded bento cards of varied sizes: "very modern".
- A closing call-to-action card with a concrete time ("Tomorrow at 7 a.m.").
- A Today / Week / Month segmented selector.
- An illustration on the right of a landing-page hero.

---

## Part 2: The reviewer's words
This is the source of Part 1. Read it when a rule there is unclear or a case isn't covered: the reasoning is here.
- The feedback was dictated by voice. Obvious transcription slips are fixed, and editor notes are in [brackets]. Otherwise the wording is the reviewer's.
- Screens A–J are two AI-generated landing pages (A–E site one, F–J site two) for "Tally", a made-up sales and stock app for shop chains. Site one was liked much more; site two was "even more terrible".

### How the reviewer talks
- **Direct and plain.** "I don't like…", "that's bad", "this one's much worse", "I like this a lot", without softening. Do the same in critiques: name the thing, say what's wrong, say the fix.
- **Recurring words:**
  - "AI slop" / "AI-like": generic filler copy and decoration.
  - "random captions": text no one needs.
  - "border radius" / "border radii": how round things are, and whether they match.
  - "concentric" / "standardized" / "syncs with": matching shapes.
  - "too blocky", "too squarish", "sharp": hard edges and lines.
  - "classy" / "modern": rounder and calmer.
  - "messy" / "chaotic": too many fonts, colours or sizes.
  - "cramped" / "too much space": density.
  - "UI rules": a system, not one-off choices.
- **Practical about trade-offs.** Likes something, then picks what works for an ERP: "I like D a lot but it's not good for ERP because it takes away so much space". Show the ideal and the practical choice side by side.
- **Thinks about real users.** "Our old clients like white", "they want to see things", "we have to really concentrate on what's on the screen at a time".
- **Accepts "it depends".** Many answers come with a condition ("this will vary", "depends on the app"). Keep those conditions.
- **Reacts to examples, not abstractions.** Show pictures, give options letters, and let the reviewer answer "for A, …".

### Critique of the AI landing pages
"This will be some UI critique for a landing page. This may be different for a lot of things from ERP software, but we'll take the feedback anyway."

**A (site one: nav and hero)**
- I don't like how the Get Started button on the top right has a very small border radius. I need it to have a larger border [radius].
- In the header area I don't like how the title is very AI-like. The wording is very AI-sloppy. I also don't like how there are too many captions underneath, for example "Sales, stock, and the small details that matter. Together in one place, wherever your day takes you." All that needs to be removed and made a little bit better.
- The "See Tally in action" button also needs a better border radius that syncs with the Get Started button.
- Below that there are more captions below the button, and those need to be removed as well.
- We only want creative captions under the title, for example with some icons or with some actual usable things, not just random AI slop text.
- I like how there is an image on the right. However, the "Today across your shops" card has a squarish border radius, which I don't like. It's different from the UI style.
- The shadow behind that, and the SVG below it with the torn paper and the zigzag, look very rough.
- If we use a better border radius, I want it to be a full border radius, not stuck to the page bottom. The "Less checking in, more moving forward" strip should not be attached to the bottom.
- The lines and everything are too squarish, and the icons in the bottom-right part are different. The lines between them are too square and sharp, and the icons are a different size and a bit too big as well.

**B (site one: features)**
- This looks pretty good, but it's a bit too complicated with all the receipts coming together. The icons on each receipt are a little weird. The arrow pointing to "Live total today" has a broken arrowhead. But "Live total today" and the little cards below it are kind of nice.
- The bottom part with the three things ("Sales together", "Stock in sight", "Catch the exceptions") is very AI-like. I don't like the straight lines separating them. And I don't like having the same three things every time: the number, the title, then the caption. I usually want to provide more value than random captions. UI-wise this is not too bad.

**C (site one: product showcase)**
- I like this one a lot. However, I don't like the lines next to "A good day, at a glance". They feel unnecessary and too sharp.
- The screenshot of the ERP is quite good. However, the Overview button needs a better, larger border radius, and it should sync with all the cards inside the overview page.
- I don't like the captions below the Overview title: just the date, the number of shops and the live indicator. We have to fill it with something more useful than that.
- In the top right, the icons need a better border radius for their shading when you click them.
- I like Total sales, Transactions and Cancelled sales, but they're too wide. Cancelled sales will never be a big enough number to need that much space, so there's a spacing issue.
- The two Review buttons should not be buttons without proper button styling.
- On the sales chart I need a better border radius on the tab. The bars themselves are too wide; they need to be sleeker.
- "Stock needing attention" is the classic cards separated by lines. I don't like that. Each one should be its own card, maybe with a background. It also takes too much space horizontally, and it should handle text truncation.
- The store performance table is terrible. It takes way too much space and has padding between items. I don't like how it just has lines between them, not really separated properly.

**D (site one: pricing)**
- There are captions everywhere: below the first title and below the tiles under each package. Other than that it looks okay.
- The border radii are, once more, a little too small. I need them a little larger.
- The icons are still a bit too big for every point in each package.
- At the bottom, the selector for the number of shops needs better UI. The dropdown has too much padding beside the number. The "Number of shops" label and the line to the left of "Essentials" are a little too far apart in general.
- The colour choice has been okay, but I'm not a big fan of green and yellow. Colour choice is always easy to make. I prefer more dark mode and pure light mode, with UI rules on just the colours you choose. I just want black, white and an accent colour, and it should work in both dark mode and light mode.

**E (site one: stories, CTA, footer)**
- Profile images should always be circular for humans.
- I don't like the line starting to the right of the profiles.
- I don't like the top-left corner [the "THE SHOP-OWNER PERSPECTIVE" eyebrow], because it's random text.
- I don't like the last hero section, because it has another button, needs more border radius, and has random captions as well.
- One of the main things I don't like is the random captions AI puts around.
- In the footer there are lines between every section, like between the logo and "A clearer day for every shop", and on the right side, which doesn't need any lines.
- The back-to-top button should not live there, if we even need one.

**F (site two: nav and hero), "even more terrible"**
- I don't like the font. There are too many different fonts and colours.
- I don't like the italic one. I don't like the serif font.
- The caption is way too big ("Tally reads the till in each of your cafés…").
- There's a caption and a line above the title area. That's bad.
- The logo is bad.
- The language selector is different too. It should just be a flag with the language you selected, opening a dropdown.
- The border radii here are way too varied. "Start free trial", "Start free for 14 days" and the dashboard one are not the same.
- Below that you see "No card needed", "About 15 minutes per shop" and "Help on WhatsApp". That is not needed at all.
- The numbers below are separated by lines. Too blocky.

**G (site two: features)**
- Again, the variety of fonts is not good.
- I like the border radii of the cards already; they're interesting.
- I don't like the caption above each title, like "01 Today's totals" or "02 Best and worst shops".
- The UI for each card is pretty good. But the bar graphs in the first and second cards don't have the same border radii. Concentric borders and standardisation are very important, and so are colours. The colours here are all random. We should use proper accent colours and shades.
- The laptop and phone in 05 are not properly made.
- In 06 I don't like the number of tags; they're all messy.

**H (site two: product showcase)**
- I don't like the random use of colour and italics, the different fonts, or the line from outside Tally to inside Tally. The app itself looks not bad.
- There are too many colours. The border radii are off for a lot of things, such as the top-left area.
- I don't like the Today, the date and the live sync next to the profile image and logo. They don't need to be there.
- It needs more spacing between cards, from "Sales so far" and "Transactions" to "Average basket", and below that to "Sales by hour". The vertical spacing between them is not good.
- I really like the Today / Week / Month selector, but I don't like the "vs last [Saturday]" area.
- We have different background colours for different cards. Highlighting the first one is good, but don't highlight the cancelled one. Buttons like "Check" without real button UI are bad.
- The chart looks okay. "Shops, best to worst" is too cramped and needs more padding. For cancelled sales, I don't like the error sitting right on top. That should not be there.
- We don't need the top-right text on each card, for example "vs last Saturday", "14 today", "Rp 1.212.000", or "5 items · 3 shops".
- I don't like the line above the owner at the bottom left. And I always feel the title-and-caption-below combo next to a profile image is not the best. Copy T3 Code for this if needed.

**I (site two: pricing)**
- Again, a lot of fonts and too many colours.
- At the top right, Monthly and Yearly have a nested "2 months free", which I don't think is needed.
- Text like "1–3 shops" and "20+ shops" should not be at the top right.
- There are too many captions under and above the prices.
- The border radius on "Start free trial" doesn't look good. One has an arrow and one doesn't.
- The list with icons below is fine, but not the most user-friendly.
- The "9 shops / Growth" calculator at the bottom right should be removed, and so should everything with "14 days free on any plan".
- It has to be more simple and focused.

**J (site two: stories, CTA, footer)**
- Again, too many fonts and colours.
- The rating should not be in the top right. The "— Customer stories" label at the top left should be removed.
- Every user-review card is a different size, a different colour and a different font. It's very messy.
- I do like that there are different cards with rounded corners. This is very modern. The "Tomorrow at 7 a.m." card looks good.
- The icon is in the middle of nowhere.
- The buttons ("Start free for 14 days" and "Chat with us on WhatsApp") are different sizes. We have to fix that. The border radii feel very off.
- The footer is messy and chaotic. There's text everywhere with no clear divisions. There's a large line I don't like because it's blocky.
- Privacy, terms, language and the copyright are fine.
- The fonts, like "Product / Works with / Company / Help" against the text below, clash: the contrast across the number of fonts is insane.

### Notes behind the picker answers
**Icons**
- Feather, the same feel as T3 Code. "Line ends round, yes."
- 16 px "depends on the icons we're using", so it was re-picked in Feather.
- Empty-state art: "I don't like the empty-state art yet. There's still a little too much text." A big icon and a short title only.

**Type and colour**
- **The "1":** "I like the typeface that has the number 1 without the bottom line. None of the options had this, so I just picked the first one" [the system font].
- **Big number:** "the smallest, because it's already bold, so it doesn't need to be too big, especially for an ERP".
- **Labels:** the lighter one, "and make it more standardised rather than having another thinner font".
- **Accent:** "this will vary, but let's default to blue". Medium strength: "not too contrasting and not too grey".
- **Greys:** "I like the cool one. The warm one is actually much more stylish, but for ERP the cool one is fine."
- **Page background:** "off-white, because it gives more contrast for all the different cards. Light grey is just too grey."
- **Theme:** "light mode, because our old clients like white, and dark mode mostly for myself."
- **Rows:** "something between 1 and 2 [36–44 px]. It has to match the border radius as well."
- **Card radius:** "as round as possible. I like D [24 px] a lot, but it's not good for ERP because it takes away so much space. I settled on B [16 px] because it has the most utility but still looks classy."
- **Buttons:** "more round. The more round, the more classy, at least nowadays. But combined with how much space it takes, so I took the middle ground [12 px]."
- **Status:** "I like C [soft pill] a lot. That's what a lot of us use, but if we execute dot + text it'll be much better, especially if the dot is a bit smaller and more centred with the text."
- **Sidebar:** "I really like the contrast", so dark.
- **Accent use:** "I want to reserve accent. I don't like clicking on things and having them change colour. I really like A [buttons only], but we can add it to more of the action buttons we need, for example adding a new thing."

**Copy, motion and phone**
- **Toast:** "not too interruptive. If there are buttons in the bottom right, toasts usually just cover them."
- **Headline:** "a bold claim, but not as AI as this. Short and snappy, for example 'All-in-one Shopee and TikTok ERP'."
- **Money:** "depends on the space we have. Full is best, but if there's no space, the short version."
- **Dates:** "relative smart dates are the best. If not, the first one with the month written out, so there's no confusion. This is for displaying dates, choosing dates, everything."
- **Emoji:** "none at all, ever." Later: "Emojis under comments are allowed… That's the only place we will allow emojis. Also in the rich text editors, we allow that as well."
- **Help text:** "I'd prefer never. If there's a validation error, show that, and if it's really needed you can show it, but I'd prefer never as much as possible. Make it as clear as possible."
- **Press:** "shrinking a little bit, but make sure nothing else in the UI moves."
- **Page change:** "I like the sliding a lot, but only for certain things, when we actually change the page."
- **Lists:** "one after another, but fast enough that they don't have to wait too long."
- **Numbers:** "counting up. But we may not have real time for all of these, so be careful."
- **Skeletons:** "I like the pulse. But a rule: skeleton loaders have to be exactly the same size as the UI that will come out, because we should know what the UI looks like. Before, during and after, it must fit the exact shape of every div."
- **Phone tables:** "very difficult. Avoid as much as possible, but it depends on the usage. If there are a lot of rows, they want to see things. Usually maybe just do summaries. I'd prefer compact rows instead of cards, because cards need way too much scrolling."
- **Phone screens:** "more nested. Have everything and the options more nested, because we have to really concentrate on what's on the screen at a time."
- **Corners:** "continuous curves on border radiuses, no abrupt changes."

### Test builds that followed this skill
**A landing page:** "This one, the landing page, is extremely tasteless. With all the UI design skills and everything, it's meant for an ERP system, not for building a nice landing page that is interesting." "The UI is good, as in it has less clutter, but it needs some flair, like every landing page does. For example my personal website has extra graphics, a running theme and a storyline."

**A dummy ERP (screens E1–E37):** "Other than that it looks good."
1. E31: two-line error messages look weird, because the "!" icon is centred vertically.
2. E35: toggles are squares inside pills? Looks off.
3. E37: the profile pop-up is white and looks off next to the black sidebar.
4. E11: I don't like full pages for items. I like panes or pop-ups. Same for New product.
5. E6: the name in the top left. I don't like the icon.
6. E35: the toast isn't at the far right? And why is the Save changes button at the top right? If it fits on one page, the rule is to put it at the bottom. For scrollable pages, make sure saving before exiting is obvious.
7. Dropdowns: are they all custom? Make this a rule, and make sure it's a reusable component too.
8. E28: the skeletons for Transactions, Average basket, Cancelled and To ship are not the same size?

**A job-queue dashboard tidy-up:** "I don't like the new side by side. I like the old one. I wanted it to remove a lot of the text, that's all, but it kind of failed." After a first cut of 17 strings it was still too much text; what was left included "Last decision: memory pressure/OOM; retry", "8.4 GB free to admit of 14 GB" and "RAM 10.4 available, 2 reserve | pressure normal | heartbeat 32s ago". [Lesson: "less text" means much less. Raw system strings, repeated facts and debug stats move into hovers. Each fact appears once, in plain short words.]

### Live app reviews
**Sales ERP, first review (J1–J8)**
- J1: "header issue when scrolling." The sticky table header overlaps the rows.
- J2 (order pane): "the products section ui needs work." The Products block is a grey box, and quantity and price run together ("1IDR 87,000").
- "main sales page loses a lot of columns as well, for checking the differences etc." [The redesign cut the default columns to six. The money columns are used to check differences, so they stay visible by default.]
- J3: "any part with product needs to have picture pls."
- J4: "clicking on cancellation reasons by reason section dont do anything?" [Every visible summary row should filter its list.]
- "search bars are not the same throughout. filter button hover not there, custom dropdowns need to be standardized, make sure loading is sub 0.5s as usual"
- J5: "how come there is order details dropdown as a table?" [A table hidden inside a disclosure is wrong; show it as a section.]
- J6: "ugly border when focusing on search bars."
- J7: "make tables full height in screen, and make rows less tall here."
- J8: "no icons on side bar?"
- On process: "logic from previous version should not have changed, only UI should have changed." "do less tests, only isolated tests if changing logic." "be critical."

**Sales ERP, second review**
- Remove captions like "Display & references", "Fee split per product (i)", "May be out of date · <date> Details" and "Cancelled orders · by order date". An ops banner for stopped syncs stays.
- No "Sales" parent with sub-items; its children are normal top-level items with icons.
- "their table headers are styled differently; pick one style and use it everywhere." The page header must be identical in structure, size and position on every page.
- A cluttered favourites page keeps the few functions that matter and loses secondary controls and explanations.
- "No captions, no explanatory lines, no 'as of' lines; text only what's needed."

**Internal ops app**
- "focus or highlight when clicking it it highlights in blue, can you disable repo wide focus blue highlights. i hate that so much"
- Grey states: search dark at rest, light on hover and focus; list row light on hover, dark when selected, "so that the colors match when I'm not hovering over anything".
- "height of logo must be same as the title + caption" [measure the real line boxes].
- Follow-up: "remove focus rings entirely. just make the color whiter when clicked".

**Sales ERP, empty phone page**
- "this needs a lot of ui work. too much random functions and stuff for nothing showing up. be more clear, just say nothing is there yet."

**Sales ERP, reports**
- "reports page need simplification. tables too big and no pagination". Charts and the summary on top with every detail table behind one segmented switch, 50 rows per page, was approved; the page went from 21,957 px to 2,378 px tall.

**Sales ERP, third review**
1. "horizontal vs vertical scrollbars need to be same. make it like the vertical one. for the entire app, all round reuse the component styles."
2. "if i click filter then columns, it will overlap. always one or the other"
3. (Bare ‹ › next to a week chip) "these buttons need more context for prev and next week. make sure the ui is clean though"
4. "what happened to our N/A values? all gone? hidden?"
5. "no differences column anymore? that was a main function. color if there is difference, green or red."
6. "settings page ui needs another ui pass, its weird and not according to style" … "i dont like border when focused. remove borders when focused."
7. "I don't want this modal to show when I click on certain cells. I want the whole row click to show the pane. that means you have to fix certain columns. For example the status column needs to be a bit wider because some of the statuses get truncated"
8. "order-level fees here should be clear about which ones are paid by the consumer, by the platform, or by the company itself. You should label them. Put an icon, perhaps on the left side, and then for whether it's negative or positive, use green and red to color-code it here."
- Later: "you need to use the marketplace logo and the company logo, not just icons pls. and for totals no need icon, just bold them. for shipping use an icon is fine"

**Leads app, second UI pass**
- "the top bar is okay, but there are way too many. There's lots of text everywhere there."
- "when I click on them, the new leads will have a background and a left border, which needs work. For every single one of the cards that open, there is way too much text everywhere."
- "Tagging has a lot of buttons split here … DM, Send, Add notes, etc., AI analysis, History. … We should not reduce features, but we should just group them properly and make the UX better."
- "There is a title, caption, filter, the 'Why we post' part, more numbers before we actually see posting times, automation. After that we actually see the schedule."
- "you should put more items behind the click if possible. Also when I click it, it goes back to the Today page."
- "Please make sure the UI elements, such as the filters, are consistent with all the reusable ones."
- "We also need proper skeleton loaders for everything."

**UI terms review**
- "i dont like full names of languages, i like "EN" and "CN" better, like the abbreviations. make that a rule too."
- On a selected card shown with an outline: "i dont like the borders."
- "for pills i think its fine, colored pills sometimes is worth doing."

**Calendar**
- "there's too much padding vertically." "Make sure that the entire calendar fits within my screen without having to scroll." The same for Week and Day.
- The filter panel "needs proper restructuring. For example the search bar has to be on top." "Make it more simple as well please."
- The controls "need proper styling, and also the height of the buttons." The view picker buttons "are not the same."
- On a polish-only patch: "still needs a lot of work. reorganize where things should be."
- On the chosen layout: "search bar and today, november, day, week, month, schedule, are not aligned vertically" and "each item in the calendar must NOT use the heavy left border."

---

## Part 3: Principles
91 chosen from 100 candidates, plus UI-15 and UX-51 added later (93 in all). IDs are stable. Cite a principle's ID in an audit or critique when it explains a problem.

How to use them:
- **Editing an existing tool (default):** they are a lens for finding and explaining problems. They never license a restyle.
  Where a principle is a style choice (UI-16, UI-17, UI-24, UI-25, UI-44), the product's existing choice wins.
  The defect is breaking that choice inconsistently. A principle the product doesn't follow becomes a suggestion.
- **Redesign (only when asked):** they are the direction. Variants should follow them.
- Skipped on purpose, so don't add them back: closure, line height 1.4–1.6, squint test,
  golden ratio, F-pattern, Zeigarnik, endowed progress and the Fogg model.

### UI: how it looks

- **UI-1 Proximity** (Wertheimer). Things close together read as a group. Group with space, not lines.
- **UI-2 Similarity** (Wertheimer). Things that look alike read as the same kind. All tappable text shares one look.
- **UI-3 Common region** (Palmer). Group with a shared soft background instead of a border around each item.
- **UI-4 Figure and ground** (Rubin). Sheets and dialogs need a dim backdrop so it's clear what is on top.
- **UI-5 Alignment and continuity.** Content shares left edges. Every extra edge is one more thing to track.
- **UI-7 Hierarchy by size, weight and colour** (Refactoring UI). The key number is big and dark, and its label is small and grey.
- **UI-8 Type scale.** Font sizes come from one fixed scale, for example a 1.25 ratio: 12, 15, 19, 24, 30.
- **UI-9 Line length 45–75 characters** (Bringhurst: "Anything from 45 to 75 characters is widely regarded as a satisfactory length of line.").
- **UI-11 8-point grid.** Gaps and sizes are in 4 or 8 point steps.
- **UI-12 Inside spacing smaller than outside.** A label sits closer to its own field than to the one above it.
- **UI-13 Nested corner radius.** The outer radius equals the inner radius plus the padding. The same radius inside and out looks pinched.
- **UI-14 One family of radii.** Two or three radii across the app, for example 8 for controls and 16 for cards.
- **UI-15 Continuous corners (squircle).** Corners curve continuously into the straight edges, with no kink. See Part 1 for how to build them.
- **UI-16 Circles for people, rounded squares for things.** Avatars are circles. Shops, products and apps are rounded squares.
- **UI-17 Pill vs rounded-rectangle buttons.** This is a style choice: pills feel friendly and rounded rectangles feel like a tool. Pick one for the whole app.
- **UI-18 60-30-10 colour.** About 60% neutral background, 30% secondary surfaces and 10% accent. The accent is for actions and active states only.
- **UI-19 Contrast of at least 4.5:1** (WCAG 2.2 AA). Large text needs 3:1. No light grey on white for content.
- **UI-20 Colour is never the only signal** (WCAG 1.4.1). Pair colour with an icon or a word.
- **UI-21 One neutral ramp** (Refactoring UI). Five to eight planned greys, not a new grey picked by eye on each screen.
- **UI-22 Tinted neutrals** (Refactoring UI). Greys carry a slight warm or cool tint.
- **UI-23 No grey text on coloured backgrounds** (Refactoring UI). Use a tint of the surface colour, or white with transparency.
- **UI-24 Use fewer borders** (Refactoring UI). Separate with space, a background shift or a soft shadow before adding a line.
- **UI-25 Soft, layered shadows.** A tight shadow plus a wide soft one from one light source above. Never a single heavy grey blur.
- **UI-26 A fixed elevation scale.** Three or four shadow levels, each with one job: resting card, raised menu, dialog.
- **UI-27 Tabular figures** (OpenType `tnum`). Numbers in columns or live counters use equal-width digits.
- **UI-28 Right-align money.** Amounts line up by their last digit.
- **UI-29 Optical alignment.** Centre by how things look, not by their box. A play triangle moves right.
- **UI-30 Overshoot for round shapes.** A circle is slightly bigger than a square of the same visual size.
- **UI-31 One icon style.** The same stroke width, corner style and size grid everywhere.
- **UI-32 One primary action per screen.** One filled button, with quieter styles for the rest.
- **UI-33 Emphasise by de-emphasising** (Refactoring UI). Make the other items quieter instead of making the active one louder.
- **UI-34 Labels above fields** (Wroblewski). A placeholder is never the label.
- **UI-35 Start with too much white space** (Refactoring UI). Cramped is a defect, and airy is the default.
- **UI-39 Z-pattern for sparse screens.** Top-left, top-right, diagonal, bottom. The action goes at the end.
- **UI-40 Dark mode is not pure black** (Material). Very dark grey with off-white text.
- **UI-41 Softer colours in dark mode** (Material). Use lighter, less saturated accents. Saturated colours vibrate on dark backgrounds.
- **UI-42 Letter-spacing by size.** Tighten big headings slightly and loosen small all-caps labels.
- **UI-43 No all-caps sentences.** Capitals only for labels of a word or two.
- **UI-44 At most two typefaces.** One family with a few weights covers almost everything.
- **UI-45 Data-ink ratio** (Tufte: "Above all else show the data."). No chart gridlines, boxes or decoration that carry no data.
- **UI-46 Label lines directly** (Tufte, Few). Put the name at the end of each line instead of in a legend.
- **UI-47 Ease-out for things that enter.** They start fast and settle gently. No linear UI motion.
- **UI-48 Short motion, 150–300 ms** (Material, Apple). Small changes finish in about 200 ms.
- **UI-49 Skeletons instead of spinners.** Show the shape of the coming content, and no layout jump when it arrives.
- **UI-50 Isolation effect** (Von Restorff). The one thing that looks different gets remembered. Keep it to one per screen.

### UX: how it works

- **UX-1 Fitts's law** (Fitts, 1954). Make important targets big and near. Tap targets are at least 44 pt (Apple) or 48 dp (Android).
- **UX-2 Hick's law** (Hick, Hyman). Each extra choice slows the decision. Show a few and put the rest behind "More".
- **UX-3 Chunking** (Miller: "The magical number seven, plus or minus two"). Group long numbers and codes, for example 0812 3456 7890.
- **UX-4 Jakob's law** (Nielsen: "Users spend most of their time on other sites."). Put things where other apps put them.
- **UX-5 Tesler's law.** Some complexity can't be removed, only moved. The app carries it, not the user.
- **UX-6 Doherty threshold** (1982). Respond in under about 400 ms, or show progress.
- **UX-7 Peak–end rule** (Kahneman). People remember the best moment and the ending. Finish flows well.
- **UX-8 Serial position.** The first and last items are remembered best. Put key items at the ends of menus.
- **UX-10 Goal gradient** (Hull). People speed up near a goal. Show how close they are.
- **UX-11 Aesthetic–usability effect** (Kurosu, Kashimura). People find polished interfaces easier to use and forgive small problems in them.
- **UX-12 Postel's law** ("Be conservative in what you do, be liberal in what you accept from others."). Accept 1250000, 1.250.000 and 1,25 jt.
- **UX-13 Occam's razor** ("Entities should not be multiplied beyond necessity."). Of two designs that do the job, keep the one with fewer parts.
- **UX-14 Pareto 80/20.** The few features used most are the fastest and most obvious.
- **UX-15 Parkinson's law.** A task fills the time it is given. Autofill and remember the last-used choice.
- **UX-16 Choice overload** (Iyengar, Lepper). Offer a few good presets instead of many options.
- **UX-17 Cognitive load** (Sweller). Show what the task needs and nothing more.
- **UX-18 Working memory** (Baddeley). Never make users carry information from one screen to the next.
- **UX-19 Progressive disclosure** (Nielsen). Basics first, with advanced options on request.
- **UX-20 Recognition over recall** (Nielsen #6). Let users pick from recent or visible items instead of typing from memory.
- **UX-21 Visibility of system status** (Nielsen #1). Always show what happened and whether it worked.
- **UX-22 Match the real world** (Nielsen #2). Use the user's words, not the database's.
- **UX-23 Undo instead of "Are you sure?"** (Raskin: "Never use a warning when you mean undo.").
- **UX-24 Consistency and standards** (Nielsen #4). The same action has the same word, place and look everywhere.
- **UX-25 Error prevention** (Nielsen #5). Make mistakes impossible, for example with pickers and limits instead of free text.
- **UX-26 Shortcuts for experts** (Nielsen #7). Keyboard shortcuts and a command bar that don't get in anyone's way.
- **UX-27 Errors explain the fix** (Nielsen #9). Say what went wrong in plain words and what to do next.
- **UX-28 Signifiers** (Norman). Anything tappable looks tappable.
- **UX-29 Feedback on every action** (Norman). A pressed state, then progress, then the result.
- **UX-30 Natural mapping** (Norman). Controls sit next to what they control, for example filters directly above their table.
- **UX-31 Constraints** (Norman). Inputs accept only valid values, for example a quantity that stops at 0.
- **UX-32 Mental model** (Norman). Organise things by how users think: by day and by shop, not by table.
- **UX-33 Smart defaults** (Johnson, Goldstein). The default is the right answer for most people, for example Today.
- **UX-34 Numbers need context** (Tversky, Kahneman). Compare a number with yesterday or last week.
- **UX-35 Paradox of the active user** (Carroll, Rosson). No long tours. Teach in place, at the moment it matters.
- **UX-36 Optimistic UI.** Show the result now, sync in the background and roll back only on failure.
- **UX-37 Validate after the field** (Wroblewski, 2009). No errors while the user is still typing. Check when they leave the field.
- **UX-38 Empty states lead somewhere.** Say why the screen is empty and give the next step.
- **UX-39 Thumb zone** (Hoober). Main phone actions sit in the bottom half.
- **UX-40 Banner blindness** (Benway, Lane). Important notes go inline, next to what they affect, not in banners.
- **UX-41 Actions next to their object.** Row actions are on the row, not in a distant toolbar.
- **UX-42 Don't make me think** (Krug). Labels say exactly what will happen: "Save sale", not "Proceed".
- **UX-43 Omit needless words** (Strunk). Halve the words, then halve them again.
- **UX-44 Least astonishment.** Things do what users expect. Closing a form keeps the draft.
- **UX-45 Kano model** (Kano). Basics before delighters. Missing basics hurt and extra delight doesn't make up for them.
- **UX-46 Flow** (Csikszentmihalyi). Match the challenge to the user's skill, neither boring nor overwhelming.
- **UX-47 Labour illusion** (Buell, Norton). During waits, say what is being done: "Adding up 1.240 sales from 3 shops…".
- **UX-50 Fewer steps** (keystroke-level model; Card, Moran, Newell). Count the taps. Every step removed is saved many times a day.
- **UX-51 Safe triangles for submenus** (Alexoglou, Smashing Magazine 2023; Kamens/Amazon 2013). Moving diagonally toward a submenu keeps it open. The safe area expires when the pointer stops. Hover menus also work by click and keyboard.

---

## Appendix: Landing-page reference style
A personal portfolio site that the landing-page mode is modelled on. It is the landing-page taste reference, not the app reference.

**Tokens**
- **Background:** `#0a0a0a`, flat, no gradient anywhere.
- **Text:** warm off-white `rgb(233,228,218)`, never pure white. Muted text is cool grey `#9a9aa4` / `#8f8f9a`, with dimmer `#63636c`–`#75757e`.
- **Accents:** one colour per project, used only in the project's small label and its progress dashes, for example purple `#8b7bff`, green `#5fd39a`, pink `#d96bb1`, orange `#f0a150`, blue `#6fb3f2`.
- **Type:** three voices.
  1. A handwriting face (Caveat), 500–600 weight, for the name, section titles and first-person headlines.
  2. System sans for body text, 13.5–16 px.
  3. Monospace, 9–11 px, UPPERCASE with 1.1–1.8 px tracking, for meta labels, dates, nav and links.
- **Radii:** almost none. 0 everywhere, 2–3 px on small chips, 7–10 px on photo tiles, circles for dots.
- **Shadows:** none. **Borders:** hairlines only.
- **Layout:** a text column about 540 px wide on the left third. A large single-line drawing is fixed on the right. Each work item fills one viewport.
- **Navigation:** a fixed right rail of tiny mono labels, each with a bar whose width marks position. No top nav bar.
- **Motion:** opacity and transform only, 0.25–0.35 s, on the rail and hover. No scroll-jacking, no entrance animations.

**What defines the look**
1. **Dark, flat and almost empty.** One colour plane, no cards, no boxes, no shadows.
2. **A handwritten headline voice** that gives warmth against the technical mono.
3. **First-person claims as headlines,** short and concrete, with a number where there is one.
4. **One line-art drawing** as the only illustration: continuous strokes, no fill, fixed while the content scrolls.
5. **Mono uppercase meta labels**, small and tracked, in the project's accent colour.
6. **Colour is a signature, not decoration.** Each project gets one hue, used in two tiny places only.
7. **One idea per screen,** with a lot of empty space.
8. **Quiet navigation:** the right-edge rail replaces a header.
9. **Real logos and real store badges** instead of generic icons.
10. **Data shown honestly:** a thin-line chart with direct labels and no gridline clutter.

**Where it breaks from SaaS template defaults**
- No gradient hero, no glow, no glassmorphism, no rounded cards, no drop shadows, no icon grid of features.
- No top nav bar, no CTA button. Contact is a plain mono link list.
- No stock photos; only real photos, as small tiles.
- Copy is personal, first person and specific, not "Empowering teams to…".
- Small type everywhere except the headlines. Hierarchy comes from the typeface, not from size jumps.

**Carry over** the restraint (flat, no cards or shadows), warm off-white on near-black, mono meta labels, one accent per subject, concrete copy, and one idea per screen. The handwriting face is a personal-site signature; ask before using it in a product.
