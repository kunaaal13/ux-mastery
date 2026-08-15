# Quiz — Module 05: Heuristics & Evaluation

14 questions. Target: 10/14.

---

### Part A — Recall

**1.** "Visibility of system status" primarily addresses:
- a) the Gulf of Execution
- b) the Gulf of Evaluation
- c) cognitive load
- d) Fitts's Law

**2.** Nielsen's severity scale runs from:
- a) 1–3
- b) 0–4
- c) 1–5
- d) low/medium/high only

**3.** Recommended number of independent evaluators for a heuristic evaluation:
- a) 1
- b) 2
- c) 3–5
- d) 10+

**4.** A user who intends the right action but mis-taps has made a:
- a) mistake
- b) slip
- c) violation
- d) lapse of consistency

**5.** "Aesthetic and minimalist design" is fundamentally about:
- a) using less colour
- b) competition for attention between elements
- c) flat design
- d) reducing feature count

**6.** Which is NOT one of Nielsen's ten?
- a) Error prevention
- b) Recognition rather than recall
- c) Accessibility for all users
- d) Help and documentation

---

### Part B — Short answer

**7.** List Nielsen's ten heuristics.

**8.** Give the four parts of a good error message, and one common violation of each.

**9.** State the four cognitive walkthrough questions and map each to a fix type.

**10.** Name the three factors that determine severity, and give an example where a rare problem outranks a frequent one.

**11.** What are the two things heuristic evaluation fundamentally cannot tell you?

---

### Part C — Applied

**12.** A checkout shows all validation errors only after submit, clears the card fields, and displays "Invalid input" in red above the form. List every heuristic violated, rate severity, and give the fix.

**13.** You are asked to critique a product in 20 minutes in an interview. Outline exactly how you spend the time, and name the step most candidates skip.

**14.** Write six heuristics you would use to evaluate an AI chat assistant, with a one-line rationale each, and explain why Nielsen's set alone is insufficient here.

---
---

## Solutions

**1. b)** Gulf of Evaluation — perceiving and interpreting system state.

**2. b)** 0–4, where 0 is "not a problem" and 4 is "catastrophe, must fix before release."

**3. c)** 3–5. A single evaluator finds roughly a third of problems; returns flatten after about five. They must evaluate *independently* before aggregating, or they converge.

**4. b)** A slip — right intention, wrong execution. A mistake is a wrong intention arising from a faulty mental model.

**5. b)** Competition for attention. The original wording is that every extra unit of information competes with the relevant units and diminishes their visibility — it is not a mandate for sparse visuals, and a dense professional tool can satisfy it.

**6. c)** Accessibility is not one of Nielsen's ten (it is arguably an omission of the set; Shneiderman's "universal usability" covers it, and it is treated properly in Module 10).

---

**7.** (1) Visibility of system status; (2) Match between system and the real world; (3) User control and freedom; (4) Consistency and standards; (5) Error prevention; (6) Recognition rather than recall; (7) Flexibility and efficiency of use; (8) Aesthetic and minimalist design; (9) Help users recognise, diagnose, and recover from errors; (10) Help and documentation.

**8.** Parts and violations:
1. **What happened**, in the user's terms — violated by "Error 0x8004."
2. **Why** — violated by "Something went wrong," which gives no cause and so no route to a fix.
3. **How to fix it**, specifically — violated by "Invalid input," which does not say what would be valid.
4. **A way out** — violated by an error with no retry, no contact route, and no link back to a working state.
Additional common violations: destroying entered data, marking errors with colour alone, blaming the user, and placing the message far from the field it concerns.

**9.**
1. *Will the user try to achieve the right effect?* → goal/expectation problem; fix with framing, entry-point context, or copy that sets the right goal.
2. *Will they notice the correct action is available?* → visibility/discoverability problem; fix with placement, contrast, and signifiers.
3. *Will they associate the correct action with the effect they want?* → labelling/mapping problem; fix with wording, icon+label, and grouping.
4. *If performed, will they see progress?* → feedback problem; fix with state changes, confirmation, and progress indication.
Mapping: 1–3 are the Gulf of Execution, 4 is the Gulf of Evaluation.

