# Mixed Exam 1 — Foundations

30 questions drawing on Modules 01–06 (foundations, psychology, UX laws, Gestalt, heuristics, visual design). Target: 22/30. Worked solutions below, with marking notes on what a strong versus weak answer contains.

---

### Part A — Recall

**1.** ISO 9241-210 defines user experience as a person's perceptions and responses resulting from:
- a) the use of a product only
- b) the use and anticipated use of a product, system, or service
- c) the visual interface of a product
- d) the usability of a product measured after a task

**2.** In the Double Diamond, divergence in the *second* diamond means:
- a) gathering more research about the problem
- b) generating many candidate solutions before narrowing to one
- c) recruiting a wider participant pool
- d) expanding the definition of the problem statement

**3.** Which of Nielsen's five usability components is most often confused with efficiency?
- a) learnability
- b) memorability
- c) satisfaction
- d) errors

**4.** The Gulf of Execution is the gap between:
- a) what the system does and what it displays
- b) the user's intention and the actions the system makes available
- c) the designer's model and the system model
- d) the user's expectation and the system's response time

**5.** Which of these is *not* a pre-attentive attribute?
- a) colour hue
- b) size
- c) alphabetical order
- d) orientation

**6.** Hick's Law describes reaction time as a function of the number of alternatives, and the relationship is:
- a) linear
- b) quadratic
- c) logarithmic
- d) step-shaped

**7.** The Doherty Threshold is approximately:
- a) 100 ms
- b) 400 ms
- c) 1 s
- d) 3 s

**8.** Tesler's Law (the Law of Conservation of Complexity) states that:
- a) all complexity can be designed away with enough iteration
- b) every application has an irreducible complexity that must be borne by someone
- c) users prefer complex interfaces when they are experts
- d) complexity increases as the square of the feature count

**9.** The strongest Gestalt grouping cue is:
- a) similarity
- b) proximity
- c) common region
- d) uniform connectedness

**10.** Which Nielsen heuristic does an unlabelled icon toolbar most directly violate?
- a) User control and freedom
- b) Recognition rather than recall
- c) Error prevention
- d) Flexibility and efficiency of use

**11.** WCAG's minimum contrast requirement for normal-size body text is:
- a) 3:1
- b) 4.5:1
- c) 7:1
- d) 2:1

**12.** Compared with HSL, OKLCH is preferred for building colour ramps because:
- a) it has a wider gamut on every display
- b) equal lightness values look equally light across hues
- c) it is easier for engineers to parse
- d) it guarantees WCAG conformance

---

### Part B — Short answer

**13.** Write a Lean UX hypothesis for adding a saved-search feature to a job board, and state which part of it is the falsifiable claim.

**14.** Give a one-sentence distinction between a persona and a Job-to-be-Done statement, then say when each is the wrong tool.

**15.** Name the three models present in any product, and say which one the designer directly controls.

**16.** Distinguish intrinsic, extraneous, and germane cognitive load, and state which a designer should attack first and why.

**17.** Explain why "7±2" is a misuse of Miller's Law, and give the number a designer should actually work with.

**18.** State the strength ordering of the four main Gestalt grouping cues and explain why the ordering is practically useful rather than trivia.

**19.** Describe the squint test: what it is, four ways to run it, and what you are looking for.

**20.** Give the severity-rating dimensions used in a heuristic evaluation and explain why severity is rated separately from the heuristic violated.

**21.** Explain the difference between a primitive and a semantic colour token, and state what semantic tokens buy you.

**22.** Why is "never encode meaning by colour alone" a stronger rule than "check your contrast ratios"?

---

### Part C — Applied

**23.** A team ships a redesigned navigation. SUS rises from 64 to 79, but task success in the benchmark study is flat and support contacts about "where do I find X" are unchanged. Diagnose, naming the relevant law.

