# Quiz — Module 10: Accessibility

12 questions. Target: 9/12.

---

### Part A — Recall

**1.** POUR stands for:
- a) Perceivable, Operable, Understandable, Robust
- b) Practical, Open, Usable, Reliable
- c) Perceivable, Optimised, Usable, Responsive
- d) Predictable, Operable, Understandable, Readable

**2.** The practical conformance target for most products is:
- a) WCAG 2.2 Level A
- b) WCAG 2.1/2.2 Level AA
- c) WCAG 2.0 Level AAA
- d) WCAG 3.0

**3.** Minimum contrast for normal body text at AA:
- a) 3:1
- b) 4.5:1
- c) 7:1
- d) 2.5:1

**4.** WCAG 2.2's Target Size (Minimum) criterion requires:
- a) 44×44 CSS px
- b) 24×24 CSS px
- c) 48×48 dp
- d) no minimum

**5.** Automated accessibility tools detect approximately:
- a) nearly all issues
- b) a minority — commonly cited around a third
- c) only contrast issues
- d) only markup errors

**6.** The first rule of ARIA is:
- a) always add ARIA roles to custom components
- b) do not use ARIA if native HTML will do
- c) use `aria-label` on every element
- d) ARIA replaces semantic HTML

---

### Part B — Short answer

**7.** Explain the social model of disability and why it is the useful framing for designers.

**8.** Give the permanent / temporary / situational framing with an example for one need category.

**9.** List five things a designer must specify in handoff for a component to be built accessibly.

**10.** Name five accessibility failures ranked by damage, and say why the top one is worst.

---

### Part C — Applied

**11.** Review this pattern: a data table where rows are deleted by swiping left, status is shown as a coloured dot, the delete confirmation is a modal, and results update live as filters change. List the accessibility problems and the fixes.

**12.** Your team has one week left before launch and accessibility has not been considered. What do you do, in order, and what do you explicitly defer?

---
---

## Solutions

**1. a)** Perceivable, Operable, Understandable, Robust.

**2. b)** AA of WCAG 2.1 or 2.2 — the level referenced by most regulation and procurement. AAA is applied selectively, not wholesale; 3.0 is a draft.

**3. b)** 4.5:1 (3:1 for large text, defined as ≥18.66 px bold or ≥24 px, and 3:1 for UI components and meaningful graphics).

**4. b)** 24×24 CSS px at AA (with exceptions for sufficient spacing, inline text, and user-agent defaults). 44×44 is the platform guidance and the AAA-level figure — a better practical target for touch.

**5. b)** A minority; roughly a third is the commonly cited figure. They cannot judge whether alt text is meaningful, whether focus order makes sense, whether a label describes the right thing, or whether the flow is actually completable.

**6. b)** Do not use ARIA if a native element will do; incorrect ARIA is worse than none because it lies to assistive technology.

---

**7.** The social model holds that disability arises from **barriers in the environment** rather than from an attribute of the person — a person is disabled *by* a design that assumes a mouse, not by their motor condition. It is useful for designers because it makes the design the variable: instead of "we cannot support that user," the finding becomes "our design creates this barrier, and removing it is our job." It also connects directly to the mismatch framing used in inclusive design, where the fix is always on the environment side.

**8.** Example for motor/dexterity: **permanent** — a person with one arm; **temporary** — a broken arm or a recent injury; **situational** — someone holding a baby, carrying shopping, or on a moving train. All three benefit from one-handed operability, large targets, and no precise dragging. The framing matters because it shows the design change serves a far larger population than the disability statistic alone suggests, which is the most effective argument with sceptical stakeholders.

**9.** Any five: the **semantic element** (button vs link vs heading — links navigate, buttons act); the **accessible name**, which must contain the visible label text (WCAG 2.5.3); **role and states** (expanded, selected, checked, invalid, busy); **focus behaviour** — tab order, whether focus is trapped, and where focus goes after the action; **announcements** for asynchronous changes (live region text such as "3 results found"); **alt text** for each image or an explicit decorative marking; **keyboard equivalents** for any hover- or gesture-only interaction; **error association** between message and field.

