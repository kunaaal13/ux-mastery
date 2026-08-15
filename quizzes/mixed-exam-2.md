# Mixed Exam 2 — Practice

30 questions drawing on Modules 07–13 (interaction design, information architecture, research, accessibility, design systems, metrics and strategy, advanced topics). Target: 22/30. Worked solutions below, with marking notes on what a strong versus weak answer contains.

---

### Part A — Recall

**1.** An affordance is:
- a) the visual cue that tells a user an action is possible
- b) a relationship between an object's properties and an actor's capabilities
- c) the label attached to a control
- d) the feedback returned after an action

**2.** Interface response to a tap should be acknowledged within approximately:
- a) 10 ms
- b) 100 ms
- c) 400 ms
- d) 1 s

**3.** Optimistic UI is the wrong choice for:
- a) marking a message as read
- b) liking a post
- c) submitting a payment
- d) reordering a playlist

**4.** A tree test measures success rate, time, first click, and:
- a) satisfaction
- b) directness
- c) findability rate
- d) scent strength

**5.** "Five users find 85% of problems" applies to:
- a) any research question with five participants
- b) usability problems in one homogeneous group, across iterative rounds
- c) surveys with five respondents per segment
- d) proportional claims about user preference

**6.** WCAG 1.4.3 Contrast (Minimum) requires:
- a) 3:1 for all text
- b) 4.5:1 for normal text, 3:1 for large text
- c) 7:1 for normal text, 4.5:1 for large text
- d) 4.5:1 for all text and UI components

**7.** WCAG 2.5.8 Target Size (Minimum) at AA specifies:
- a) 44×44 CSS px
- b) 48×48 CSS px
- c) 24×24 CSS px
- d) 32×32 CSS px

**8.** The first rule of ARIA is:
- a) always add a role to custom controls
- b) do not use ARIA if a native HTML element will do
- c) label every element with `aria-label`
- d) prefer `aria-live` over focus management

**9.** In a design system, components should consume:
- a) primitive tokens
- b) semantic tokens
- c) raw hex values
- d) component tokens only

**10.** In AARRR, the stage where design has the highest leverage is:
- a) Acquisition
- b) Activation
- c) Revenue
- d) Referral

**11.** The Fogg Behaviour Model states that behaviour occurs when:
- a) motivation exceeds a threshold
- b) motivation, ability, and a prompt converge at the same moment
- c) a trigger produces a variable reward
- d) friction falls below the cost of the action

**12.** Translating meaning and intent rather than words — recreating a message for a market — is:
- a) internationalisation
- b) localisation
- c) transcreation
- d) globalisation

---

### Part B — Short answer

**13.** Distinguish an affordance from a signifier, and explain why the distinction changes what you do when users cannot find a control.

**14.** Name the states in the state matrix, and say which two are most often missing from a design handoff.

**15.** Give the rule for choosing between a toast, an inline message, a banner, and a modal.

**16.** Rewrite this error message and state the principles you applied: "Error 4012: Invalid input."

**17.** State the difference between a card sort and a tree test in one sentence each, and say why neither substitutes for the other.

**18.** Explain what a high pogo-sticking rate and a high zero-result query rate each tell you, and what you would do about each.

**19.** Give four ways an A/B test can produce a result you should not act on.

**20.** State the practical WCAG conformance target, and explain why conformance is the floor rather than the goal.

**21.** Give the test for whether something belongs in a design system, and name the cost of promoting something too early.

**22.** Write the Goals → Signals → Metrics chain for a password-reset flow, and name one counter-metric.

---

### Part C — Applied

**23.** A checkout form has a single "Continue" button that turns red with the message "Please fix the errors below." Users abandon at 40%. Diagnose using interaction design principles and give the redesign.

**24.** A support site's navigation was designed by the content team around their internal departments. Search accounts for 70% of sessions and zero-result queries are rising. Give the full IA remediation plan.

**25.** A stakeholder says: "The A/B test shows the new upgrade prompt lifted conversion 12%. Ship it." The prompt is a full-screen interstitial with a small "Not now" link. Respond.

**26.** You inherit a product with no accessibility work done. You have two sprints. Prioritise, and justify the ordering.

**27.** A design system has 140 components, adoption is 30%, and teams keep building their own. Diagnose and give the recovery plan.

**28.** Engagement is up 20% after a redesign, but support contacts are up 15% and D30 retention is flat. Explain what may be happening and what you would investigate.

**29.** You are asked to design an AI assistant that answers questions from a company's internal documentation. Give the interaction design, naming the AI-specific heuristics.

**30.** A subscription product's cancellation flow currently requires a phone call during business hours. Legal says it is compliant in your main market. Give your position and the design you would propose.

---
---

## Solutions

**1. b)** An affordance is the *relationship* between an object's properties and an actor's capabilities — it exists whether or not it is perceivable. Option (a) is the signifier, which is the perceivable cue. The distinction matters because it separates "the action is impossible" from "the action is possible but invisible," and those have different fixes.

**2. b)** ~100 ms for acknowledgement — the perceptual threshold at which a response feels instantaneous and causally linked to the input. The 400 ms in option (c) is the Doherty Threshold for productive interaction; it is a different quantity and answering with it is the common confusion.