**24.** A mobile banking app puts "Transfer" — the most frequent action — in the top-right corner, and "Delete account" as a small text link at the bottom of a settings list. Critique both placements using laws, and say what you would change.

**25.** A settings page uses cards around each group, hairline borders between rows inside the cards, and a divider between cards. Users call it "heavy" and "hard to scan." Diagnose using Gestalt and prescribe fixes in order.

**26.** You are given 45 minutes to heuristically evaluate a checkout flow before a stakeholder meeting. Describe exactly what you would do, and state the two most important limitations you would declare in the room.

**27.** A pricing page shows three plans. All three cards have a coloured badge, all three CTAs are filled buttons in the brand colour, and the recommended plan sits in the middle. Explain what is wrong using at least three concepts, and give the fix.

**28.** A checkout has a six-second payment authorisation step. Users double-tap "Pay" and some are charged twice. Give the design, interaction, and engineering fixes, mapping each to a law.

**29.** A dashboard shows twelve metric tiles, all the same size, in a 4×3 grid. Users say they "cannot tell what matters." Give a fix grounded in visual hierarchy and Gestalt, and name the risk of over-applying it.

**30.** A PM says: "Our onboarding has a 62% completion rate. Let's cut it from six steps to three — Hick's Law." Write the response you would give in the meeting.

---
---

## Solutions

**1. b)** Perceptions and responses resulting from the use *and anticipated use* of a product, system, or service. The "anticipated" clause is the point of the question: the definition covers before, during, and after — marketing promises, the app-store listing, and the memory of last week's failure are all in scope. Option (a) is the common under-reading; (c) confuses UX with UI, which is precisely what the definition rules out.

**2. b)** Generating many candidate solutions before narrowing. The first diamond diverges and converges on the *problem* (Discover/Define); the second diverges and converges on the *solution* (Develop/Deliver). Option (a) and (d) describe first-diamond activity, which is the standard mix-up.

**3. b)** Memorability. Efficiency is how fast an experienced user performs tasks; memorability is how easily a user who has been away re-establishes proficiency. They pull apart sharply in products used infrequently — a tax tool can be efficient in a single sitting and disastrous at memorability twelve months later.

**4. b)** The gap between the user's intention and the actions the system makes available. Option (a) is the Gulf of *Evaluation* — perceiving and interpreting system state. Execution is "how do I do this?"; evaluation is "did it work?"

**5. c)** Alphabetical order. Pre-attentive attributes are processed in roughly 200 ms without focused attention: hue, size, orientation, motion, enclosure, position, and a handful of others. Order requires reading and conscious sequential processing, so it is not pre-attentive — which is exactly why an alphabetical list of 40 items does not "pop" the item you want.

**6. c)** Logarithmic — `RT = a + b·log2(n+1)`. This matters because adding options has *diminishing* cost, which undercuts the reflexive "fewer choices is always better" argument. See Q30.

**7. b)** ~400 ms (Doherty & Thadhani, IBM, 1982) — the threshold below which the system keeps up with the user and attention does not wander. 100 ms is the separate acknowledgement budget for "this feels instantaneous"; 1 s is where you should show something; 10 s is where the user leaves.

**8. b)** Every application has an irreducible complexity, and the only question is who bears it: the user, the designer, or engineering. Option (a) is the misreading the law was coined to refute.

**9. d)** Uniform connectedness — an explicit visual connection (a line, a shared container edge, a connector) beats every other cue. Common region (c) is second and is the more common answer, which is why it is the tempting distractor.

**10. b)** Recognition rather than recall. An unlabelled icon requires the user to retrieve the meaning from memory rather than recognise it on screen. Error prevention (c) is a downstream consequence, not the primary violation.

**11. b)** 4.5:1 for normal text (WCAG 1.4.3, level AA). 3:1 applies to large text and, under 1.4.11, to UI component boundaries and meaningful graphics. 7:1 is the AAA threshold.

