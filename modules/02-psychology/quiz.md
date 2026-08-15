# Quiz — Module 02: Psychology & Cognition

12 questions. Target: 9/12.

---

### Part A — Recall

**1.** The Gulf of Evaluation is the gap between:
- a) what the user wants to do and how to express it
- b) the system's state and the user's ability to perceive and interpret it
- c) the designer's model and the system model
- d) intrinsic and extraneous load

**2.** Which type of cognitive load should a designer attack first?
- a) intrinsic
- b) extraneous
- c) germane
- d) all equally

**3.** Which of these is NOT a pre-attentive attribute?
- a) hue
- b) size
- c) semantic meaning of a word
- d) motion

**4.** A realistic modern estimate of working-memory capacity for unrelated items is about:
- a) 2 chunks
- b) 4 chunks
- c) 7 chunks
- d) 12 chunks

**5.** "People take the first option that seems good enough" describes:
- a) anchoring
- b) satisficing
- c) the decoy effect
- d) loss aversion

---

### Part B — Short answer

**6.** Name the three models present in any product and say which one the designer controls directly.

**7.** Give three concrete sources of extraneous cognitive load, each with a one-line fix.

**8.** Why does a page with four filled "primary" buttons have no primary button? Answer using perception, not taste.

**9.** State a one-sentence test that separates ethical persuasion from a dark pattern.

---

### Part C — Applied

**10.** Users delete an item at the bottom of a long list, see nothing happen, and delete again. Diagnose using perception concepts and give two fixes at different costs.

**11.** A settings screen has 40 toggles and users cannot find anything. Give your fix sequence in priority order and name what each step costs.

**12.** Your team wants to add an animated banner to promote a new feature on a screen where users perform a focused daily task. Argue for or against, using at least three concepts from this module.

---
---

## Answers

**1. b)** Evaluation is about perceiving and interpreting system state. Option (a) is the Gulf of Execution.

**2. b)** Extraneous — it is load created by presentation, which is precisely what the designer controls. Intrinsic can only be sequenced; germane is useful and should be protected.

**3. c)** Semantic meaning requires conscious processing. Pre-attentive attributes are form, colour, position, and motion.

**4. b)** ~4 chunks. Miller's "7±2" came from a 1956 paper on absolute judgement and is routinely over-applied; chunking raises effective capacity because a chunk is a *meaningful* unit, and expertise creates bigger chunks.

**5. b)** Satisficing (Herbert Simon).

**6.** System model (how it actually works), conceptual model (the story the design tells), user's mental model (what the user believes). The designer directly controls the **conceptual model** — the other two are, respectively, engineering reality and a consequence.

**7.** Any three, e.g.:
- Unnecessary choices → provide a sensible, editable default.
- Inconsistent components → unify via a design system.
- Ambiguous or internal jargon labels → rename to the user's words, validated by a first-click test.
- Split attention (help far from the field) → move guidance inline.
- Memory carries across screens → display the value instead of requiring recall.

**8.** The pop-out effect depends on the target differing from all distractors on a pre-attentive attribute. When four elements share "filled + saturated," none differs, so visual search becomes serial and the eye must read each to decide. Emphasis is relative, not absolute.

**9.** Model answers: "Does this technique help the user reach a goal they hold themselves, and is the reverse action as easy as the forward one?" or "Would I be comfortable showing the user exactly why this works?"

**10.** Diagnosis: **change blindness** — the change (a toast at the top of the viewport) occurred outside the user's locus of attention, which was at the bottom of the list where they clicked. Possibly compounded by **banner blindness** if the toast sits in a region resembling promotional content.
- Cheap fix: move feedback to the point of action — inline row animation (row collapses), or an undo bar anchored near the interaction.
- Higher-cost fix: optimistic removal with an inline "Deleted — Undo" replacing the row itself for a few seconds, plus a persistent count of items so the change is visible in a second place (redundant encoding).

**11.** Priority order with costs:
1. **Group into meaningful sections with plain-language headers** — cost: near zero; risk of the wrong taxonomy, so validate with a card sort.
2. **Surface the most-changed settings at the top** — cost: requires usage data; risks feeling arbitrary if the data is thin.
3. **Add search** — cost: engineering effort; strongest single fix for large settings surfaces because it converts navigation into recall-free retrieval.
4. **Progressive disclosure — "Advanced" section** — cost: extra clicks for power users; only bury options with verified low usage.
5. **Remove settings entirely** by choosing a good default — cost: lost capability and a support burden from the minority who needed it. Last resort, and reversible.

**12.** Model answer (against, with conditions):
- **Inattentional blindness**: users in a focused daily task systematically miss peripheral content, so the banner will likely be unread by the people we most want to reach.
- **Banner blindness**: a wide colourful rectangle is the exact shape users have learned to ignore.
- **Motion is the strongest pre-attentive attribute**, so if it *is* noticed it will interrupt a focused task — capturing attention involuntarily and adding extraneous load to the task the user came for. It also needs a `prefers-reduced-motion` fallback.
Better alternative: place the promotion **in the path** of the task (contextual entry point at the moment the feature is relevant), or use a one-time, dismissible, non-animated inline cue and measure engagement. Acceptable use of motion: rare, urgent, user-relevant events.
Full credit requires naming the trade-off — a contextual cue reaches fewer users per session but converts far better, and does not degrade the primary task.