**3. c)** Payments. Optimistic UI is right for high-success, low-cost, easily reversed actions (a, b, d). When failure genuinely matters and reversal is confusing or has financial or legal consequence, pessimistic UI is correct — you must not tell the user something succeeded and then retract it.

**4. b)** Directness — whether the user reached the destination without backtracking. Low directness with high success means the structure is workable but a label is ambiguous. Findability rate (c) is a separate measure from a different study type.

**5. b)** Usability problems, one homogeneous group, iterative rounds. It does not license five-person proportional claims (d), does not tell you what to build, and requires five *per segment* when segments differ meaningfully.

**6. b)** 4.5:1 normal, 3:1 large. Option (c) is the AAA criterion 1.4.6; option (d) confuses text contrast with 1.4.11 Non-text Contrast, which is 3:1 for UI component boundaries and meaningful graphics.

**7. c)** 24×24 CSS px, added in WCAG 2.2 at AA, with exceptions for spacing and inline text. The 44×44 figure in (a) is Apple's platform guidance and is a good design target, but it is not the WCAG criterion — quoting it as WCAG is a common error.

**8. b)** Do not use ARIA if a native HTML element will do. Native semantics carry role, state, and keyboard behaviour for free; bad ARIA is worse than none, because it overrides what the browser would have reported correctly.

**9. b)** Semantic tokens — role-based names such as `color-text-primary`. Consuming primitives (a) couples components to raw values and makes theming, dark mode, and accessibility modes impossible without rewriting component code.

**10. b)** Activation — the moment a user first experiences core value. Acquisition is largely marketing's lever; revenue and referral both depend on activation having happened first.

**11. b)** B = MAP: motivation, ability, and prompt converging simultaneously. Option (c) describes the Hook Model's trigger–action–variable reward–investment loop, which is a related but distinct model.

**12. c)** Transcreation. Internationalisation is engineering the product so it *can* adapt (locale handling, RTL support, text expansion tolerance); localisation is adapting content and formats for a locale; transcreation recreates intent, and is what marketing copy and humour require.

---

**13.** An **affordance** is the relationship between an object's properties and the capabilities of the actor — a door affords pushing whether or not anyone realises it. A **signifier** is the perceivable cue that communicates where the action should happen: the plate, the label, the shadow under a button.

Why the distinction changes your action: when users cannot find a control, the affordance almost always exists (the button is there, it works) and the *signifier* has failed. So the fix is perceptual, not functional — increase the visual differentiation, add a label, restore a border or shadow, place it where scanning will find it. Teams that do not hold the distinction respond by adding more functionality or a tooltip, which does not address the failure. The inverse case also matters: a signifier that suggests an affordance which does not exist (an underlined non-link, a card that looks tappable but is not) is a false signifier, and it costs more trust than a missing one.
*Marking:* the strong answer states that affordances can exist unperceived and draws the diagnostic consequence. A weak answer defines the two terms correctly but stops there.

**14.** The full matrix: **empty first-use, empty after clearing, no results, loading, partial, populated, overflowing, error, offline, success, permission-denied.**

Most often missing from handoff: **overflowing** and **permission-denied**. Overflowing is missed because designers populate mocks with tidy sample data — realistic names, short titles, three items — so nobody sees what happens at 47 characters, 400 rows, or a name with no spaces. Permission-denied is missed because the designer works in an account with full access and never encounters the state; it then ships as either a blank screen or a raw 403, which reads as a broken product rather than a policy.

Runners-up worth naming: **partial** (some data loaded, some failed) and **empty after clearing**, which is different from empty first-use because the user knows what should be there and needs a different message — "no results for this filter, clear it" rather than an onboarding invitation.
*Marking:* naming the list is recall; the marks are in explaining *why* those two get missed, which shows you understand the mechanism (designers test in their own conditions) rather than having memorised a checklist.

**15.** Choose by **severity and required action**, on two axes: does the user need to act, and can the message be missed?

- **Toast** — transient, dismissible, no action required, low consequence. "Copied to clipboard." Never for anything the user must read, because it disappears and is often outside the locus of attention.
- **Inline** — attached to the element it concerns. Correct for validation and field-level errors, because the message must be adjacent to the thing being fixed. This is the default for form errors.
- **Banner** — persistent, page or section scope, informs about a condition the user should know but need not resolve immediately. "You are offline; changes will sync when you reconnect."
- **Modal** — only when the user must decide before continuing *and* the decision cannot be deferred. Modals block, they break keyboard and screen-reader flow if built carelessly, and they train a dismissal reflex, so each one must justify its existence.

Cross-cutting rule: feedback should be **proportional** to the action (Shneiderman) and **near the locus of attention**. A toast in the opposite corner from the click is routinely missed through change blindness — which is why a successful destructive action often needs an inline or banner confirmation, not a toast.
*Marking:* a strong answer gives a decision rule and names the modal test explicitly. Listing the four patterns with descriptions and no selection criterion is a half answer.

**16.** Rewrite: **"Enter your date of birth as DD/MM/YYYY — for example, 14/03/1988."** — placed inline, next to the field, with the field visibly marked and focus moved to it.

