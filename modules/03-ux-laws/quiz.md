# Quiz — Module 03: UX Laws

15 questions. Target: 11/15. Worked solutions below, with marking notes on what a strong versus weak answer contains.

---

### Part A — Recall

**1.** Fitts's Law says movement time depends on:
- a) target size and colour
- b) distance to target and target size
- c) number of targets and their spacing
- d) user expertise and target size

**2.** Hick's Law describes a relationship that is:
- a) linear
- b) exponential
- c) logarithmic
- d) constant

**3.** The Doherty Threshold is approximately:
- a) 100 ms
- b) 400 ms
- c) 1 s
- d) 10 s

**4.** Tesler's Law states that:
- a) complexity should always be removed
- b) complexity is conserved and can only be moved
- c) users prefer simple interfaces
- d) engineering complexity should be minimised

**5.** The Peak–End Rule says an experience is judged primarily by:
- a) its average quality
- b) its total duration
- c) its most intense moment and its ending
- d) its beginning

**6.** Which law explains why the "Most popular" pricing tier gets chosen more often?
- a) Miller's Law
- b) Von Restorff Effect
- c) Postel's Law
- d) Parkinson's Law

---

### Part B — Short answer

**7.** Why are screen corners the fastest targets for a mouse, and why does that not transfer to touch?

**8.** Explain why "menus should have 7±2 items" is a misuse of Miller's Law, and state where the law genuinely applies.

**9.** Give the four conditions under which breaking an established convention is justified.

**10.** Name three techniques that improve perceived performance without changing actual speed, and state where each fails.

**11.** State the test for whether an urgency mechanic (countdown, low-stock badge) is legitimate rather than a dark pattern.

---

### Part C — Applied

**12.** A checkout has a 6-second payment authorisation step. Users double-tap "Pay" and some are charged twice. Give the design and interaction fixes, mapping each to a law.

**13.** A pricing page has three plans. All three have a coloured badge, all three buttons are filled, and the recommended plan is the middle one. What is wrong, using laws, and what would you change?

**14.** A PM wants to cut the settings screen from 40 options to 8 "because of Hick's Law." Respond.

**15.** A subscription product has good satisfaction scores but poor word of mouth and high churn at renewal. Which laws would you reach for, and what would you investigate first?

---
---

## Solutions

**1. b)** Distance and size — `MT = a + b·log2(2D/W)`. Colour and expertise affect search and the constants, not the law's variables.

**2. c)** Logarithmic: `RT = a + b·log2(n+1)`. This matters, because it means adding options has *diminishing* cost, which undercuts the common "fewer is always better" claim.

**3. b)** ~400 ms (Doherty & Thadhani, IBM, 1982).

**4. b)** Conserved and relocatable — to the user, the design, or the engineering.

**5. c)** Peak and end; duration is heavily discounted ("duration neglect").

**6. b)** Von Restorff (isolation) — plus anchoring and the decoy effect if the tiers are arranged to make it look like the best value.

---

**7.** The pointer is clamped by the screen boundary, so an edge target is effectively infinite in width along that axis, and a corner is infinite in two axes — you can throw the cursor without precision and it stops on target. It does not transfer to touch because there is no clamping: a finger can land beyond the physical edge and misses entirely, the finger occludes the target, and reachability (thumb arc) dominates. On touch, the equivalent insight is the thumb zone — the bottom band of the screen is cheapest, the top corners most expensive.
*Marking:* a strong answer names clamping as the mechanism; a weak one just says "corners are easy."

**8.** Miller's 1956 paper was about the span of immediate memory and absolute judgement, measured in *chunks*. A menu is visible on screen, so nothing is being held in memory — the constraint is visual search and information scent, not memory span. Modern estimates for working memory are closer to ~4 chunks anyway. The law genuinely applies wherever the interface removes information the user still needs: codes to be carried across steps, table headers scrolling out of view, instructions in a dismissed modal, values that must be transcribed between screens.
*Marking:* the reframe ("visible items are not memory") is the whole point of the question.

**9.** (1) The new model is meaningfully better on a dimension the user cares about; (2) the task is frequent enough that the learning cost amortises; (3) you can afford a bridge — onboarding, familiar fallback, or an in-place teaching cue; (4) you have a way to measure whether the bet worked. Absent all four, take the convention.

