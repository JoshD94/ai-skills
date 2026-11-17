# Design principles (the 93 kept)

These 91 were chosen from 100 candidates, then UI-15 and UX-51 were added (93 in all). The illustrated picker page is at
`references/ui-ux-principles.html`.
IDs match that page. Cite a principle's ID in an audit or critique when it explains a problem.

How to use them:
- **Editing an existing tool (default):** they are a lens for finding and explaining problems. They never license a restyle.
  Where a principle is a style choice (UI-16, UI-17, UI-24, UI-25, UI-44), the product's existing choice wins.
  The defect is breaking that choice inconsistently. A principle the product doesn't follow becomes a suggestion for the reviewer.
- **Redesign (only when asked for one):** they are the direction. Variants should follow them.
- Skipped on purpose, so don't add them back: closure, line height 1.4–1.6, squint test,
  golden ratio, F-pattern, Zeigarnik, endowed progress and the Fogg model.

## UI: how it looks

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
- **UI-15 Continuous corners (squircle).** Added back on request. Corners curve continuously into the straight edges, with no kink. See taste.md for how to build them.
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

## UX: how it works

- **UX-1 Fitts's law** (Fitts, 1954). Make important targets big and near. Tap targets are at least 44 pt (Apple) or 48 dp (Android).
- **UX-2 Hick's law** (Hick, Hyman). Each extra choice slows the decision. Show a few and put the rest behind "More".
- **UX-3 Chunking** (Miller: "The magical number seven, plus or minus two"). Group long numbers and codes, for example 1234 5678 9012 3456.
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