Principles applied:
- **Say what is wrong specifically**, not that something is wrong. "Invalid input" fails because the user cannot act on it.
- **Say which element**, and place the message next to that element (locus of attention; WCAG 3.3.1 Error Identification).
- **Say how to fix it** — WCAG 3.3.3 Error Suggestion. An example is more effective than a format description, because it is recognition rather than interpretation.
- **Remove the error code from the primary message.** A code helps support, not the user; keep it, but subordinate it or attach it to the support path.
- **Do not blame the user.** "Invalid" implies fault; the format was never shown. Better still, prevent the error — accept multiple formats and normalise, which is Postel's Law applied to input.
- **Announce it to assistive technology** without stealing focus unexpectedly (WCAG 4.1.3 Status Messages), or move focus deliberately to the first field in error.

Trade-off: highly specific messages take more copy and more engineering branches. The honest position is that error-message specificity earns its cost at the points where abandonment is expensive — checkout, sign-up, submission — and generic messages are tolerable in low-stakes internal tooling.
*Marking:* the strongest answers reach the **prevention** point — the best error message is the one never shown, because the format was accepted or the constraint communicated up front.

**17.** **Card sort:** participants group and name content items, telling you their mental model and vocabulary — generative, used to *design* a structure. **Tree test:** participants perform find-it tasks against a text-only hierarchy, telling you whether people can locate things in a structure you propose — evaluative, used to *verify* it.

Neither substitutes for the other because they answer different questions. A card sort can produce a structure that matches how users would organise the content and still fails on findability, because grouping in the abstract is a different cognitive task from searching under a goal — users sorting cards see all items at once, while users navigating see only labels and must infer scent. Conversely a tree test tells you a structure fails but not what to replace it with, because it never elicits the user's own categories or words. The productive sequence runs sort → draft two or three candidate structures → tree test each → refine labels → re-test the weakest tasks.

Practical parameters worth stating: card sorts want 15–30 participants and 30–60 items (more causes fatigue); tree tests want 30–50 per structure.

**18.** **Pogo-sticking** — repeated in-and-out movement between a list and its items — indicates weak **information scent**: the list is not carrying enough information for the user to judge which item is right, so they must open each one to find out. Fixes are informational rather than structural: enrich the list with the attributes people are actually discriminating on (price, date, status, a snippet, a thumbnail), improve the labels, and consider a preview so evaluation does not require navigation. It is a strong signal precisely because it is behavioural — users are demonstrating a failed prediction, repeatedly.

**Zero-result queries** are a direct, free list of **vocabulary and content gaps**. Two distinct causes hide inside the same number: content that does not exist (a gap in the product or documentation), and content that exists under a different word (a synonym gap). Sort the log by frequency and separate the two. Synonym gaps are cheap to fix — add synonym mappings and rename where the user's word is genuinely better than yours. Content gaps are a roadmap input. Either way, no query should return a bare "no results": show near matches, popular content, and a route to a human.

Both are continuous and free, which is the wider point — search logs, zero-result queries, and support-ticket topics give you IA evidence every day without recruiting anyone.
*Marking:* separating the two causes of zero-result queries is what distinguishes a strong answer; "add synonyms" alone misses that half of them are a content problem.

**19.** Any four of:

- **Underpowered.** No power calculation from baseline rate, minimum detectable effect, and desired power, so the "result" is noise that happens to look like signal.
- **Peeking.** Stopping when the numbers look good massively inflates the false-positive rate; the duration must be pre-committed and run at least one full weekly cycle to cover day-of-week variation.
- **Novelty or primacy effects.** A change can win temporarily because it is new, or lose temporarily because it is unfamiliar (change aversion). Neither is the steady-state effect you are trying to measure.
- **Multiple comparisons.** Testing twenty metrics essentially guarantees one "significant" result by chance. Declare one primary metric in advance.
- **Significance mistaken for importance.** With enough traffic a 0.1% lift is statistically significant and commercially worthless. Report effect size and confidence interval, not a p-value alone.
- **Guardrails ignored.** The primary metric moved by degrading something else — latency, error rate, support contacts, refunds, revenue per user.
- **Post-hoc segmentation.** A segment finding discovered after the fact is a hypothesis for the next test, not a conclusion.
- **Wrong question for the method.** Long-horizon effects (trust, brand, months-long retention) and high-risk irreversible changes are not testable this way at all.

**20.** The practical target is **AA of WCAG 2.1 or 2.2** — it is the level that regulation, procurement, and EN 301 549 generally reference. A is the minimum and failing it blocks whole populations; AAA is not realistic across an entire product, though individual AAA criteria are worth adopting selectively, such as 7:1 contrast for long-form reading.

Conformance is the floor because the success criteria are **testable propositions about artefacts, not about experience**. A product can satisfy every criterion and still be miserable with a screen reader: the reading order can be technically correct and narratively incoherent, every control can have an accessible name while the names are all "button," the focus indicator can be visible and still invisible against the actual background it lands on, and the whole flow can be operable while taking four times as long as it should. Criteria are per-element and mostly per-page; experience is per-journey.