**12. b)** OKLCH is perceptually uniform, so equal lightness values look equally light across hues; HSL is not, and a yellow and a blue at the same HSL lightness differ wildly in perceived brightness. Option (d) is a trap: no colour space guarantees conformance — contrast must still be measured against relative luminance.

---

**13.** Model hypothesis, using the standard Lean UX frame:

> "We believe that giving job seekers who search repeatedly a saved-search feature with email alerts will result in more of them returning within seven days of their first search. We will know we are right when 7-day return rate for users who save a search is at least 15 percentage points above the matched control, and saved-search alert click-through exceeds 10%."

The falsifiable claim is the *outcome* clause — the return-rate lift with a stated threshold and a comparison group. Everything before it ("we believe that…") is the assumption; the value of the format is that it forces you to write down a number you could be wrong about, in advance, before you are emotionally invested in shipping.

*Marking:* a strong answer names the outcome and the threshold as the falsifiable part, and includes a comparison. A weak answer writes "we believe saved search will improve engagement" — no metric, no threshold, no way to be wrong, which is a wish rather than a hypothesis. Note the trade-off: a tightly specified hypothesis risks being unmeasurable in the time available, so the threshold should be one you can actually observe within the decision window.

**14.** A persona is a composite description of a *user type* — goals, context, behaviours, and often demographics. A JTBD statement describes a *situation* and the progress someone wants to make in it: "When I am commuting and have twenty minutes, I want to find roles that match my search without re-typing filters, so I can apply before I reach the office."

When each is wrong: personas are the wrong tool when the design question is about a situation that cuts across user types — everyone in a hurry behaves like everyone else in a hurry, and a persona will hide that. JTBD is the wrong tool when the differences that matter genuinely *are* about the person rather than the moment — accessibility needs, expertise level, regulatory role, and language are properties of the user, not the situation, and a job statement will flatten them.

*Marking:* the strong answer gives a failure mode for each, not just definitions. The weakest common answer is "personas are made up and JTBD is real," which is a slogan, not an analysis — a badly researched job statement is exactly as fictional as a badly researched persona.

**15.** The three models:

- **System model** — how the thing actually works internally.
- **Conceptual model** — the story the design tells about how it works, expressed through the interface, its vocabulary, and its behaviour.
- **Mental model** — what the user actually believes, built from this interface, from every other product they have used, and from the world.

The designer directly controls only the **conceptual model**. The system model belongs to engineering and the domain; the mental model forms in the user's head and can only be *influenced*, never set. Most "confusing interface" problems are a mismatch between the conceptual model on offer and the mental model users arrive with — which is why the fix is often relabelling and re-sequencing rather than adding explanation.

**16.** 
- **Intrinsic load** — the inherent difficulty of the task itself. Filing a tax return is intrinsically harder than liking a post. You can restructure and sequence it, but you cannot remove it.
- **Extraneous load** — load created by the *presentation*: unclear labels, inconsistent patterns, information split across screens, jargon, decorative noise, forcing users to hold values in memory between steps.
- **Germane load** — effort that goes into building durable understanding: learning the model, forming a schema. This is productive load.

Attack **extraneous** first, because it is pure waste — it is load you created and can remove without reducing what the user accomplishes, and removing it frees capacity for the other two. Reducing intrinsic load usually means removing capability (a product decision, not a design one) and reducing germane load actively harms learning.

*Marking:* full credit requires the *reason* for the ordering — that extraneous load is self-inflicted and its removal is free — not just the correct ordering. A weak answer says "reduce all cognitive load," which is wrong: germane load is the load you want.

**17.** Miller's 1956 paper concerned the span of immediate memory and absolute judgement, measured in *chunks* held in working memory. It was never about how many items should appear in a visible list. A menu on screen is not in memory — it is on screen — so the constraint is visual search and information scent, not memory span. Applying "7±2" to navigation items, form fields, or dashboard tiles is cargo cult.

