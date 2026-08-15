# Quiz — Module 06: Visual Design

13 questions. Target: 10/13.

---

### Part A — Recall

**1.** The strongest single tool for visual hierarchy is:
- a) colour
- b) size
- c) style treatment
- d) position

**2.** The recommended measure (line length) for body text is roughly:
- a) 20–35 characters
- b) 45–75 characters
- c) 90–110 characters
- d) as wide as the container

**3.** WCAG AA contrast for normal body text is:
- a) 3:1
- b) 4.5:1
- c) 7:1
- d) 2:1

**4.** In dark mode, elevation is usually expressed by:
- a) larger shadows
- b) lighter surface colour
- c) thicker borders
- d) increased saturation

**5.** A 12-column grid is common because:
- a) it matches most screen widths
- b) it divides evenly by 2, 3, 4, and 6
- c) it is the browser default
- d) it maps to an 8-point scale

---

### Part B — Short answer

**6.** Why does adding emphasis to more elements reduce total emphasis? Name the effect.

**7.** Give a practical six-step UI type scale, and say what happens if two steps are only 2 px apart.

**8.** Explain why role-based colour tokens beat value-based ones.

**9.** State the "unbreakable rule" of colour and give three populations or contexts it protects.

**10.** Give the three responsive strategies and name the one that most often causes harm.

---

### Part C — Applied

**11.** A dashboard has eight equally styled metric tiles and users say it is "hard to read." Give a full fix covering hierarchy, grouping, and verification — and name the risk.

**12.** A team ships light-grey 13 px body text at 1.2 line height across the full container width. List every problem and the fix, ordered by impact.

**13.** You are asked to bring a desktop data table to mobile. Walk through your decision process and give three different answers depending on the user's task.

---
---

## Solutions

**1. b)** Size — the bluntest and strongest. Note the caveat: emphasis is relative, so size only works against smaller neighbours.

**2. b)** 45–75 characters, ~66 as a classic target. Beyond that, the return sweep causes line-tracking errors.

**3. b)** 4.5:1 for normal text; 3:1 for large text (≥18.66 px bold or ≥24 px) and for UI components/graphical objects; 7:1 is AAA.

**4. b)** Lighter surfaces read as higher in dark mode, because shadows are largely invisible against dark backgrounds.

**5. b)** Divisibility by 2, 3, 4, and 6 — it supports halves, thirds, quarters, and sixths without fractional columns.

---

**6.** Emphasis is **relational**: an element stands out only by differing from its neighbours on some attribute. When many elements share the emphasised treatment, the target no longer differs from the distractors, the pre-attentive pop-out collapses, and visual search becomes serial. The named effect is the **Von Restorff (isolation) effect**, which requires a uniform background set to function.

**7.** For example: 12 caption / 14 secondary / 16 body / 20 section heading / 24 page heading / 32 display — roughly a 1.2–1.25 ratio. If two steps sit 2 px apart, the difference falls below the threshold at which users perceive a deliberate level, so it reads as an inconsistency or a mistake rather than a hierarchy. Fewer steps with clear jumps is always better.

**8.** Role tokens (`text-primary`, `surface-raised`, `border-subtle`) describe *what the colour is for*; value tokens (`grey-700`) describe what it is. Consequences: a theme change (dark mode, high contrast, white-label brand) only requires remapping roles to values, rather than editing every component; the semantics survive redesigns; and reviewers can catch misuse ("why is `danger` used for a neutral border?"), which value tokens hide. Value tokens still exist — roles point at them — but components should consume roles.

**9.** Rule: **never encode meaning with colour alone**; always pair it with an icon, label, shape, pattern, or position. It protects users with colour-vision deficiency (~8% of men, ~0.5% of women), users on poor or greyscale displays, users in bright sunlight or with screen filters/night modes, and any printed or photocopied output. It also aids everyone, because redundant encoding is faster to interpret.

**10.** **Reflow** (same content rearranged), **reveal/hide** (different content per viewport), **restructure** (genuinely different layout or interaction per platform). Reveal/hide causes the most harm, because hiding content on small screens assumes mobile users want less — usually false, since they often want exactly the same thing in worse conditions. Hide chrome, not content.

**11.** Fix:
- **Rank in words first** — decide which one or two metrics answer the user's primary question ("is anything wrong?" or "how are we doing this week?").
- **Hierarchy:** make the top metric dominant using at least two tools together — larger figure, higher contrast, more surrounding space — and demote the rest to a uniform secondary treatment. Demoting the seven is more effective than enlarging the one.
- **Grouping:** cluster related metrics with proximity or a shared region so the screen reads as two or three clusters instead of eight peers (Gestalt).
- **Ordering:** put the most decision-relevant tiles first and last, exploiting serial position, and avoid burying anything critical in the middle.
- **Verification:** squint test or greyscale — the intended first stop should survive the blur, and nothing important should depend on hue.
- **Then measure:** time-to-answer for a specific question ("did conversion drop yesterday?") is the real test.
Risk: a fixed hierarchy imposes one reading on users who came with a different question. Mitigate by choosing the emphasis from actual usage data, and be cautious about "make it configurable" — configurable dashboards are rarely configured, so the default must be right for the majority.

**12.** Ordered by impact:
1. **Contrast.** Light grey on white likely fails 4.5:1 — an accessibility violation and the biggest readability cost, worst for older users and in bright light. Fix: near-black body text; measure the ratio rather than eyeballing.
2. **Measure.** Full-container width will exceed 75 characters on desktop, causing return-sweep errors. Fix: cap the text container around 65–75 characters.
3. **Line height.** 1.2 is too tight for body text, which compounds the long-measure problem. Fix: ~1.5, and more if the measure stays wide.
4. **Size.** 13 px is below comfortable for sustained reading; 16 px is the sensible default. Fix last only because contrast and measure usually dominate the perceived problem — though on mobile, size interacts with the OS text-size setting, so ensure the type scales with user preferences rather than being locked.
Also check: text must remain usable at 200% zoom, and must not be an image of text.

**13.** Decision process: **start from the task the table serves**, not from the layout. Ask what the user does with it — scan for one value, compare rows on a shared attribute, or select and act in bulk. Then check which columns are actually used (analytics or observation), and what the identifying column is.
Three answers:
- **Scanning for one item:** convert to a card/list view with the identifying field plus the one or two most-used values per row, progressive disclosure for the rest, and prominent search or filter. The table structure is irrelevant to this task, so it should not survive.
- **Comparing across rows:** keep a table, but make it horizontally scrollable with the identifying column frozen, right-aligned tabular figures, and a way to reduce columns (a column picker or a "compare these two" mode). Comparison is the one task where the tabular structure is the value, so preserve it.
- **Bulk operations:** list with multi-select, a persistent selection count, and a sticky action bar; ensure selection survives scrolling and accidental navigation, since losing a large selection is a severity-4 loss of user work.
Cross-cutting: never shrink type to make the desktop table fit; ensure touch targets stay ≥44 pt; and verify the header stays available (sticky) so column meaning is not a memory task.

---

<!-- nav -->
[← Previous: 6.4 Layout & Grids](6.4-layout-and-grids.md) · [↑ Module 06 — Visual Design](README.md) · [Next: Module 07 — Interaction Design →](../07-interaction-design/README.md)