So the practice is: audit for conformance to catch the mechanical failures cheaply, then **test the real flows** with keyboard only and with a screen reader, and ideally with disabled users, because that is the only thing that surfaces the journey-level failures.
*Marking:* the marks are in the floor-versus-goal argument with a concrete example of passing-but-unusable. Naming "AA" and stopping is recall, not judgement.

**21.** The test is **repetition plus stability**: something used in three or more places, whose behaviour has settled, belongs in the system. Something used once, or still changing weekly, belongs in the product code until it settles.

The cost of promoting too early is **churn multiplied by the number of consumers**. Once a component is in the system, every subsequent change is a coordinated migration: a breaking change requires a major version, a changelog, a migration path, and time from every consuming team. A pattern that is still being figured out will change three or four times, and each change is now expensive rather than free. Worse, the second-order effect is reputational — teams that get burned by unstable system components stop trusting the system, and an untrusted system produces *less* consistency than no system at all, because people fork it and diverge silently.

The counter-trade-off is real and worth naming: promote too late and you get duplicated, divergent implementations that are expensive to consolidate, and the accessibility work gets redone badly in each one. The resolution is usually a staging concept — a labelled "candidate" or "lab" tier with an explicit no-stability promise — so early adopters can use it while nobody assumes a contract.

**22. Goal:** a user who has lost access regains it quickly and unaided, without contacting support.

**Signals:** users who begin a reset complete it; they complete it in one attempt; they do not contact support about access; they do not immediately reset again (which would indicate the new password did not stick or they never understood what happened); they successfully sign in afterwards.

**Metrics:**
- Reset completion rate (started → successfully signed in with the new credential) — primary.
- Median time from request to successful sign-in.
- Repeat-reset rate within 7 days.
- Password-reset support contacts per 1,000 reset attempts.
- Step-level drop-off, particularly at the email/OTP step.

**Counter-metric:** account-takeover rate, or fraudulent-reset reports. The cheap way to move completion up is to weaken verification, which is a security regression disguised as a UX win. A second useful guardrail is deliverability — reset emails landing in spam show up as a completion drop that has nothing to do with design.
*Marking:* a strong answer defines completion as "signed in successfully," not "submitted the form," and names the security counter-metric unprompted. Listing metrics without the goal-and-signal chain misses the point of GSM.

**23.** **Diagnosis.**

- **The error message is not where the error is.** A single summary at the button violates the locus-of-attention principle and WCAG 3.3.1: the user is told errors exist but must hunt for them. On a long form, some errors are below the fold entirely.
- **No error identification per field.** "Please fix the errors below" names neither the field nor the problem, so it cannot be acted on.
- **Colour is doing the work alone.** A red button and red fields fail 1.4.1 Use of Color; users with colour-vision deficiency, in bright sunlight, or on a poor screen get nothing.
- **Validation timing is almost certainly wrong.** Errors surfacing only on submit means the user completed the whole form before learning anything was wrong — the most expensive possible moment to be told.
- **Constraints were never communicated.** Format requirements (password rules, phone format, card acceptance) were not shown before the attempt, so the error is the first time the rule appears.
- **The state after error is unclear.** If the form re-renders and loses data, or scroll position resets, abandonment follows immediately.
- **Focus is not managed.** Keyboard and screen-reader users are left at the button with no way to know what changed (4.1.3 Status Messages).

**Redesign.**

1. **Inline validation on blur, not on keystroke**, for fields with a checkable format; validate on keystroke only to *remove* an error already shown, so the user is never scolded mid-typing.
2. **Field-level messages** stating the specific problem and the fix, with an example. Marked with an icon and text, not colour alone.
3. **On submit**, if errors remain: an error summary at the top listing each error as a link to its field, move focus to the summary, and announce it. Keep the inline messages as well — the summary is for orientation, the inline message is for repair.
4. **Communicate constraints up front** — password rules visible before typing, accepted card brands shown, format hints in helper text rather than placeholders (placeholders vanish and fail as labels).
5. **Never lose entered data**, and preserve scroll position.
6. **Prevent where possible**: accept and normalise multiple formats for phone numbers, card numbers, and dates rather than rejecting them; allow paste everywhere, which 3.3.8 Accessible Authentication requires for one-time codes.
7. **Reduce the surface**: audit whether every field is genuinely required at this step; the cheapest error is the field you removed.

**Verification.** Instrument field-level error rates and abandonment by step, then re-measure completion with error rate as a paired diagnostic — completion up with error rate flat would suggest you merely made the form shorter, which may or may not be what you wanted.
*Marking:* strong answers get to prevention and to focus management; weak answers say "add inline validation" and stop. Naming the summary-plus-inline combination, rather than treating them as alternatives, is a senior signal.

**24.** **The core diagnosis:** the navigation encodes the organisation's structure rather than users' tasks and vocabulary — a classic Conway's-law IA. Search at 70% of sessions is not inherently a failure (large catalogues legitimately skew to search), but rising zero-result queries alongside it says the vocabulary gap is real and widening: people are searching *because* navigation failed, and then failing at search too.

**Plan, in order.**

