# UI feedback, in the reviewer's words

This is the source of `taste.md`. Read it when a rule there is unclear or a case isn't covered: the reasoning is here.
- The feedback was dictated by voice. Obvious transcription slips are fixed, and editor notes are in [brackets]. Private names (clients, shops, products, internal apps) are replaced with generic ones in [brackets]. Otherwise the wording is the reviewer's.
- Screens A–J are in `references/ai-site-critique/`. A–E are site one and F–J are site two. Both are landing pages for "Tally", a made-up sales and stock app for shop chains.
- The pickers that were answered are summarised in `references/answers.md`.
- Add new feedback at the end, under a dated heading, with the screen letters it refers to.

## How the reviewer talks, and how to write for them
- **Direct and plain.** "I don't like…", "that's bad", "this one's much worse" and "I like this a lot", without softening. Do the same in critiques: name the thing, say what's wrong, say the fix.
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
- **Practical about trade-offs.** Likes something, then picks the option that works for an ERP: "I like D a lot but it's not good for ERP because it takes away so much space". Put the ideal and the practical choice side by side.
- **Thinks about real users.** "Our old clients like white", "they want to see things", "we have to really concentrate on what's on the screen at a time".
- **Accepts "it depends".** Many answers come with a condition ("this will vary", "depends on the app"). Keep those conditions; don't flatten them into absolutes.
- **Reacts to examples, not abstractions.** Show pictures, give options letters, and let the reviewer answer "for A, …".

## Critique of the AI landing pages
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
- We don't need the top-right text on each card, for example "vs last Saturday", "14 today", [an amount], or "5 items · 3 shops".
- I don't like the line above the owner at the bottom left. And I always feel the title-and-caption-below combo next to a profile image is not the best. Copy [the app-chrome reference] for this if needed.

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

## Notes behind the picker answers
**Icons**
- Feather, the same feel as [the app-chrome reference].
- "Line ends round, yes."
- 16 px "depends on the icons we're using", so it was re-picked in Feather.
- Empty-state art: "I don't like the empty-state art yet. There's still a little too much text." A big icon and a short title only.

**Type and colour**
- **The "1":** "I like the typeface that has the number 1 without the bottom line. None of the options had this, so I just picked the first one" [the system font].
- **Big number:** "the smallest, because it's already bold, so it doesn't need to be too big, especially for an ERP".
- **Body text:** smaller.
- **Labels:** the lighter one, "and make it more standardised rather than having another thinner font".
- **Accent:** "this will vary, but let's default to blue". Medium strength: "not too contrasting and not too grey".
- **Greys:** "I like the cool one. The warm one is actually much more stylish, but for ERP the cool one is fine."
- **Page background:** "off-white, because it gives more contrast for all the different cards. Light grey is just too grey."
- **Theme:** "light mode, because our old clients like white, and dark mode mostly for myself."
- **Cards:** stand apart with a soft shadow, "the card way".
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
- **Emoji:** "none at all, ever." Later: "Emojis under comments are allowed… That's the only place we will allow emojis. Also in the rich text editors, we allow that as well." So comment reactions and the editor emoji picker stay; no emoji anywhere else. **Voice:** neutral, "this one depends".
- **Help text:** "I'd prefer never. If there's a validation error, show that, and if it's really needed you can show it, but I'd prefer never as much as possible. Make it as clear as possible."
- **Press:** "shrinking a little bit, but make sure nothing else in the UI moves."
- **Page change:** "I like the sliding a lot, but only for certain things, when we actually change the page."
- **Lists:** "one after another, but fast enough that they don't have to wait too long."
- **Numbers:** "counting up. But we may not have real time for all of these, so be careful."
- **Skeletons:** "I like the pulse. But a rule: skeleton loaders have to be exactly the same size as the UI that will come out, because we should know what the UI looks like. Before, during and after, it must fit the exact shape of every div."
- **Phone tables:** "very difficult. Avoid as much as possible, but it depends on the usage. If there are a lot of rows, they want to see things. Usually maybe just do summaries. I'd prefer compact rows instead of cards, because cards need way too much scrolling."
- **Header:** "depends on the app, but for [one sales ERP] I like C the best" [the shop picker as the header].
- **Choosing a shop and phone screens in general:** "more nested. Have everything and the options more nested, because we have to really concentrate on what's on the screen at a time."