The number to work with is **about 4 chunks** — the modern estimate (Cowan) for unrelated items held in working memory. Use it where the interface genuinely removes information the user still needs: a verification code to carry across screens, table headers that scroll out of view, instructions inside a modal that must be dismissed, a value transcribed between two steps. The design implication is not "shorten menus," it is "stop making people carry things."

*Marking:* the reframe — visible items are not held in memory — is the whole question. Stating "~4 chunks" without the reframe is half an answer.

**18.** **Uniform connectedness → common region → proximity → similarity.**

The ordering is useful because these cues routinely *conflict* in real layouts, and knowing which wins tells you which one to fix. If a card boundary (common region) encloses A and B while your spacing (proximity) groups B and C, users will perceive A+B and your spacing work is invisible. Designers who do not know the ordering respond to "these don't look grouped" by adding *more* cues — a border, plus a tint, plus a heading — which produces the heavy, flat result diagnosed in Q25. The correct move is to identify the strongest cue currently in play and change *that* one.

**19.** The squint test is deliberately degrading your view of a design so you see only what pre-attentive perception delivers in the first ~200 ms: the groups, the hierarchy, and the figure/ground separation, with all detail and all semantic content stripped out.

Four ways to run it: physically squint at the screen; apply a Gaussian blur to a screenshot; zoom the browser or canvas out to roughly 25%; convert the screenshot to greyscale — which has the bonus of verifying you have not encoded meaning with colour alone.

What you are looking for: (1) do the intended things group, and does anything group that should not; (2) is there a single clear first stop for the eye; (3) does the primary action survive as distinct; (4) is figure cleanly separable from ground. If the answer to any of these is no, the problem is structural and no amount of copy editing or icon polish will fix it.

**20.** Severity is typically rated on three dimensions, combined into a single 0–4 scale:

- **Frequency** — how often will users hit it? A problem on the checkout path outranks one in an admin corner.
- **Impact** — how hard is it to overcome when hit? Recoverable annoyance versus task failure versus data loss.
- **Persistence** — is it a one-time learning hurdle, or does it bite on every single use?

Severity is rated separately from the heuristic violated because **the heuristic tells you what kind of problem it is; severity tells you whether to spend money on it.** They are orthogonal: a "consistency and standards" violation can be trivial (a button radius differs by 2px) or catastrophic (the word "archive" means delete in one screen and hide in another). Merging them would let a taxonomy decide your roadmap. In practice, keep them in separate columns and have multiple evaluators rate severity independently before discussing, because severity is where evaluator bias concentrates.

*Marking:* the strong answer names all three dimensions *and* the orthogonality argument. A weak answer says "high, medium, low" with no criteria, which produces a rating nobody can defend when a stakeholder pushes back.

**21.** A **primitive token** names a raw value: `blue-600`, `grey-100`, `space-4`. A **semantic token** names a *role*: `color-text-primary`, `color-surface-raised`, `color-border-danger`, `color-action-primary`. Components consume semantic tokens; semantic tokens resolve to primitives.

What that buys you:
- **Theming for free.** Dark mode, a high-contrast mode, and a white-label brand become remappings of the semantic layer rather than rewrites of every component.
- **Auditability.** `color-border-danger` on a neutral divider is visibly wrong in review; `#D93025` is not.
- **A single place to fix contrast.** If `color-text-secondary` fails 4.5:1, you change one token, not 200 usages.

The trade-off is indirection: three layers means a designer chasing a colour has three hops to make, and teams under-invest in naming, which produces semantic tokens that are actually primitives wearing a costume (`color-blue-button`). The discipline is that a semantic name must describe the *job*, so that changing the value never makes the name a lie.

**22.** Because contrast is a *threshold* rule and colour-only encoding is a *total failure* rule.