1. **Content inventory and analytics baseline.** Enumerate every article: URL, owner, traffic, last updated, deflection rate, purpose. This is boring and the highest-leverage first step, because it almost always reveals that a large share of content has near-zero traffic — which changes the problem from "organise all of it" to "retire most of it."
2. **Harvest the users' vocabulary for free.** Search logs (especially zero-result and low-click queries), support-ticket subject lines, and community posts. This is the raw material for labelling and costs nothing.
3. **Separate the two failure modes in search.** Missing content versus synonym gaps, as above. Fix synonyms immediately — it is a same-week win that reduces the pressure while the restructure runs.
4. **Define a content model** before a taxonomy: what *types* of content exist (troubleshooting, how-to, reference, policy, release note), what attributes each has (product, platform, plan tier, severity), and how they relate. This is what makes the IA scale and it is the artefact engineering most needs from you.
5. **Open card sort, 15–30 participants, 30–60 items.** Open rather than closed, because the existing categories are the thing under suspicion and the names participants invent are as valuable as the groupings. Run a handful moderated to hear the reasoning.
6. **Draft two or three candidate structures**, deliberately different in shape — one broader and shallower, one organised by task, one by product area — rather than three variations of the same idea.
7. **Tree test each, 30–50 users per structure**, on the tasks that generate the most support volume. Read directness as well as success: high success with low directness means the structure works and a label is ambiguous, which is a cheap fix.
8. **Refine labels and re-test the weakest tasks.** Prefer users' words over internal ones, and drop the department names entirely — they are meaningless to the person with the problem.
9. **First-click test on the designed pages**, since a correct first click strongly predicts eventual success.
10. **Ship with redirects for every changed URL**, and consider polyhierarchy where an item genuinely belongs in two places — cross-linking is cheaper than forcing a false single home.
11. **Monitor**: findability rate, search-versus-navigate ratio, zero-result rate, pogo-sticking, and support volume by topic. Expect a short-term dip from change aversion in returning users, and segment new versus returning so you do not misread it.

**Trade-off to state:** restructuring breaks the muscle memory of frequent users and any external links, and it is expensive. If the inventory shows the real problem is content quality and coverage rather than organisation, the restructure is the wrong project — say so before spending the quarter.

**25.** Model response — accept the number, contest the conclusion.

**First, validate the test.** Was a power calculation done in advance, was the duration pre-committed, did it run at least one full weekly cycle, was there peeking, and was conversion the single pre-declared primary metric? A 12% lift from an underpowered or peeked test is not a 12% lift.

**Second, ask what "conversion" counted.** An interstitial reliably lifts the click that immediately follows it. The question is whether it lifted *paid, retained* upgrades. I would want the downstream figures: completed payments, refund and chargeback rate, cancellation within the first billing cycle, and D30 retention of the cohort that upgraded through the prompt. A prompt that converts people who did not intend to buy shows up later as refunds and churn, and by then nobody attributes it to the prompt.

**Third, check the guardrails.** Support contacts, app-store and review sentiment, session frequency for users who saw it and did not convert, and — importantly — the behaviour of the *non-converting majority*, who are the large group whose experience just got worse. Ninety-something percent of exposed users paid the interruption cost and gained nothing.

**Fourth, name the pattern honestly.** A full-screen interstitial with a visually subordinate "Not now" is **confirmshaming's quieter cousin — interface interference through false hierarchy**: the decline option is available but deliberately harder to see and hit. That is a recognised dark-pattern category, it is increasingly a regulatory exposure rather than only an ethical one, and it is exactly the kind of thing that reads badly in a screenshot on social media.

**Fifth, the ethical test, stated as a decision rule rather than a sentiment:** would we describe this mechanism to the user in plain language and still be comfortable? "We made the decline link small so more people would miss it" fails that test. Would the user, understanding it fully, still consent?

**What I would propose instead.** Keep the goal — I am not arguing against prompting for upgrade. Run a second test against a non-blocking, well-targeted variant: an inline prompt at a moment where the user has just hit the limit the paid tier removes, with equal visual weight on both options. That tests *targeting and timing* rather than *interruption and asymmetry*. Declare completed-and-retained upgrade as the primary metric with refund rate and D30 retention as guardrails, and give it a full cycle. If the honest variant gets most of the lift, we have the outcome without the exposure. If the interstitial genuinely wins on retained revenue, that is a real business decision to make with the trade-off visible — but I would still fix the button asymmetry, because that part is not what is producing the lift, it is only what makes it indefensible.
*Marking:* the strong answer does three things — audits test validity, separates the proxy metric from the outcome metric, and names the dark-pattern category with a usable ethical test — while keeping the stakeholder's goal alive and proposing a measurable alternative. Refusing on ethical grounds alone, or accepting the number at face value, are both weak.

**26.** **Prioritisation principle:** order by **damage × population blocked**, and prefer fixes that are systemic (fix once, apply everywhere) over per-screen remediation. In two sprints you cannot reach conformance, so the goal is to remove the failures that *block* people entirely and to stop new failures being created.

**Sprint 1 — unblock.**