## Test build: a landing page (following the skill)
"This one, the landing page, is extremely tasteless. With all the UI design skills and everything, it's meant for an ERP system, not for building a nice landing page that is interesting. I will not even critique this, because it is a terrible landing page: it has no taste."
"The UI is good, as in it has less clutter, but it needs some flair, like every landing page does. For example my personal website has extra graphics, a running theme and a storyline. This is okay UI-wise, but in terms of taste it is not good."

## Test build: a dummy ERP (following the skill; screens E1–E37 in `references/erp-test/`)
"Other than that it looks good." The points:
1. Two-line error messages like in E31 look weird, because the "!" icon is centred vertically.
2. E35: toggles are squares inside pills? Looks off.
3. E37: the profile pop-up is white and looks off next to the black sidebar.
4. E11: I don't like full pages for items. I like panes or pop-ups. Same for New product.
5. E6: the name in the top left. I don't like the icon.
6. E35: the toast isn't at the far right? And why is the Save changes button at the top right? If it fits on one page, the rule is to put it at the bottom. For scrollable pages, make sure saving before exiting is obvious.
7. Dropdowns: are they all custom? Make this a rule, and make sure it's a reusable component too.
8. E28: the skeletons for Transactions, Average basket, Cancelled and To ship are not the same size?

## Test: a job-queue dashboard tidy-up (following the skill)
"I don't like the new side by side. I like the old one. I wanted it to remove a lot of the text, that's all, but it kind of failed. Remove this, and just make a change to remove a lot of random text."

After the first text cut (17 strings), it was still too much text. What was left included "Last decision: memory pressure/OOM; retry", "8.4 GB free to admit of 14 GB" and "RAM 10.4 available, 2 reserve | pressure normal | heartbeat 32s ago". [Lesson: "less text" means much less. Raw system strings, repeated facts and debug stats come out of view and move into hovers. Each fact appears once, in plain short words.]

## Later additions
- **Corners:** "continuous curves on border radiuses, no abrupt changes" [squircle corners everywhere].
- **Submenus:** a safe triangle for menus (Smashing Magazine, "Better Context Menus With Safe Triangles").

## Sales ERP, first live review (screens J1–J8)
- J1 (Merchandising): "header issue when scrolling." The sticky table header overlaps the rows.
- J2 (order pane): "bottom right in pane, the products section ui needs work." The Products block is a grey box, and quantity and price run together.
- "main sales page loses a lot of columns as well, for checking the differences etc." [The redesign cut the default columns to six. The money columns are used to check differences, so they must stay visible by default.]
- J3 (Merchandising): "any part with product needs to have picture pls. including merchandising page."
- J4 (Cancellations): "clicking on cancellation reasons by reason section dont do anything?" [Every visible summary row should filter its list.]
- "reports page takes so long to load."
- "search bars are not the same throughout. filter button hover not there, custom dropdowns need to be standardized, make sure loading is sub 0.5s as usual"
- J5 (Discount detail): "how come there is order details dropdown as a table?" [A table hidden inside a boxed disclosure is wrong; show the table as a section.]
- J6: "ugly border when focusing on search bars." [A double ring and a dark outline on focus.]
- J7 (Products): "make tables full height in screen, and make rows less tall here."
- J8 (sidebar): "no icons on side bar?" [The Sales sub-items have no icons.]
- On process: "logic from previous version should not have changed, only UI should have changed." "do less tests, only isolated tests if changing logic." "be critical."

