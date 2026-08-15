# Quiz — Module 04: Gestalt

12 questions. Target: 9/12.

---

### Part A — Recall

**1.** Which principle overrides proximity?
- a) similarity
- b) common region
- c) closure
- d) symmetry

**2.** The strongest grouping cue of all is:
- a) proximity
- b) similarity
- c) uniform connectedness
- d) common fate

**3.** The Law of Prägnanz states that the eye:
- a) follows the smoothest path
- b) completes incomplete shapes
- c) resolves ambiguity toward the simplest interpretation
- d) separates figure from ground

**4.** Two items animating in the same direction are perceived as related because of:
- a) continuity
- b) common fate
- c) closure
- d) similarity

**5.** In a form, the label should be:
- a) equidistant between its field and the one above
- b) closer to the field above it
- c) closer to its own field than to any other element
- d) always inside the field as a placeholder

---

### Part B — Short answer

**6.** Explain why a peeking card at the edge of a horizontal list communicates scrollability better than pagination dots, naming the principle.

**7.** Give the rough ordering of grouping strength among uniform connectedness, common region, proximity, and similarity, and say why the ordering is useful.

**8.** Describe the squint test and name four ways to perform it.

**9.** What is the most common spacing bug in layouts, and what does it cause perceptually?

---

### Part C — Applied

**10.** A settings page uses cards around every group, borders inside each card, and dividers between rows. Users describe it as "heavy" and "hard to scan." Diagnose and prescribe.

**11.** A dashboard shows 8 metric tiles. Users say they cannot tell which metric matters. Give a Gestalt-based fix and name the risk of over-applying it.

**12.** You are handed a screen where the label of one form field appears to belong to the field above it, section headers look decorative, and the primary button does not stand out. Write the critique as you would deliver it in an interview, in order.

---
---

## Solutions

**1. b)** Common region — a shared boundary beats mere nearness, which is why a card drawn around the wrong elements defeats correct spacing.

**2. c)** Uniform connectedness — an explicit visual connection (a line, a shared container edge, a connector) is the strongest grouping cue.

**3. c)** Simplest available interpretation. (a) is continuity, (b) is closure, (d) is figure/ground.

**4. b)** Common fate.

**5. c)** Closer to its own field than to any other element. Note that placeholders as labels (option d) is a known anti-pattern: the label disappears on focus, which converts recognition into recall and breaks accessibility.

---

**6. Closure.** The mind completes the cut-off card, so a partially visible item is perceived as a whole object that continues beyond the viewport — which directly implies more content in that direction. Dots are an abstract, learned symbol that requires the user to notice and interpret them, and they do not indicate the *direction* of interaction. The peeking card also gives a larger implicit affordance and works without any legend.

**7.** Uniform connectedness → common region → proximity → similarity. It is useful because these cues routinely **conflict** in real layouts: when your card boundary groups A and B while your spacing groups B and C, the boundary wins and users perceive A+B. Knowing the order lets you predict which cue users will follow and fix the right one, rather than adding more cues on top.

**8.** The squint test is deliberately degrading your view of the design so you see only what pre-attentive perception delivers in the first ~200 ms — the groups, the hierarchy, and the figure/ground separation. Four ways: physically squint; apply a Gaussian blur to a screenshot; zoom out to ~25%; convert to greyscale (which also verifies you are not encoding meaning with colour alone).
Judging criteria: do the intended things group, is there a clear first stop for the eye, does the primary action survive, is figure distinguishable from ground.

**9.** Between-group spacing equal to or smaller than within-group spacing. Perceptually, proximity then fails to encode the intended structure, so the eye groups by whatever cue is left — typically by row or by shared background — and the section structure becomes invisible. Users experience this as "cluttered" or "the sections run together," and no amount of heavier headings fixes it, because proximity is a stronger cue than typographic weight for grouping.

**10.** Diagnosis: **too many boundaries competing**. Cards (common region), internal borders, and dividers are three simultaneous grouping mechanisms applied to nested levels, so every level looks equally strong and the hierarchy flattens. Each boundary also adds visual weight, producing "heavy." Scanning is hard because there is no dominant grouping cue — figure/ground is ambiguous at every level.
Prescription, in order:
1. Remove internal borders and dividers; rely on the spacing scale (e.g. 16 within a group, 40 between groups) so proximity carries structure.
2. Keep **one** region mechanism per level — either a card *or* a background tint, not both.
3. If rows need separation for scanning at high density, use a very light hairline only, or zebra striping (uniform connectedness) rather than full borders.
4. Re-run the squint test: the section groups should survive, the rows should not compete with them.
Trade-off to state: fewer boundaries reduce weight but can hurt very dense data tables, where hairlines genuinely aid row tracking — so density determines how far to go.

**11.** Fix using **isolation (Von Restorff) plus figure/ground and size**: make the one or two most important metrics visually dominant — larger type, higher contrast, more space, possibly a wider tile — and demote the remaining tiles to a uniform secondary treatment. Group related metrics with proximity or a shared region so the dashboard reads as 2–3 clusters rather than 8 equal items. Add sensible ordering (most-decision-relevant first, serial position favours first and last).
Risk of over-applying: if several tiles get emphasis, isolation collapses and you are back to a flat field of equal weights; and heavy emphasis on a metric that is not universally the priority forces a single reading on users who came for a different question. Mitigation: let the emphasis follow the user's stated primary question, and consider configurability rather than a fixed hierarchy — while noting that configurable dashboards are rarely configured, so the default must still be right.

**12.** Model critique (delivered in this order — structure before surface):
1. **Primary task.** "First, what is this screen for? Assuming it is completing this form, everything should serve that."
2. **Grouping.** "The section headers are not reading as headers, because the space above a header is the same as the space between fields — proximity is not encoding the section structure, so I read one long list. I would increase between-section spacing to roughly double the within-section spacing."
3. **Field-label association.** "Each label sits equidistant between two fields, so proximity is ambiguous and users will associate labels with the wrong input, particularly when scanning. Tighten the label-to-its-own-field gap to the smallest step on the scale, and keep field-to-field larger."
4. **Hierarchy and emphasis.** "The primary action does not stand out — I would check how many filled buttons are on screen. Emphasis is relative, so one filled primary and the rest outlined or text restores the pop-out. Colour alone is not enough; weight and size should carry it too."
5. **Verification.** "I would squint at it or view it in greyscale to confirm the groups survive and the primary action is still the first thing my eye lands on."
6. **Next step.** "Then I would validate with a first-click test rather than assuming my grouping matches users' expectations."
*Marking:* the strong answer names the mechanism (proximity, isolation) and gives a specific fix; a weak one says "add more spacing and make the button pop."