1. **Keyboard operability of the primary flows.** Walk sign-in, the core task, and checkout with the keyboard only. Anything unreachable or trapped (2.1.1, 2.1.2) is a total block for a large population, including many people who do not identify as disabled. This is the single highest-damage class.
2. **Focus visibility (2.4.7).** Restore a visible focus indicator everywhere it was removed, with sufficient contrast against the surfaces it lands on. Removing outlines without a replacement is the most common and most damaging single failure, and it is usually a one-line systemic fix.
3. **Form labels and error identification (3.3.2, 3.3.1, 1.3.1).** Every input gets a programmatically associated visible label; every error is described in text and associated with its field. Placeholder-as-label must go.
4. **Images and icon-only controls (1.1.1, 4.1.2).** Accessible names on every icon button; empty alt on decorative images; real descriptions on informative ones.
5. **Text contrast (1.4.3) and non-text contrast (1.4.11)** in the token layer rather than screen by screen — fixing the semantic tokens fixes every consumer at once.

**Sprint 2 — consolidate and prevent.**

6. **Custom controls: name, role, value (4.1.2)** — the bespoke dropdown, tabs, and modal. Replace with native elements where possible (first rule of ARIA) rather than layering ARIA onto divs.
7. **Status messages (4.1.3)** so async results and validation are announced without stealing focus.
8. **Zoom and reflow (1.4.4, 1.4.10)** — 200% zoom and 320 CSS px width without two-dimensional scrolling.
9. **Accessible authentication (3.3.8)** — allow paste in OTP and password fields. Small change, disproportionate impact.
10. **Prevention, which is the part that makes it stick:** fix the shared components rather than the screens, add automated checks (axe or equivalent) to CI, add an accessibility section to the definition of done, and write the acceptance criteria into the component documentation.

**Explicitly deferred and stated as such:** full audit and VPAT, AAA criteria, complex data-table semantics, and video captions if there is no video in the core flow. I would document these as known gaps with owners rather than leave them unnamed.

**Trade-off:** automated tooling catches perhaps a third of issues and none of the journey-level ones, so I would spend part of sprint 2 on a keyboard-and-screen-reader run of the real end-to-end flows, and budget for testing with disabled users after the two sprints — that is where the findings that matter most tend to come from, and it is the thing most likely to be cut.
*Marking:* the ordering must be justified by damage and population, not by ease. A strong answer includes the prevention step and names what it is deliberately *not* doing; a weak one lists WCAG criteria in numeric order.

**27.** **Diagnosis.** 140 components with 30% adoption is a supply problem masquerading as a demand problem. The likely causes, in the order I would check them:

- **Breadth over reliability.** A hundred half-right components is worse than thirty everyone trusts. Once a team is burned by a component that lacked a state, was inaccessible, or broke on upgrade, they stop reaching for the system at all — and the cost of an unreliable system is *worse* consistency than before it existed.
- **Patterns are missing.** Systems that neglect the pattern layer — forms, empty states, error handling, page templates, tables, filtering — hand teams components and no answers to the actual composition problems they face. Teams then build the composition themselves, and the component divergence follows.
- **Configurable rather than composable.** Twenty boolean props on a component is a smell; when the flags do not cover a case, teams fork rather than compose.
- **No escape hatch.** If the system offers no sanctioned way to do something it does not cover, every gap becomes a silent fork. A documented escape hatch keeps deviation visible.
- **Contribution is closed or slow.** If a team's only route is to file a request and wait a quarter, building their own is the rational choice.
- **Design–code parity has drifted**, so using the system requires reconciling two sources of truth.
- **Adoption was never measured properly**, so nobody knows *which* 70% is missing or why — 30% could be one team at 90% and five at zero, which is a completely different problem from uniform partial adoption.

**Recovery plan.**

1. **Measure adoption properly first.** Instrument component usage in code, per team and per surface, and audit production screens against the library. Get the distribution, not the average. Interview the teams with the lowest adoption — the reason is usually specific and fixable, and asking is faster than guessing.
2. **Freeze new components.** No additions until the existing set is trustworthy. This is unpopular and necessary.
3. **Triage the 140 into keep / merge / deprecate**, using real usage data. Expect a large tail with one or zero consumers. Consolidate duplicates, deprecate the tail on a published timeline with codemods or migration notes where possible.
4. **Harden the core twenty.** Complete states (including focus, error, loading, disabled, empty), accessibility by default, content guidance, and a "when not to use" section — that section prevents more misuse than any amount of documentation elsewhere. Accessible-by-default is the biggest single multiplier the system offers, and it is the strongest argument for adoption you have.
5. **Ship the missing patterns**, prioritised by what teams are actually rebuilding — usually forms, tables, and empty states.
6. **Open the contribution loop** with a published path, a service-level expectation on review, and a named owner. Federate: let the highest-need teams contribute rather than queue.
7. **Publish an escape hatch** — a sanctioned way to deviate, with a lightweight record of why. Deviation you can see is a roadmap input; deviation you cannot see is drift.
8. **Semantic versioning with real changelogs and migration guides**, and batch breaking changes rather than dripping them, because the cost is borne by every consumer each time.
9. **Re-measure adoption quarterly** against the distribution, and treat a team's adoption falling as a signal to go and ask why rather than to escalate.