**10.** **Frequency** (how often it occurs), **impact** (how hard it is to overcome when it occurs), **persistence** (whether users learn around it or hit it every time).
Example where rare outranks frequent: a data-loss bug that hits 0.5% of sessions when the network drops mid-save is severity 4 because it is unrecoverable and destroys trust, while a misaligned label seen by 100% of users is severity 1. Impact and recoverability dominate frequency when the consequence is irreversible.

**11.** (a) Whether users actually want the feature or concept at all — inspection can only assess execution, not demand; (b) how real users with real goals, real data, and real distractions will actually behave, including domain misunderstandings that experts do not share. Related caveat: experts over-report cosmetic problems and under-report the ones only surfaced by genuine task context.

**12.** Violations:
- **#9 Help users recognise, diagnose, recover** — "Invalid input" gives no field, no cause, no fix. Severity 4.
- **#3 User control and freedom** — clearing entered card fields destroys the user's work; there is no way to recover it. Severity 4 (Tognazzini's "protect users' work").
- **#5 Error prevention** — validating only on submit misses the chance to prevent the error; constraints and formats were never communicated up front. Severity 3.
- **#1 Visibility of system status** — the user cannot tell *which* field is at fault. Severity 3.
- **#6 Recognition rather than recall** — after clearing, the user must recall what they entered. Severity 3.
- Likely **accessibility** violation too (Module 10): error identification by colour alone, and errors not programmatically associated with fields, so screen-reader users get no usable signal. Severity 4 in regulated contexts.
Fix: validate inline on blur; show constraints before entry ("16 digits"); preserve every entered value on failure; place a specific message adjacent to the offending field, with an icon and text as well as colour; move focus to the first failing field; keep a summary at the top that links to each error; make the messages field-specific ("This card number is 15 digits — Amex cards need 15, so check the card type") rather than generic.
Overall severity: catastrophic, because it blocks a revenue path and destroys user work.

**13.** Time allocation:
- **0–2 min — Frame.** State who the user is, the primary task, and the business goal, flagging these as assumptions.
- **2–5 min — Walk the happy path** as a first-time user, narrating what draws the eye and what you expect versus what happens.
- **5–12 min — Probe the edges:** empty, error, loading, long-content, offline, small screen, keyboard-only, contrast, target sizes. Most severe findings live here.
- **12–16 min — Categorise** by heuristic and rate severity 0–4.
- **16–19 min — Prioritise and propose:** top three with a specific fix each and the metric you would move.
- **19–20 min — State the limits:** what you would validate with users or data, and what you could not assess.
The skipped step is the last one — naming what you *cannot* conclude from an inspection, and what you would test. It converts a critique into a plan, and it is the clearest seniority signal in the round.

**14.** Six heuristics for an AI chat assistant (any reasonable set with rationales earns credit):
1. **Set capability expectations up front** — users cannot see the boundary of what the system can do, so the interface must signal scope or they will fail in ways they blame themselves for.
2. **Expose uncertainty and sources** — a fluent wrong answer is the dominant failure mode; confidence and provenance let users calibrate trust.
3. **Make correction and steering cheap** — the interaction is iterative, so editing the previous turn, retrying with changes, and adjusting tone or scope must be first-class, not a re-typed prompt.
4. **Show and bound the cost of mistakes** — before any action with side effects (sending, deleting, purchasing, running code), preview the action and require intent confirmation; irreversibility is the risk axis.
5. **Preserve user control over automation** — the user, not the system, initiates consequential actions; provide interruption (stop generation) and an escape to a deterministic path.
6. **Support memory and continuity legibly** — show what the system remembers about the user or session, and let them inspect, edit, and delete it.
Why Nielsen's set alone is insufficient: it assumes a deterministic system with a discoverable, finite set of controls and a visible state. A generative system has an open-ended input space (so discoverability is about *capability*, not controls), non-deterministic output (so "consistency" partially fails as a criterion), and failure modes — plausible fabrication, silent scope creep, unintended side effects — that no classical heuristic names. Nielsen's #1, #3, #5, and #9 still apply and remain valuable; they just do not cover trust calibration, provenance, or automation authority.