**10.** Ranked:
1. **Keyboard traps and missing focus indicators** — worst, because they block entire populations from completing anything at all; a trap means the user cannot even leave the component, and no workaround exists on their side.
2. **Custom controls with no name/role/state** — a screen reader announces "clickable" with no meaning, making the control unusable.
3. **Colour-only encoding of status or errors** — invisible to a large population and in many contexts.
4. **Placeholder-as-label** — the label vanishes when needed, contrast usually fails, and programmatic association is lost.
5. **Insufficient contrast** — especially grey-on-white body text and disabled states; degrades everyone's experience and is trivially preventable.
The top one is worst because it is a total blocker rather than a degradation, and because it is invisible to sighted mouse-using teams, so it ships routinely.

**11.** Problems and fixes:
- **Swipe-to-delete as the only method** — violates keyboard operability (2.1.1) and WCAG 2.2's dragging-movements criterion (2.5.7); invisible to screen-reader and switch users, and has no signifier for anyone. **Fix:** provide a visible delete action per row (button or overflow menu) reachable by keyboard, with the swipe kept only as an accelerator.
- **Coloured dot for status** — violates 1.4.1 Use of Color; also likely fails 1.4.11 non-text contrast if the dot is the only indicator. **Fix:** pair the dot with a text label, and ensure the text is the accessible name; if space is tight, use shape plus text rather than hue alone.
- **Delete confirmation modal** — needs explicit focus management: focus moves into the dialog on open, is trapped while open, returns to the triggering row's control on close (or to a sensible neighbour if that row is gone), and Escape closes it. Without this it is a keyboard trap or a focus-loss bug. Also give it a proper dialog role and an accessible name, and make the confirmation text specific ("Delete invoice 4021?") rather than "Are you sure?".
- **Live-updating results on filter change** — violates 4.1.3 Status Messages if nothing is announced, and can violate 3.2.2 On Input if the context change is unexpected. **Fix:** announce the result count via a polite live region ("18 results"), keep focus where the user put it, and avoid moving focus to the results automatically. Ensure the filter controls have visible labels and that active filters are shown as removable, keyboard-reachable chips.
- **Table semantics generally** — ensure real table markup with header cells associated to data cells (1.3.1), a caption or accessible name, and that row actions are reachable in a sensible focus order.
- **Target sizes** for row actions — at least 24×24 CSS px, preferably 44×44 pt on touch, with adequate spacing so delete is not adjacent to a common action (anti-Fitts for destructive actions).

**12.** In order, prioritising blockers over degradations:
1. **Run a keyboard-only pass on the primary flows** (30 minutes). Find traps, unreachable controls, and missing focus indicators. These are total blockers and often cheap to fix.
2. **Run automated tooling** (axe/Lighthouse) across key pages — catches contrast failures, missing labels, missing alt, and invalid roles quickly. Treat the output as a floor, not a verdict.
3. **Fix, in this order:** keyboard traps → missing/invisible focus indicators → controls with no accessible name → form labels and error association → contrast failures → colour-only encoding → images missing alt.
4. **Screen-reader spot check** on the two highest-value flows (sign-up and the core task) with VoiceOver or NVDA — even 45 minutes finds the worst announcement gaps.
5. **Check zoom/reflow at 200%** on the same flows.
6. **Write down every known gap** with severity in a public list, with owners and target dates. An honest, tracked backlog is defensible; a silent one is not.
Explicitly deferred (and scheduled, not dropped): a full component-library audit; usability testing with assistive-technology users; complex custom widgets that need rebuilding rather than patching; a formal conformance report or VPAT; and any criterion requiring content rework across the whole product, such as rewriting long-form copy for plain language.
What I would not defer: anything that blocks a population entirely — keyboard traps, unreachable primary actions, and unlabelled critical controls. I would rather delay a non-essential feature than launch with a flow that a keyboard user cannot complete, and I would say that plainly, with the legal exposure noted once rather than repeatedly.

---

<!-- nav -->
[← Previous: 10.3 Designing Accessibly](10.3-designing-accessibly.md) · [↑ Module 10 — Accessibility](README.md) · [Next: Module 11 — Design Systems →](../11-design-systems/README.md)