A contrast failure degrades the experience: text at 3.8:1 instead of 4.5:1 is harder to read, and worse in sunlight or on a poor screen, but the information is still there for most people. Encoding meaning by colour alone *removes the information entirely* for anyone who cannot make that discrimination — roughly 8% of men have some colour-vision deficiency — and also for anyone printing in greyscale, using a monochrome display, in bright sunlight, or under a display filter. A red-versus-green status dot with no icon, label, or position difference conveys nothing to those users; there is no partial credit.

Both rules matter, but they are different in kind: one is about legibility on a continuum, the other is about whether the channel exists at all. Pair colour with an icon, a label, a pattern, or a position, and the rule costs almost nothing to follow.

*Marking:* the distinction between "degraded" and "absent" is the answer. Reciting both rules without separating them is a weak answer.

**23.** Diagnosis: this is the **Aesthetic–Usability Effect**. Users perceive attractive interfaces as more usable, and that perception inflates *self-reported* measures without touching *behavioural* ones. SUS is attitudinal; task success and support contacts are behavioural. A 15-point SUS jump with flat task success is the classic signature of a visual refresh that did not change the underlying findability problem.

What it means in practice:
- The redesign probably did improve perceived quality, credibility, and possibly first impressions — those are real and worth something, particularly for acquisition and trust.
- It did **not** fix the information architecture. "Where do I find X" is a findability question; navigation styling does not answer it and labels and structure do.

What I would do next: separate the two questions. Run a tree test on the current structure to isolate whether the problem is the hierarchy or the labels — low directness with high success points at ambiguous labels, low success points at the structure. Mine the support-contact text and zero-result search queries for the users' actual vocabulary, since those are free and continuous. Then re-benchmark task success against the same task set.

The broader caution: the Aesthetic–Usability Effect is a methodological hazard, not just a design phenomenon. It means attractive prototypes score better in usability tests than they deserve to, so a team that only measures attitudinally will systematically ship pretty products that do not work.

*Marking:* naming the law is worth little on its own. The strong answer states *why* the two metric families diverged (attitudinal versus behavioural), and proposes a method that isolates structure from labels. A weak answer concludes "the redesign failed" — it did not; it succeeded at something that was not measured by task success.

**24.** **"Transfer" in the top-right corner.**
By **Fitts's Law**, movement time depends on distance and target size. On a phone held one-handed, the top-right corner is the single most expensive region for a right-handed thumb and worse for a left-handed one — it requires a grip shift, which is not just slow but risky when holding the phone in one hand. The screen-corner advantage that makes corners cheap on desktop does **not** transfer to touch: on desktop the pointer is clamped by the screen edge, making the corner effectively infinite in two axes; a finger has no clamping, can land past the physical edge, and occludes the target it is aiming at.

Fix: move the primary, high-frequency action into the bottom thumb zone — a bottom bar, a persistent bottom-anchored primary button, or a bottom sheet. Keep it large. Frequency should determine reach cost: the most-used action gets the cheapest position.

**"Delete account" as a small bottom text link.**
This one is more interesting, because it is the *right* instinct implemented in a way that fails. Making a destructive, irreversible action small and distant is a legitimate application of Fitts's Law in reverse — high motor cost is an appropriate guard for high consequence, and it aligns with Nielsen's error prevention. But a small text link is the wrong instrument:
- It is likely below the 24×24 CSS px minimum target size, which is a WCAG 2.2 failure (2.5.8) affecting users with motor impairments — you have added friction for the wrong population.
- It is also *low visibility*, which is a different property from *high cost*. Users who genuinely want to close their account cannot find it, which drives support contacts and, in some jurisdictions, regulatory exposure around cancellation friction.

Fix: keep it distant and de-emphasised in *weight* (not the brand colour, not a filled button), but give it a proper touch target and a clear label. Put the friction where it belongs — in a confirmation step that requires deliberate action (typing the account name, re-authenticating) and states exactly what will be lost and whether it is recoverable. That is error prevention with a real cost, rather than a target that is merely hard to hit.

*Marking:* the strong answer distinguishes *motor cost* from *visibility* and notes that "hard to tap" penalises disabled users rather than careless ones. A weak answer says "make Transfer bigger and Delete smaller."