## Sales ERP, second live review (screens K1–K3)
- K1/K3 (Sales): remove captions such as "Display & references", "Fee split per product (i)" and "May be out of date · <date> Details". The ops banner for stopped syncs stays.
- K2 (sidebar): no "Sales" parent with sub-items. Its children are normal top-level items, same level and style as the rest. Keep icons.
- Orders vs Products: "their table headers are styled differently; pick one style and use it everywhere." The title area changes between pages; the page header must be identical in structure, size and position on every page.
- Merchandising: remove text slop. The favourites page is cluttered: keep the few functions that matter (list favourites, add/remove, the quantities it exists for); remove secondary controls and explanations. Merchandising tables use the same table UI as every other page.
- Cancellations: remove "Cancelled orders · by order date" and similar captions.
- Every page with a table gets one standard, reusable structure: header (title, then toolbar: search, source, filter), the table (same header style, row height, sticky header, number alignment, pictures, empty values) and a bottom bar with pagination and the row count. "No captions, no explanatory lines, no 'as of' lines; text only what's needed." Build it as shared components.
- Again: "logic from previous version should not have changed, only UI."
[Lesson: a caption under a title, an "as of" line and a references disclosure are all slop. One page skeleton everywhere: title, toolbar, table, bottom bar. Missing money stays "—".]