**Trade-off to state:** deprecating components has a real cost for the teams using them, and a freeze slows delivery for anyone waiting on a genuinely new need. The judgement is that trust is the binding constraint here, and trust is rebuilt by reliability and responsiveness, not by inventory.
*Marking:* the key insight is that adoption is a trust and service problem, not a coverage problem — the instinct to fix low adoption by building more components is exactly wrong. A strong answer also insists on getting the distribution before acting.

**28.** **The most likely reading:** engagement rose because the product became *harder*, not more valuable. More sessions, more actions per session, and more time in task are all consistent with users failing and retrying — which is why engagement is the most misused HEART dimension, and why "more time in the product" is a failure signal for anything task-oriented. Support contacts up 15% corroborates that reading directly. Flat D30 retention says whatever changed did not alter durable value in either direction, which argues against the optimistic interpretation that people are engaging more because they like it more.

**Alternative explanations I would rule in or out before concluding:**

- **Novelty.** A redesign produces exploratory behaviour that decays. Check whether the engagement lift is decaying week over week and whether it concentrates in the first sessions after exposure.
- **Composition change.** If acquisition or a campaign changed at the same time, the population changed, not the behaviour. Cohort by join week and compare like with like.
- **Instrumentation change.** Redesigns routinely renumber or duplicate events. Verify the event definitions did not change before believing any of the numbers — this is the most common preventable cause of a mystery metric move.
- **Segment concentration.** Averages conceal everything. A 20% average lift can be one segment on one platform doubling while everyone else declines.
- **Retention lag.** D30 for the post-launch cohort may not have matured; make sure you are comparing complete cohorts.

**Investigation, in order:**

1. Verify instrumentation and cohort definitions. Nothing else is worth doing until this is clean.
2. Segment engagement by platform, tenure, and entry point; split new versus returning users, since change aversion affects only the latter.
3. Read the support contacts by topic — this is the cheapest available qualitative data and it will usually name the mechanism within an hour.
4. Look at task-level metrics rather than volume metrics: completion rate, error rate, time on task, retries, and SEQ. If completion fell while sessions rose, the diagnosis is settled.
5. Watch session recordings filtered to the new flow for rage clicks, dead clicks, and repeated back-navigation — hypothesis-generating, not proof.
6. Run five to eight moderated usability sessions on the changed flow with the tasks the support tickets describe.
7. Check funnel step conversion before and after, and the guardrails that should have been declared at launch.

**The underlying lesson worth stating:** engagement should have been paired with a counter-metric — task success or support contacts per active user — before launch, and the primary metric should have been tied to the goal in user terms via GSM. If the team cannot say what a *bad* outcome would have looked like in the numbers, the measurement plan was reporting rather than measurement.
*Marking:* a strong answer treats "engagement up" as ambiguous by default and reaches for task success and instrumentation validity before interpreting. A weak answer picks one story and defends it.

**29.** **Frame first.** The product is retrieval over a fixed, owned corpus, and the failure mode that matters is a confident wrong answer about a policy or procedure — the cost of a mistake is borne by an employee who acts on it. So the design should optimise for verifiability and correction, not for conversational fluency.

**Applying the AI interface heuristics.**

- **Set expectations of capability up front.** State what the assistant knows — which spaces, which documents, how recently indexed — in the empty first-use state, not in a help page. The single largest source of dissatisfaction with these systems is a mismatch between assumed and actual scope, and users cannot calibrate a black box by trial.
- **Show sources, inline and specific.** Every claim carries a citation to the document and section, linked, with the last-updated date. This is the primary trust mechanism and it converts an unverifiable assertion into a checkable one. Document recency matters especially in an internal corpus, where stale policy pages are common.
- **Expose uncertainty honestly.** Distinguish "answered from a strong match", "assembled from partial matches", and "not found". A visible "I could not find this in the documentation" is a *feature*, and the design must make that path attractive rather than embarrassing — otherwise the system is incentivised toward fabrication.
- **Allow correction and steering.** Editable prompts, follow-up refinement, scope filters (space, product, date range), and the ability to say "not this document, the other one." The user usually knows something about where the answer lives; let them contribute it.
- **Make the cost of a mistake visible and proportionate.** For consequential categories — security, HR, legal, finance, anything with a compliance consequence — route to the canonical document and a human owner rather than paraphrasing, and label those answers differently.
- **Offer a deterministic fallback.** Keyword search over the same corpus, always one click away. When the assistant fails, the user must not be stranded; and for many queries — finding a document they already know exists — search is simply the better tool.

**Interaction and state design.**

- **Empty first-use** carries the capability statement plus three or four example queries that demonstrate the *shape* of good questions, since discoverability of capability is the hardest problem in a text box.
- **Loading**: stream tokens so acknowledgement is immediate (well inside the 100 ms perceptual threshold for *something* happening), and show retrieval progress separately from generation — "searching 4 spaces… reading 6 documents…" — because a long silent wait reads as a hang and staged, truthful progress makes the wait legible.
- **No results / not found** is a first-class state with next actions: broaden scope, switch to keyword search, ask the owning team, request the document be written.
- **Error and offline** states must distinguish "the model failed" from "retrieval failed" from "you lack permission for the only document that answers this."
- **Permission-denied** is critical in an internal tool and routinely forgotten: the assistant must never leak content from documents the user cannot open, and when it withholds, it should say that a restricted document exists and who owns it — that is useful and safe.
- **Feedback affordances** on every answer, scoped usefully — "wrong", "outdated", "missing source" — because generic thumbs give you a number and no mechanism.