**25.** Diagnosis: **too many competing boundaries.** Cards (common region), internal hairlines, and dividers between cards are three simultaneous grouping mechanisms applied to three nested levels. Because they are all *boundary* cues of similar strength, every level reads as equally important and the hierarchy flattens — there is no dominant cue, so the eye has no instruction about what to group first. Each boundary also carries visual weight, which is where "heavy" comes from: the page is largely made of lines rather than content.

Prescription, in order:

1. **Pick one region mechanism per level.** Either a card *or* a background tint, never both. If the cards are doing the group-level work, the dividers between cards are redundant — the gap between cards already separates them.
2. **Let spacing carry the within-group structure.** Remove internal hairlines and use the spacing scale — for example 8 within a row, 16 between rows, 40 between groups. Between-group spacing should be roughly double within-group spacing; the most common spacing bug is having them equal or inverted, which makes proximity encode the wrong structure.
3. **Restore hierarchy with weight, not boundaries.** Group headings get size and weight; rows stay neutral. Typographic hierarchy is cheap and does not add visual noise.
4. **Re-run the squint test.** At 25% zoom the group structure should survive and the rows should not compete with it.

Trade-off to state explicitly: this prescription assumes moderate density. In a genuinely dense data table, hairlines earn their weight — they aid row tracking across a wide row, and removing them causes users to slip between rows. So the answer is density-dependent: strip boundaries aggressively in a settings page, keep a very light hairline or zebra striping in a table. The principle that survives both cases is *one grouping mechanism per level*.

**26.** With 45 minutes, the plan:

1. **First 5 minutes — scope and set-up.** Define the exact flow (from cart to confirmation), the persona and device I am evaluating as, and the heuristic set. Nielsen's ten as the shared vocabulary, because everyone in the meeting will recognise the terms and that makes findings actionable rather than debatable.
2. **Next 10 minutes — a clean pass with no notes.** Walk the flow as a first-time user on the target device, without stopping to write. This preserves the first-encounter reaction, which is destroyed the moment you start annotating.
3. **Next 20 minutes — a systematic pass.** Screen by screen, note every issue against a heuristic. Deliberately check the states that flows hide: validation errors, an expired card, a declined payment, back-button behaviour, and refresh mid-flow. Most checkout problems live in the error paths, not the happy path.
4. **Final 10 minutes — rate and sort.** Score each finding 0–4 on frequency, impact, and persistence, then sort by severity, not by screen order. Write the top five with a one-line description, the heuristic, the severity, and a suggested direction. Screenshots with a single annotation each.

The two limitations I would declare in the room, unprompted:

- **This is not user research.** A heuristic evaluation surfaces violations of known principles; it cannot tell me whether real users actually fail, and it systematically over-predicts some problems while missing domain-specific misunderstandings entirely. Anything on this list is a hypothesis about a problem, not evidence of one.
- **A single evaluator finds a minority of the issues.** The method assumes 3–5 independent evaluators whose findings are merged; one person in 45 minutes will miss a substantial share, and my severity ratings are unvalidated because there is nobody to disagree with me. Declaring this protects the finding list from being treated as complete.

*Marking:* the strong answer includes the error-path pass and declares the limitations *before* being asked. A weak answer describes walking through the screens and listing problems, with no severity method and no statement of what the method cannot do — which is exactly how a heuristic evaluation gets over-claimed and then discredited.

**27.** What is wrong:

- **Von Restorff requires a plain background.** The isolation effect works because one item differs from a uniform field. Three badges means nothing is isolated, so no plan pops and the entire emphasis budget has been spent for zero effect.
- **Three filled brand-colour CTAs destroy the pre-attentive pop-out.** Pop-out depends on the target differing from *all* distractors on some pre-attentive attribute. When all three buttons are identical, visual search becomes serial — the user must read all three cards to find the recommended one, which is precisely the work the design was supposed to save them.
- **Serial position** places recall weight on the first and last items, so the middle plan is the weakest position for memory. For a side-by-side comparison table this matters less than it would for a list read over time, since everything is visible at once — but it still means the middle plan needs to *earn* its prominence visually, and here nothing does.
- **Colour is carrying meaning alone.** If the badge is distinguished only by hue, it fails for users with colour-vision deficiency and in greyscale.

The fix:
- **One** badge, on one plan, with text ("Most popular" / "Best value") not just colour.
- **One** filled button — on the recommended plan. The other two become outlined or text buttons. Emphasis is relative; you cannot make one thing prominent without making the others less so.
- Reinforce the recommendation on a second, non-colour channel: slightly larger card, more internal space, or a raised elevation. One attribute is enough for pop-out; a second makes it robust in greyscale.
- Check the badge and button meet 4.5:1 for text and 3:1 for the button boundary.

Then verify with data rather than assertion: compare plan-selection distribution before and after. The trade-off worth naming is that a strong recommendation *works* — it will shift selection — which places an ethical obligation on the recommendation being genuinely the best fit for most users rather than the highest-margin one. Anchoring and decoy effects are equally available to a design that is steering people wrongly.

**28.** The six-second gap is well past every relevant threshold, and there are three distinct failures here that need three distinct fixes.

**Design fix — acknowledge in under 100 ms.** By the **Doherty Threshold** (~400 ms), six seconds is far outside the band where the system keeps up with the user, and the immediate cause of the double-tap is that the first tap produced no visible change. Change the button's own state instantly: label to "Authorising…", disabled appearance, spinner in place. The acknowledgement must be *on the button*, at the locus of attention — a status change elsewhere on the page will be missed (change blindness).

**Interaction fix — make the wait legible.** Six seconds sits in the 1–10 s band, where an indeterminate spinner reads as a hang. Use staged, determinate progress with honest labels: "Authorising payment… Confirming with your bank… Completing order." Occupied time feels shorter than unoccupied time, and named stages tell the user the system is progressing rather than stuck. The trade-off: stages must be real. Fictional progress that stalls at 90% is worse than no progress bar, because it destroys trust in every subsequent progress indicator you ship.

**Engineering fix — idempotency.** This is the actual fix and the others are palliative. Make the payment request idempotent with a client-generated key so a duplicate submission cannot produce a second charge. Disabling the button is *not* sufficient, because network retries, back-button re-posts, and impatient page refreshes all bypass the UI entirely. This is **Postel's Law** applied properly — be liberal in what you accept: the system must tolerate the messy real-world input of a user who taps twice, rather than requiring users to behave correctly.

**Recovery fix — Peak–End.** A double charge is a catastrophic negative peak, and by the Peak–End Rule it will dominate the memory of the entire product regardless of how good everything else was. Even with idempotency shipped, there must be a fast, visible, self-service refund or dispute path, and the confirmation email must make the single charge unambiguous. Recovering well from a failure can produce a better remembered experience than never failing at all; recovering badly is unrecoverable.

**A note on Fitts's Law (anti-application).** If "Pay" is enormous and has nothing near it, the second tap is extremely cheap to make. Combine the disabled state with a brief post-tap input dead zone so a reflexive second tap lands on nothing.

*Marking:* full credit requires **idempotency** — the real fix — *and* the sub-100 ms acknowledgement — the perceived fix. Naming only the spinner is a partial answer. A candidate who says "disable the button" and stops has fixed the demo but not the system.

**29.** The problem is that twelve tiles of identical size and weight form a uniform field, and a uniform field has no hierarchy by definition. Pre-attentive pop-out cannot operate when every element is identical on every attribute, so the user is forced into serial reading of twelve items — which is slow enough that they give up and report the dashboard as unusable.

The fix, in order:

1. **Establish a first stop.** Identify the one or two metrics that actually drive a decision and make them dominant: larger type for the value, a wider tile, more surrounding space, higher contrast. Size and position are both pre-attentive, so this works in the first 200 ms.
2. **Group with proximity or common region.** Twelve equal items is beyond comfortable scanning; three clusters of four is not. Group by the question they answer — acquisition, engagement, revenue — with clear between-group spacing at roughly double the within-group spacing, and a labelled heading per cluster.
3. **Demote the rest deliberately.** Secondary tiles get a uniform, quieter treatment. Emphasis is relative: you cannot promote without demoting.
4. **Order for serial position.** The first and last positions carry weight; put the most decision-relevant metric first.

The risk of over-applying: **if you emphasise four tiles, you have emphasised none.** Isolation collapses the moment the isolated set stops being a small minority, and you are back to a flat field with more visual noise than before. A second risk is that heavy fixed emphasis imposes one reading on a dashboard whose users arrive with different questions — the person checking revenue and the person checking error rates are not served by the same hierarchy.

Mitigation and its trade-off: the emphasis should follow the *primary* question the dashboard exists to answer, established by asking users what decision they make with it. Configurability is the obvious escape, but it is a weak one — configurable dashboards are overwhelmingly left in their default state, so the default must be right regardless. If the audience genuinely splits into distinct jobs, the honest answer is separate dashboards rather than one configurable compromise.

**30.** Model response — agree with the goal, correct the mechanism, propose something measurable:

"I want the same thing you do, and I think there is real room here. But Hick's Law will not get us there, for three reasons.

**First, the relationship is logarithmic, not linear.** Hick's Law is about choosing among simultaneous alternatives, and the cost grows with `log2(n+1)`. Even if it applied cleanly, going from six to three would save far less time than the intuition suggests — nothing close to halving it.

**Second, it does not apply to sequential steps.** Hick's Law describes selecting one option from a set presented at once, like a menu. A six-step onboarding is not one six-way choice; it is six separate tasks in sequence. The relevant question is what each step *asks for* and whether the user is willing and able to provide it at that moment.

**Third — Tesler's Law — the complexity does not disappear when we delete steps.** If those steps collect information the product genuinely needs, cutting them moves the work somewhere else: to a half-configured account, to a confusing first session, or to support. We will see completion rise and activation stay flat, which looks like a win in the deck and is not one.

Here is what I would do instead. Our 62% is an average, and averages hide the broken segment — I want the drop-off broken out per step and segmented by platform, acquisition channel, and geography, because usually one step and one segment account for most of the loss. Then I would sort each dropped user into one of three causes: **cannot** (a usability or technical failure — a field that rejects valid input, a permission prompt that fails on one OS), **will not** (we are asking for something before we have shown any value — a credit card, a workspace name, contacts access), or **should not** (we acquired people this product does not serve, which no onboarding change will fix and which is an acquisition problem).

Those three have completely different fixes. 'Cannot' is a bug list. 'Will not' is a sequencing problem — defer the ask past the first value moment, or make it optional and let people complete it later. 'Should not' belongs to marketing.

So: give me the funnel by step and segment plus five session recordings of drop-offs, and I will come back in a week with a ranked list. If the data says a step is pure friction with no downstream value, I will be first in line to cut it — and we should cut it behind a flag so we can see activation, not just completion, before we commit."

*Marking:* the strong answer keeps the PM's goal while rejecting the mechanism, corrects the law precisely (logarithmic; simultaneous not sequential), invokes Tesler's Law for the relocated complexity, distinguishes completion from activation, and ends with a concrete measurable proposal and a reversible rollout. Simply saying "that is not what Hick's Law means" is a half answer and, in a real meeting, a losing one — being right about the citation while offering no alternative gets the steps cut anyway.

---

<!-- nav -->
[← Previous: Quizzes](README.md) · [↑ Quizzes](README.md) · [Next: Mixed Exam 2 — Practice →](mixed-exam-2.md)