**10.** Any three, with failure modes:
- **Optimistic UI** — shows the result before the server confirms. Fails when the operation can genuinely fail in a way that matters (payments, irreversible actions); you then have to un-tell the user, which is worse than waiting.
- **Skeleton screens** — outline the incoming layout. Fail when the wait exceeds a few seconds; a skeleton that persists reads as a hang, and they mislead if the final layout differs.
- **Prefetch/preload during decision time** — free time to fetch the likely next screen. Fails on metered connections, and wastes resources when prediction accuracy is low.
- **Staged progress messaging** — occupied time feels shorter. Fails when the stages are fictional; users notice fake progress that stalls.

**11.** Three-part test: **Is the constraint real** (is inventory actually held, does the price actually change)? **Is it described accurately** (does the copy match the mechanism)? **Does it survive scrutiny** — does the timer reset on reload, does "3 left" change randomly? If the mechanic fails any part, it is coercion, and increasingly a regulatory exposure, not just an ethical one.

**12.** Mapped fixes:
- **Doherty Threshold** — 6 s is far past 400 ms, so the interaction feels broken. Acknowledge the tap in under 100 ms with an immediate state change on the button itself (label change + disabled state), so the user gets confirmation their action registered.
- **Doherty / response bands** — 6 s falls in the 1–10 s band: show staged determinate progress ("Authorising payment… Confirming order…") rather than an indeterminate spinner, so the wait is legible.
- **Postel's Law / robustness** — accept the messy real case: make the request idempotent so a double submission cannot double-charge. This is a UX requirement expressed as an engineering one; disabling the button alone is insufficient because network retries and back-button re-posts exist.
- **Peak–End** — a double charge is a catastrophic negative peak that dominates memory of the whole product. Add a fast, visible refund/undo path if it does occur.
- **Fitts's Law (anti-)** — if "Pay" is enormous and adjacent to nothing, the double-tap is even cheaper; combine the disabled state with a brief post-tap dead zone.
*Marking:* full credit requires idempotency (the real fix) *and* immediate acknowledgement (the perceived fix). Naming only the spinner is a partial answer.

**13.** What is wrong:
- **Von Restorff requires a plain background.** Three badges means no isolation, so nothing pops and the emphasis budget is spent for zero effect.
- **Three filled buttons destroy the pre-attentive pop-out** (Module 02): the target no longer differs from the distractors, so visual search becomes serial and the user must read all three.
- **Serial position** puts memory weight on the first and last plans; if the recommendation is in the middle it fights recall, though for a visible comparison table scanning matters more than memory.
Changes: one badge on one plan; one filled button (the recommended plan), the others outlined or text; keep the recommendation visually isolated on exactly one attribute; ensure the badge is not colour-only (add text) for accessibility. Then verify with data rather than assertion — plan-selection distribution before and after.

**14.** Model response (agree with the goal, correct the reasoning):
- Hick's Law is **logarithmic**, so going from 40 to 8 options saves far less decision time than the intuition suggests — roughly the difference between log2(41) and log2(9), not a fivefold gain.
- The law also assumes **equally probable choices**; settings are not — a handful are changed constantly and the rest almost never, so ordering and grouping do more than deletion.
- A settings screen is mostly a **visual search** problem, not a decision problem. Search, grouping into labelled sections, and surfacing the top-changed settings address it directly.
- **Tesler's Law**: the complexity does not disappear when we delete the option; it moves to support tickets, to workarounds, or to users who now cannot do their job.
- Counter-proposal: instrument usage, group into 5–6 sections validated by a card sort, promote the top settings, add search, move verified-low-usage settings behind "Advanced," and only then consider removing options with near-zero usage — reversibly, behind a flag.
*Marking:* the strong answer keeps the PM's goal (make it manageable) while rejecting the mechanism, and offers a measurable alternative. Simply saying "Hick's Law does not say that" is a half answer.

**15.** Laws to reach for and the investigation:
- **Peak–End Rule** first. Satisfaction surveys sample the average or the recent moment; word of mouth and renewal decisions are driven by the remembered experience — the worst moment and the ending. Investigate: map the journey and find the emotional low (a failed support interaction, a billing surprise, a data loss, a migration), and examine the renewal moment itself, which *is* the ending being judged.
- **Aesthetic–Usability Effect** as a methodological caution: if the product is attractive, self-reported satisfaction will be inflated relative to actual task performance, so I would look at behavioural data (task success, support contacts, time-to-value) rather than trusting the score.
- **Zeigarnik / Goal-Gradient** for whether users ever reached the product's core value; churn at renewal often means the value moment never landed, not that the last month was bad.
- **Jakob's Law** if a recent redesign reset learned models — check whether churn concentrates in tenured users.
First investigation: segment churn by tenure and by whether the account hit the activation milestone, then interview 8–10 churned users with a focus on the worst moment and the renewal experience specifically.