**Ethics and second-order effects worth naming unprompted:** an assistant that answers well reduces the incentive to keep documentation good, so instrument which documents are being cited and surface the gaps to their owners — otherwise the corpus rots while satisfaction stays high, and the system degrades quietly. Also consider what the query log reveals about individuals, and set a retention policy before launch rather than after someone asks.

**Measurement:** self-reported answer usefulness at the point of answer, citation click-through as a verification signal, deflection of support and internal help-desk tickets, and the not-found rate as a content-gap tracker — with a guardrail on *incorrect answers acted upon*, gathered from spot audits rather than user reports, since users rarely report a confident wrong answer they believed.
*Marking:* the strong answer treats sources, uncertainty, and the deterministic fallback as core rather than decorative, names permission-denied for an internal corpus, and reaches the second-order documentation-rot effect. A weak answer designs a chat window and a thumbs-up.

**30.** **Position.** Compliance in one market is the floor, not the argument. I would push to change it, and I would make the case on risk and revenue rather than on ethics alone — though the ethical case is also plain.

**Why it is a dark pattern.** Requiring a phone call during business hours to cancel something bought in two clicks online is **asymmetry between entry and exit** — one of the clearest members of the obstruction family, sometimes called a roach motel. The mechanism works by imposing a cost the user did not agree to when signing up, and it functions precisely *because* some people give up. Any mechanism whose business value depends on users failing to complete an action they intend to complete is not a design decision, it is an extraction.

**Why the compliance answer is weak.**
- **It is market-specific and moving.** Cancellation symmetry has been the direction of travel in consumer regulation across multiple jurisdictions; several already require that a subscription be cancellable by the same means it was purchased. If the product operates in more than one market, "compliant here" is a narrow claim, and building the capability under enforcement pressure costs more than building it now.
- **The revenue is worse than it looks.** Retention purchased by obstruction shows up as chargebacks, card cancellations, negative reviews, and elevated support cost per cancellation. It also poisons win-back: someone who escaped after a fight does not return, and tells people.
- **It corrupts the metrics.** Churn suppressed by friction hides the real product problem. Nobody can tell whether the product is delivering value, because the exit is blocked — you lose the most honest signal you have.

**The ethical test, stated usably:** would we show the user the mechanism and our reason for it in plain language and still be comfortable? "You must call during business hours because some of you will not manage it" fails immediately.

**What I would propose.**

1. **Cancel online, in the same number of steps as signing up**, from account settings, findable by search, with no login-only-on-desktop restriction.
2. **A single, honest retention offer** — one screen, one alternative (pause, downgrade, a discount if that is the genuine offer), with "continue cancelling" at equal visual weight. One offer is legitimate; a chain of them is obstruction by another name.
3. **Offer pause explicitly.** A meaningful share of cancellations are situational — cost this month, a break, a project ending. Pause converts a permanent loss into a temporary one and is honest, because it serves a want the user actually has.
4. **Confirm clearly**: the end date, what happens to their data, whether access continues to period end, and what re-subscribing would cost. Then send it in writing.
5. **Ask why, optionally, after the cancellation is already complete** — never as a gate. Answers given after the decision is irreversible are far more honest, and this becomes the best churn-diagnosis data the company has.
6. **Make the data-and-access consequences reversible for a window**, so a mistaken cancellation is recoverable.

**How I would argue it internally.** Propose it as a measured change, not a moral position: ship it, and track voluntary cancellation rate alongside chargebacks, support cost per cancellation, review sentiment, pause uptake, and win-back rate at 90 days. My expectation is that headline cancellations rise, chargebacks and support cost fall, and pause absorbs a meaningful fraction — but the honest framing is that gross cancellations will probably rise and someone must be willing to accept that. Separate **voluntary churn from involuntary churn** in the same work, because failed payments are often a larger and much cheaper problem to fix, and fixing it funds the argument.

**If overruled:** I would record the decision and my recommendation in writing, ask for a review date, and make sure the cancellation path that does exist is at least honest — accurate hours, accurate wait times, no misdirection about what calling will achieve. Documenting the disagreement is not theatre; it is what makes the decision reviewable when the regulation or the reviews arrive.
*Marking:* the strong answer names the specific dark-pattern category, refuses to rest on either compliance or ethics alone, proposes a measurable alternative that keeps the business goal alive, and states plainly that gross cancellations will likely rise. A weak answer either capitulates to legal or delivers a lecture with no design in it.

---

<!-- nav -->
[← Previous: Mixed Exam 1 — Foundations](mixed-exam-1.md) · [↑ Quizzes](README.md) · [Next: Final Exam — All 13 Modules →](final-exam.md)