## Internal ops app
- "focus or highlight when clicking it it highlights in blue, can you disable repo wide focus blue highlights. i hate that so much"
- Grey states: search field dark at rest, light on hover/focus; list row light on hover, dark when selected, "so that the colors match when I'm not hovering over anything".
- Hover: row background and its children must change at the same instant; no staggered inner boxes.
- "height of logo must be same as the title + caption" (36 px was too big; measure the real line boxes).
- Popovers/previews: darker background than the page.
- Charts: run end to end; drop 0–100% side labels; legend in a row above.
[Lesson: no blue focus anywhere; keyboard-only neutral cue. Measure alignment, don't eyeball it.]
- Follow-up: a white/grey focus ring is also wrong: "remove focus rings entirely. just make the color whiter when clicked". Focus and click show only as a lighter fill (same token as hover); no ring, outline or border colour change, keyboard included.

## Sales ERP, empty page on a short phone
- "this needs a lot of ui work. too much random functions and stuff for nothing showing up. be more clear, just say nothing is there yet."
[Lesson: when a page or section has no data, show one plain line ("Nothing here yet") and hide what can't act on nothing: search, filters, source pickers, helper sentences, empty table headers, "no match" text, pager and row counts. Controls come back when there is data.]

## Sales ERP, report simplification (shots A–J)
- The ask: "reports page need simplification. tables too big and no pagination".
- Shown: charts and the transaction summary on top; every detail table behind one segmented switch (a dropdown on phones), one table at a time, 50 rows per page with the standard bottom bar; the page went from 21,957 px to 2,378 px tall at 1440.
- Approved: ship the layout; drop a per-day table whose counts are in the per-period table; the finance breakdown stays the first tab.
[Lesson: for a long report page, one table at a time behind a segmented switch is acceptable; duplicate tables can go when their numbers stay reachable elsewhere.]

## Sales ERP, third live review (points 1–8)
Numbered as given:
1. (Orders table: the horizontal scrollbar under the table is thick and dark, the vertical one thin and light) "horizontal vs vertical scrollbars need to be same. make it like the vertical one. for the entire app, all round reuse the component styles."
2. (Orders: Filter and Columns popovers open on top of each other) "if i click filter then columns, it will overlap. always one or the other"
3. (Orders: the week chip "Last week ×" then bare ‹ ›) "orders pages, these buttons need more context for prev and next week. make sure the ui is clean though"
4. "what happened to our N/A values? all gone? hidden?"
5. "in sales page no differences column anymore? that was a main function. color if there is difference, green or red."
6. (Settings page) "settings page ui needs another ui pass, its weird and not according to style" (a dialog with a heavy ring on the focused input) "and settings here i dont like border when focused. remove borders when focused."
7. (Orders: clicking some cells opens an explainer modal) "I don't want this modal to show when I click on certain cells. I want the whole row click to show the pane. that means you have to fix certain columns. For example the status column needs to be a bit wider because some of the statuses get truncated"
8. (Order pane, "Order-level fees") "order-level fees here should be clear about which ones are paid by the consumer, by [the marketplace] or the platform, or by [the seller] itself. You should label them. Put an icon, perhaps on the left side, and then for whether it's negative or positive, use green and red to color-code it here."
[Lessons: one scrollbar style for the whole app, never restyled per element. Two popovers from one toolbar never stack: opening one closes the other. Icon-only steppers need to say what they step to. Missing values stay visible ("N/A" or "—"), never silently dropped. The money-check columns (differences) are a main function: visible by default, coloured green/red only when there is a difference. Whole-row click opens the pane; no per-cell modals; size columns so values don't truncate. Fees say who pays (icon + short label on the left) and are coloured by direction. Focused fields show a background tint, no ring or darker border (same as the internal ops app rule). Settings follows this style: titled groups of rows on soft cards, no lines, no "i" tips, no disclosure hiding a facts table.]
- Later, on the order pane fees: "for the logos, you need to use [the marketplace] logo and [the seller's] logo, not just icons pls. and for totals no need icon, just bold them. for shipping use an icon is fine"

## Leads app, second UI pass
Lightly cleaned of dictation:
- Today: "the top bar is okay, but there are way too many. There's lots of text everywhere there."
- Today lead cards: "when I click on them, the new leads will have a background and a left border, which needs work. For every single one of the cards that open, there is way too much text everywhere."
- Lead card actions: "Tagging has a lot of buttons split here before the outcome, whether or not to fit: DM, Send, Add notes, etc., AI analysis, History. All of this needs to be according to my UI skill … We should not reduce features, but we should just group them properly and make the UX better."
- Content: "that also needs work, especially the top part. There is a title, caption, filter, the 'Why we post' part, more numbers before we actually see posting times, automation. After that we actually see the schedule."
- All leads: "we really need to clean this up as well. I'm not sure how to but you should put more items behind the click if possible. Also when I click it, it goes back to the Today page (the history page)."
- "Please make sure the UI elements, such as the filters, are consistent with all the reusable ones in [the app]."
- Scans and Settings: "do another UI pass … Padding issues, spacing issues: is this not as clean as something like my ops page?"
- "We also need proper skeleton loaders for everything."
[Lessons: keep every feature, but group actions (one primary action visible, the rest in a grouped menu or behind the open card); the main content (schedule, the lead list) comes first and explainers/stats move below or behind a click; a selected/open card is not marked with a tinted background plus a left border; filters reuse the app's shared components; the best-spaced page in the app is the spacing benchmark; every loading state gets a skeleton shaped like the content.]
- Shown as a compact review page. The answer: "yes merge".

## UI terms review
- "flag plus name of language i dont like full names of languages, i like "EN" and "CN" better, like the abbreviations. make that a rule too."
- Selected state shown as a quiet outline: "for 54 i dont like the borders."
- Status: "for pills in 53 i think its fine, colored pills sometimes is worth doing."
[Lessons: language picker = flag + short code (EN, ID, CN); a selected card gets a soft grey fill with no border; dot + text stays the default status, but a soft coloured pill is fine where a status needs attention.]

## Calendar and request thread (asked before the patch)
- Schedule view: "there's too much padding vertically."
- "Make sure that the entire calendar fits within my screen without having to scroll." The same for Week and Day.
- The no-deadline part with the dots "needs to be redone a little bit more."
- Filter panel on the left "needs proper restructuring. For example the search bar has to be on top."
- "Make it more simple as well please."
- Create, New Task, Trash, Today and the other controls "need proper styling, and also the height of the buttons." The day/week/month/schedule picker buttons "are not the same."
- Request thread: "the comment sent, all that UI has to be a little bit better."

## Calendar patch v1 review (C1–C18)
- "calendar patch ui still needs a lot of work. reorganize where things should be, use my erp-ui skill"
[Lesson: on a new page, tightening spacing and button heights isn't enough. When asked for a UI pass, look at where each control lives (page header, view switch, toolbar, filters, the unscheduled list) and propose a reorganized layout, not only a polish.]

## Calendar layout A vs B
- Picked A ("rest is fine"), with two fixes:
  - "search bar and today, november, day, week, month, schedule, are not aligned vertically"
  - "each item in the calendar must NOT use the heavy left border."
[Lessons: every control in a toolbar row shares one height and one centre line (search, buttons, title, segmented picker). Calendar or list items get no thick coloured left border; use a soft fill or a dot instead.]

## Client-setup screens, heavy clean (E1–E21)
- "i still want all details hidden. technical details specifically. make them easy to read as a non technical pls"
[Lesson: an ops screen for a non-technical reader (orders, client setup, usage) shows plain-language status and the one thing they must do. Technical details (hosts, stack names, step ids, logs, parameter paths, digests, record hashes) are hidden by default, behind a "Details" disclosure or gone. A heavy clean that only tidies spacing and copy is not enough when the content itself is technical.]

## Sales ERP, 16-item UI list ("Enforce all these rules.")
- Nav: the clicked tab must highlight at once (optimistic), not after the page loads.
- "Make sure the scrollbar is the same throughout the entire app. I like the scrollbar for the vertical scroll in the orders page. Make sure the horizontal scrollbar also follows the style. Let's keep this more subtle."
- "For columns ... like marketplace and status, don't make them two lines. Make them one line instead."
- "If they change the name of the column then just show the new name ... Don't show both."
- Shop dropdown: the marketplace logo beside each shop; "only [one marketplace] or only [the other], with one click."
- No border around filter chips (date filter, "filters applied"); export/import buttons: no stray border, same font weight.
- Logistics: split bought vs sold sections with faint colours, "make it look nice". Compare: "a little bit of color to show which one is the best."
- Activity: plain language, "not that technical"; padding between toolbar and table.
- First load of orders/products/reports "under 0.5 seconds", benchmarked.
[Lessons: one scrollbar style app-wide (subtle, horizontal too); table cells stay on one line; a renamed column shows only the new name; filter controls carry no box border; buttons in one row share one weight and one style; a muted colour hint is welcome where it helps compare (best value, bought vs sold).]

## Sales ERP, filter loading
- "when changing filters, pls use skeleton loads as well, this is a rule for all pages. enforce this."
[Lesson: a filter change (shop, date, status, search, tab, sort) swaps the affected content for its skeleton until new data arrives; never leave stale rows or charts showing, never a spinner.]

## Sales ERP, editable logistics table
- Header "Total" lacks right padding; "each cell is editable immediately"; a cell turns dark grey on click; row selection doesn't follow the click; typing changes the height; a new pre-order should not take two clicks; edits "tracked as a change in the history logs".
[Lessons: editable tables behave like a spreadsheet: one click edits, the selected row follows the click, view and edit states have identical size, focus is a soft fill not a dark block; header and cell insets match; every inline edit is audited.]

## Alora Design v1 review (design.alorawork.com; letters L/G/E/S/X)
Lightly cleaned of dictation:
- "I want it to be dark mode by default, and make the dark mode properly dark instead of this blue-tinted dark." [For the Alora Design site and library defaults. ERP products for older clients may still start light; don't flatten.]
- (L1 hero) "The preview in the right header section doesn't need another area around it." Then: "My hero section, I want it to be a bit different. I want it to be more plain. Let's not have a demo in that part. The demo we should move to the bottom."
- "Let's use neutral by default instead of cool." "Let's use pink by default." [Accent default for this library.]
- "Padding and everything can change myself, but it doesn't look that good, especially since we have spacing issues."
- (Metric cards Orders, Cancelled) "I don't like how the numbers look in that. I want to make a new creative UI element that shows short numbers and long numbers a little bit differently, so it's a little bit nicer to view. Right now, canceled with only one number looks really bad."
- (Low stock) "not enough padding on the right."
- "All, unpaid, to pack, shipped, needs review, paid, or canceled, the bubbles have different padding, and that needs work."
- "The selector, like today for dates, is too long."
- "It's not centered vertically for the two shops that haven't synced. The payout field is also not centered properly."
- "We need more UI elements." "I really want to put a lot of spotlight on a lot of niche UI elements."
- "Let's just show the gallery right away here on the main page."
- (Examples) "It says team, products, and promotions are not part of the example. Please fix that."
- "The navbar changes position when I go to examples versus when I go to export and gallery." "We need a better header section."
[Lessons: dark means neutral near-black, no blue tint. Every pill, chip and segment shares one padding scale. A one-digit number must not sit lost in a card: short and long numbers need their own treatment. Date/select triggers size to their value. Single-line alerts centre icon, text and button on one line. The site header is identical in position and size on every page. Every nav item in an example opens a real page. A landing hero can be plain; live demos go lower.]

## Alora Design v2 review (landing)
- (S25/S24, the labelled component tiles on the landing) "I want all the components to not be in their own grid. I want all of them to just be right there on the page natively and do this for everything. Try and make a nice bento style with all of these. That's how we should show it."
- (Bottom "Corners that agree" demo) "please just remove this part. We'll do this later."
[Lesson: a showcase shows components in use, composed into a bento of real-looking cards, not a catalogue of labelled boxes, one per component.]

## Alora Design v3 review (landing bento, B1–B19)
- "[The shop settings card] needs better padding/spacing. [The team card] too. [The product photos card] too." [B10 shop settings, B12 team, B18 photos and tags: ragged right-hand controls of different widths, crowded avatar group, cramped rows, a dropzone with too much empty space.]
- Hero title: "make it simpler. just use 'just some random ui styling'". [The exact words were picked; casual and modest beats a bold claim for this site.]

## Alora Design v3.1 review (landing hero, sales card, customize panel)
- "make the hero section really big. overly big text"
- (Bento "Sales today" card) "this part too different?" [Read as: make it big and distinctive too, not a plain stat.]
- "i want customize thing to be interesting. i want a small customize flap on the left of the screen, only opens on hover, this will open a nice customize section on the left of the screen. moving all ui elements to the right, so that there is no right spacing. and the leftover space taken over by this ui element."
[Lessons: on a showcase landing, the headline can be oversized; scale is the flair. Settings panels can be a hidden edge tab that opens on hover and pushes the page aside rather than floating over it, with the panel filling the freed space.]

## Alora Design v3.2 review (customize flap, header)
- "make sure scrolling on the left and right are different" [The open customize panel and the page each scroll on their own; wheel over one never moves the other.]
- "for title, use alora logo not just alora design normal text"
[Lessons: a side panel next to a page is its own scroll area, never chaining into the page. A brand's site header uses the real logo, not the name typed in the UI font.]
- "make sure it works mobile too responsive"
[Lesson: every change is checked at phone and tablet widths before it ships; no horizontal scroll, nothing wraps or crowds.]

## Alora Design v4 direction
- "i also want a section on ai stuff, for example later a collection on spinners or loaders for ai"
- "i also want [an AI assistant background], to be like interactive agent ui options for example, or just interactive backgrounds, but those i will add and curate as we go on"
- "make sure our page starts with components, but also have tabs in nav bar for other things. and on the main page show all of these. the full gallery, pls dont make it like cards, make it like the mainpage where its just real components on screen"
[Lesson: a gallery index is the components themselves laid out live, never a grid of preview cards.]

## Alora Design v4 review (AI section)
- "ai part swap right and left, and make it larger taller make sure the input box also good, right now its not balanced centered, padding etc" [Chat list goes left, thread right, like a real app; the composer's placeholder, icons and send button sat off-centre with uneven padding.]
[Lesson: a chat composer has equal insets on all sides, its placeholder and buttons share one centre line, and the attach/send buttons sit on the same baseline row with matching corner offsets.]
- (Composer with buttons on a row under the text) "no make it like [the internal app's] assistant where the text is in middle between attach files and send button"
[Lesson: the AI composer is one row: attach | text | send, one control size so a single text line and both buttons share a centre; multi-line text grows upward while the buttons stay at the bottom.]
