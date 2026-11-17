---
name: erp-ui
description: "Run whenever the user says \"erp ui\" (alone or in a sentence, any case), or asks to build, redesign, edit, tidy or critique an ERP, admin, dashboard or app UI with this taste. Holds one product owner's UI taste (taste.md, and their words in feedback.md, which win), 93 chosen UI/UX principles, and reference screenshots. Editing an existing tool changes only what was asked; redesign only when asked. Landing pages need a concept and flair first. One self-audit pass, then lettered screenshots for critique; feedback is written back into the skill."
---

# ERP UI

An opinionated taste for ERP, admin and app interfaces: calm, dense, rounded, no clutter.
It was written down from one product owner's picks and line-by-line critiques of real screens, so the rules are specific and tested, not generic best practice.
No score-driven hill climb: rubric scores went up while the reviewer liked the result less.

## Files
- `taste.md`: the rules. Never list, Always list, visual system, copy, motion, phone, components, landing-page and editing modes. **These win over everything else.**
- `feedback.md`: the critiques behind the rules, in the reviewer's own words, plus how they talk. Read it whenever a case isn't covered by `taste.md`.
- `principles.md`: 93 UI/UX principles kept from 100 candidates. Background only; `taste.md` wins.
- `templates/builder-brief.md`: a brief to hand a subagent that builds or edits the UI.
- `references/`:
  - `answers.md`: every picker answer (icons, type, colour, copy, motion, phone).
  - `ai-site-critique/` (A–J): two AI-made landing pages that were critiqued.
  - `erp-test/` (E1–E37, E22 left out) and `audit.md`: a dummy ERP built with this skill, and its self-audit.
  - `app-chrome/`: the app-chrome reference (settings screens of a desktop app).
  - `landing-page-reference/style.md`: the landing-page reference style.
  - `ui-ux-principles.html`: the illustrated principles picker.

## Pick the mode first
- **Edit an existing tool** (the default for anything that already exists):
  - Change only what was asked for, such as "remove the random text" or "fix the toggles".
  - Keep the layout, colours and structure.
  - Put any wider ideas in a short list; don't build them.
- **Redesign:** only when asked for a redesign or a new build. `taste.md` is the spec, and every Never item is a hard failure.
- **Landing page:**
  - Restraint alone looks tasteless here. First propose a concept, a running theme and a signature visual (see `references/landing-page-reference/`), and get an OK.
  - Then build with the restraint rules.

## Workflow
1. Read `taste.md` and `feedback.md` in full, the references that fit the job, and the repo's AGENTS.md or CLAUDE.md if there is one.
2. Work on a branch, or in an output folder for prototypes. Don't merge, release or deploy without the reviewer's OK.
3. Build it yourself, or hand `templates/builder-brief.md` to a subagent.
4. **Self-audit once:**
   - Screenshot every changed screen and state with a headless browser (for example Playwright), desktop 1440×900 and phone 390×844.
   - Check each screenshot against every Never and Always item, and fix what fails.
   - Write `audit.md`, at most 40 lines: pass or fail per Never item, plus every placeholder or invented fact.
5. **Show the reviewer** one review page or folder:
   - Lettered screenshots (E1, E2… or Q1…) so they can reply "for E6, …".
   - Before and after side by side when editing. Capture both within seconds of each other so the data matches.
6. **Write feedback back** the same day:
   - Their words go in `feedback.md`, under a dated heading, with the screen letters.
   - New or changed rules go in `taste.md`, with the screen letter as evidence.
   - Don't flatten an "it depends" into an absolute.
7. After their OK, ship through the repo's normal path. Stop preview servers and close browsers you opened.

## Rules that always apply
- No production or client data in screenshots.
- Logic doesn't change in a UI pass unless asked: "only UI should have changed."
- Write plainly and briefly, in a direct voice. See "How the reviewer talks" in `feedback.md`.
