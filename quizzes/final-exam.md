# Final Exam — All 13 Modules

40 questions across the whole curriculum, weighted toward applied scenarios. Allow roughly 2.5 hours if you write the answers out in full.

**Conditions.** Closed book. Do not open the module files, the cheat sheet, or the per-module quizzes until you have finished. Where a question asks for a critique, a diagnosis, or a response to a colleague, answer it **aloud** first and then write it down — the spoken version is the one an interview will actually test, and the gap between what you can recognise and what you can say is the thing this exam is measuring.

Parts A and B are worth one mark each. Each applied scenario in Part C is worth one mark, awarded only if you addressed every lettered sub-part with a named mechanism and a specific action; a partial answer scores zero, because a partial answer is what a weak interview sounds like.

A scoring band interpretation and a "map your misses" table sit at the end. Do not read them first.

---

### Part A — Recall

**1.** ISO 9241-210 defines user experience as a person's perceptions and responses resulting from the use or *anticipated* use of a system. The significance of "anticipated" is that:
- a) users should be surveyed before launch
- b) expectation formed before use is part of the experience, so marketing and pricing are UX surface
- c) anticipation is a synonym for desirability
- d) the definition covers only interactive software

**2.** Which of these is NOT a pre-attentive attribute?
- a) hue
- b) size
- c) alphanumeric meaning
- d) orientation

**3.** Hick's Law describes decision time as a function of the number of equally probable options. The relationship is:
- a) linear, so halving the options halves the time
- b) logarithmic, so each added option costs less than the last
- c) exponential, so options must be aggressively pruned
- d) constant above five options

**4.** Two elements are enclosed by a card boundary; a third sits nearer to one of them but outside the card. Users will perceive:
- a) the two nearest elements as a group, because proximity is the strongest cue
- b) the two elements inside the card as a group, because common region beats proximity
- c) all three as one group, because closure completes the boundary
- d) no grouping, because the cues conflict

**5.** Which of Nielsen's ten heuristics is violated by a delete action that offers no undo and no confirmation?
- a) Match between system and the real world
- b) User control and freedom
- c) Recognition rather than recall
- d) Aesthetic and minimalist design

**6.** WCAG 2.1 AA requires a contrast ratio of at least 3:1 for:
- a) all body text
- b) large text and the boundaries of UI components
- c) decorative graphics
- d) focus indicators only

**7.** In a design system, components should consume:
- a) primitive tokens, because they are the source of truth
- b) semantic tokens, because they express role and survive theming
- c) raw hex values, for performance
- d) component tokens exclusively, to avoid coupling

**8.** A card sort tells you how users group and name things. To find out whether users can *locate* an item in a structure you propose, you run:
- a) a second, closed card sort
- b) a tree test
- c) a heuristic evaluation
- d) a diary study

**9.** In the AARRR funnel, the stage where design has the highest leverage — and the one most connected to onboarding work — is:
- a) acquisition
- b) activation
- c) revenue
- d) referral

**10.** In the Fogg Behaviour Model, B = MAP, a behaviour fails to occur when:
- a) motivation is low, regardless of the other factors
- b) any one of motivation, ability, or prompt is absent at the moment of the prompt
- c) ability is high but motivation is also high
- d) the prompt arrives before motivation has been established

---

### Part B — Short answer

**11.** Give the three models present in any product, and state which one the designer is responsible for.

**12.** State precisely what the claim "five users find 85% of usability problems" does and does not license.

**13.** Explain why "menus should have 7±2 items" misuses Miller's Law, and name one place the law genuinely applies.

**14.** A team removes focus outlines because "they look ugly." Name the success criterion violated, the population harmed, and the correct fix.

**15.** Distinguish an affordance from a signifier in one sentence each, and give an interface example where the affordance exists but the signifier is missing.

**16.** Give the rough ordering of Gestalt grouping strength among uniform connectedness, common region, proximity, and similarity, and say why the ordering is practically useful.

**17.** Write the Goals → Signals → Metrics chain for a password-reset flow.

**18.** Name three sources of extraneous cognitive load, each with a specific fix.

**19.** Explain the say-do gap and state the rule it implies when attitudinal and behavioural data are both available.

**20.** When is optimistic UI the right choice, and when is it actively harmful? Give the deciding question.

**21.** Give the three tiers of design tokens with an example of each, and say why the middle tier exists.

**22.** Name four states from the state matrix that teams most often forget, and say what each one costs when it is missing.

**23.** State the difference between localisation and internationalisation, and give one thing that breaks if you skip the second.

**24.** Give a usable one-sentence test that separates ethical persuasion from a dark pattern, and name one dark pattern category that now carries regulatory exposure.

---

### Part C — Applied scenarios

**25.** A B2B analytics product has a dashboard with fourteen metric tiles, all the same size, all with a coloured sparkline, and four buttons in the header styled as filled primaries: Export, Share, Schedule, and Configure. Users in testing say "I don't know where to look" and "I can never find Export."
(a) Diagnose the problem using named perceptual mechanisms.
(b) Give your changes in priority order.
(c) How would you verify the fix before shipping it?

**26.** A checkout has a payment authorisation step that takes six seconds. Users tap "Pay" repeatedly; a small number are charged twice.
(a) Name the laws and principles in play.
(b) Give the design fixes and the engineering fix, and say why the design fixes alone are insufficient.
(c) What would you monitor after launch, and what guardrail would tell you the fix worked without hiding a new problem?

**27.** You inherit a settings screen with 40 options. The PM wants it cut to 8 "because of Hick's Law." You believe the goal is right and the reasoning is wrong.
(a) Correct the reasoning without dismissing the goal.
(b) Propose an alternative approach with concrete steps.
(c) Name the risk your alternative carries, and how you would bound it.

**28.** A subscription product scores well on CSAT and SUS but has poor word of mouth and high churn concentrated at renewal.
(a) Which laws and effects would you reach for, and why does the satisfaction score not contradict them?
(b) What would you investigate first, and with which method?
(c) What would change your mind about your leading hypothesis?

**29.** A support team reports that customers cannot find the returns policy. Analytics shows a high search-to-navigate ratio, a spike in zero-result queries for "send back," and heavy pogo-sticking between the help index and its articles.
(a) Interpret each of the three signals.
(b) Design a validation sequence you could run in two weeks.
(c) What would you ship first, and why that rather than a navigation redesign?

**30.** An A/B test shows the new upgrade prompt lifts conversion 12%, statistically significant. Qualitative sessions show users describing the prompt as "pushy" and one participant says they clicked upgrade by accident.
(a) What do you check about the test itself before interpreting the result?
(b) What downstream metrics would settle the question?
(c) Under what conditions do you ship, and under what conditions do you refuse regardless of the lift?

**31.** A form field's label sits equidistant between two inputs, section headers read as decoration, error messages appear only as red borders, and the submit button is one of three filled buttons on screen.
(a) Deliver the critique in the order you would give it in an interview.
(b) For the error handling specifically, write one replacement message and state the construction rule it follows.
(c) Name the accessibility failures and their success criteria.

**32.** You are asked to design a cancellation flow. The brief says: "Add three retention offers before the confirm step, and put the cancel link in the footer."
(a) Identify what is wrong with the brief and reframe it.
(b) Propose a flow you would be willing to defend publicly.
(c) State the business argument for your version, in the language a commercial stakeholder will accept.

**33.** A design system has 140 components. Adoption is 30%. Product teams say the system "slows them down" and several have forked the button.
(a) Diagnose the likely causes.
(b) Give your intervention plan for the first quarter.
(c) Which metrics would tell you the intervention is working, and which vanity metric would you refuse to report?

**34.** A team is adding an AI assistant that answers questions over a customer's own documents. It sometimes fabricates answers and sometimes returns nothing useful.
(a) Name the core design problems this surface creates.
(b) Give the heuristics you would write for it, with a rationale for each.
(c) How would you design for the failure cases specifically?

**35.** An accessibility audit returns 90 issues on a 12-screen product, with no prioritisation. You have three sprints.
(a) How do you triage, and on what axis?
(b) Give the fix order you would argue for, with reasoning.
(c) How do you stop the backlog regenerating?

**36.** A dense data table for a logistics operations team must show 25 columns, support bulk actions, and be usable for eight-hour shifts. A stakeholder asks you to "make it cleaner, like the consumer app."
(a) Explain why consumer minimalism is the wrong target here.
(b) Give the design moves that improve this table without reducing density.
(c) What would you measure to prove it improved?

**37.** A retail bank's "replace a lost card" journey works on every screen you have tested, yet customers rate it poorly. The journey spans the app, a call centre, a physical letter, and a branch visit.
(a) What artefact would you build, and what would it show that screen-level testing cannot?
(b) Name the likely failure points across channels.
(c) What is the single highest-leverage fix in most versions of this problem, and why?

**38.** A mobile-first product is being adapted to desktop. The team's plan is to stretch the mobile layout to full width and keep the bottom tab bar as a top bar.
(a) Name the reasoning errors in this plan.
(b) Give the adaptation decisions you would make, by category.
(c) What would you test first, and with whom?

**39.** Activation is defined as "completed the product tour." 80% of users complete the tour; 12% are still active at day 30.
(a) What is wrong with the activation definition, and what would you replace it with?
(b) Break the problem into causes and give the distinct fix each one implies.
(c) Which cohort analysis would you run, and what result would change the roadmap?

**40.** A growth team proposes a streak mechanic with a daily push notification and a visible "you'll lose your 47-day streak" warning before the user can pause.
(a) Analyse the mechanic using the behavioural models.
(b) Apply the ethical test explicitly and state your conclusion.
(c) Propose a version you would ship, and name what you would monitor to detect harm.

---
---

## Solutions

**1. b)** Anticipated use puts expectation inside the definition, which is why pricing, marketing claims, onboarding emails, and even the app-store screenshot are UX surface — they set the expectation the product is then judged against. (a) confuses a definition with a method; (c) desirability is a separate quality dimension; (d) the standard is deliberately not software-specific.

**2. c)** Alphanumeric meaning requires conscious, serial processing — reading. Hue, size, orientation, motion, and enclosure are all processed pre-attentively in roughly 200 ms, which is why a design can be judged by squinting but not by reading.

**3. b)** Logarithmic: `RT = a + b·log2(n+1)`. (a) and (c) are the common intuitions and both are wrong; the practical consequence is that deleting options buys far less than people assume, and ordering, grouping, and search buy more.

**4. b)** Common region beats proximity. This is exactly why a card drawn around the wrong elements defeats otherwise correct spacing — the boundary wins and no amount of spacing tuning fixes it.

**5. b)** User control and freedom — the heuristic that calls for a clearly marked emergency exit and support for undo and redo. (a) concerns language and conventions, and is not what fails here.

**6. b)** 3:1 covers large text (1.4.3) and non-text contrast for UI component boundaries and meaningful graphics (1.4.11). Normal body text needs 4.5:1. Purely decorative graphics are exempt, which is why (c) is wrong.

**7. b)** Semantic tokens (`color-text-primary`, `color-border-danger`) express role rather than value, which is what makes dark mode, high-contrast modes, and white-label themes remappings rather than rewrites. Components consuming primitives is the most common cause of a theme that will not theme.

**8. b)** A tree test. The sort is generative and reveals the user's model; the tree test is evaluative and tests yours. Neither substitutes for the other, and running only the sort is the classic mistake.

**9. b)** Activation — the moment a user first experiences core value. Acquisition is mostly a marketing lever; revenue and referral are downstream of a user who never got value in the first place.

**10. b)** All three must converge at the same moment: motivation, ability, and a prompt. The practical consequence is that the cheapest intervention is almost always increasing ability (making the behaviour easier), not increasing motivation, because motivation is expensive and decays.

---

**11.** The **system model** (how the thing actually works), the **conceptual model** (the story the interface tells about how it works), and the **user's mental model** (what the user believes). The designer owns the **conceptual model** — you cannot legislate what users believe, and you usually cannot change the system, but you choose the story the interface tells, and the quality of the design is largely the distance between that story and the user's model.

**12.** It licenses: with a **homogeneous user group**, testing **five participants** in an **iterative** round surfaces most of the *usability problems* that round will surface. It does not license: five users per *product* when you have distinct segments (it is five per segment); any claim about *proportions* or preference ("60% preferred B" from five people is noise); any claim about whether the feature is *wanted*, which is a different question requiring a different method; and it says nothing about problems that only appear at scale, on slow connections, or with real data.

**13.** Miller's 1956 paper concerned the span of immediate memory measured in *chunks* — items held in the head. A menu is visible on screen, so nothing is being held in memory; the constraint is visual search and information scent, not memory span. Modern working-memory estimates are closer to ~4 chunks in any case. The law genuinely applies wherever the interface takes away information the user still needs: a confirmation code shown once and needed two steps later, table headers that scroll out of view, instructions in a dismissed modal, or values a user must transcribe between screens.

**14.** The criterion is **2.4.7 Focus Visible (AA)**. Harmed: every keyboard-only user, including people with motor impairments, screen-reader users, people using switch access, and a large population of power users — the indicator is how they know where they are. The fix is not to restore the browser default and accept it; it is to **design** the focus state as a deliberate part of the visual language, meeting **1.4.11** at 3:1 against adjacent colours, with sufficient thickness and offset to survive on every background. If the concern is that it appears on mouse click, `:focus-visible` addresses the aesthetic complaint without removing the indicator.

**15.** An **affordance** is a possibility for action offered by a thing to a capable actor — it exists whether or not anyone perceives it. A **signifier** is the perceptible cue that communicates where that action is possible. Example: a swipeable list row affords swiping, but with no peeking action colour, no chevron, no hint animation, and no first-run cue, the signifier is absent — the action exists and is undiscoverable, which is functionally identical to it not existing for most users.

**16.** **Uniform connectedness → common region → proximity → similarity.** It is useful because these cues routinely conflict in real layouts. When a card boundary groups A and B while spacing groups B and C, the boundary wins and users perceive A+B. Knowing the ordering lets you predict which cue users will actually follow and fix *that* one, rather than piling additional cues on top of a conflict — which is the usual response and which makes the layout heavier without making it clearer.

**17.** **Goal:** users who are locked out get back into their account quickly and without contacting support. **Signals:** fewer support contacts about access; more reset flows started that end in a successful login; fewer repeat resets by the same user within a short window; fewer abandoned resets at the email step. **Metrics:** password-reset support contacts per 1,000 active users; reset-to-successful-login completion rate; repeat-reset rate within 7 days; step-level abandonment at request, email, and new-password entry. Guardrail: account-takeover rate must not rise, because the cheapest way to improve completion is to weaken verification.

**18.** Any three, e.g. — **Inconsistent terminology** across screens ("account" here, "profile" there) forces re-learning at every step; fix by agreeing one term per concept and enforcing it in the content guidelines. **Information presented as prose when it is structurally a table or list** forces the user to parse and hold structure; fix by giving it the structure it actually has. **Requiring transcription between screens** (a code, a reference number, an amount) turns recognition into recall; fix by carrying the value forward, or by making it copyable and visible where it is needed. Others acceptable: unlabelled icons, decorative motion competing with content, split attention between an instruction and the field it governs, and inconsistent control placement between steps.

**19.** The say-do gap is the systematic divergence between what people report about their behaviour and what they actually do: they misremember past behaviour, cannot reliably predict future behaviour, and rationalise both. The rule it implies: **when attitudinal and behavioural evidence are both available, weight the behavioural.** Use the attitudinal data to explain the mechanism, not to establish the fact.

**20.** Optimistic UI — showing the result before the server confirms — is right when the action has a **high success rate and a low cost of being wrong**: likes, marking read, reordering a list, adding a tag. It is harmful when failure is plausible and consequential, because you then have to *un-tell* the user, and a reversal is more damaging than the wait would have been: payments, irreversible deletes, anything with legal or financial weight. The deciding question is: **if this fails after I have already shown success, what does the user have to do about it, and can they still do it?** If the answer involves money, data loss, or a message someone else has already seen, be pessimistic.

**21.** **Primitive** — raw values, e.g. `blue-600`, `space-4`. **Semantic** — role-based, e.g. `color-text-primary`, `color-surface-raised`, `color-border-danger`. **Component** — optionally scoped to one component, e.g. `button-primary-background`. The middle tier exists to decouple decision from usage: it is the layer that makes theming, dark mode, and accessibility modes a remapping rather than a rewrite, and it makes misuse *auditable* — a `danger` token on a neutral border is visible in review, while `#D93025` is not.

**22.** Any four, with costs — **Empty on first use** (missing: the user's first impression of the product is a blank screen with no path to value, which is an activation failure, not a cosmetic one). **No results after filtering** (missing: indistinguishable from empty-on-first-use, so the user believes the data is gone rather than filtered). **Partial / degraded** (missing: one failed sub-request blanks the whole screen instead of the one region that failed). **Error with a recovery path** (missing: the user is told something went wrong and given nothing to do). Also acceptable: loading, overflowing/long-content, offline, permission-denied, and success.

**23.** **Internationalisation (i18n)** is the structural preparation that makes a product *capable* of being adapted: externalised strings, no text baked into images, layouts that tolerate 30–40% text expansion and right-to-left mirroring, locale-aware dates, numbers, currency, name and address formats, and no assumptions about sort order. **Localisation (l10n)** is the act of adapting to a specific locale: translation, content, imagery, and conventions. If you skip internationalisation, translation breaks the interface rather than filling it — German strings overflow fixed-width buttons, RTL layouts mirror incorrectly, dates parse wrongly, and name fields reject valid names. The costly part is that these are structural fixes discovered at translation time.

**24.** Test: **"Would this design still work if the user could see exactly how it works and why we built it?"** — or equivalently, does this help the user reach a goal they already hold, or does it manufacture a goal that serves us at their expense? A category with real regulatory exposure: **fake urgency and false scarcity** (timers that reset on reload, "only 2 left" that is not inventory-backed), alongside **subscription traps** and **confirmshaming**; these are named in consumer-protection enforcement and in the EU's regulatory framework, so the exposure is legal, not only ethical.

---

**25.**
**(a) Diagnosis.** Three mechanisms. **Pop-out has been destroyed by uniformity**: with fourteen tiles identical in size, weight, and treatment, no tile differs from its distractors, so pre-attentive search fails and the user is forced into serial reading — which is the literal experience of "I don't know where to look." **The emphasis budget is overspent on the actions**: four filled buttons means none is primary; the pop-out effect requires the target to differ from *all* distractors, so Export is now found by reading, not by seeing. **There is no grouping**: fourteen equal items with no common region or proximity structure gives the eye no chunks, so working memory has nothing to hold and the whole field is processed as fourteen separate objects.

**(b) Changes, in priority order.**
1. **Establish hierarchy among the tiles.** Identify the one or two metrics that drive a decision and make them dominant — larger type, more space, possibly a wider tile — and demote the rest to a uniform secondary treatment. Isolation only works against a plain background (Von Restorff), so the demotion is as important as the promotion.
2. **Group the remaining tiles into two or three clusters** by question answered, using proximity and, if needed, one region mechanism per level — a card *or* a background tint, never both.
3. **Reduce to one filled primary in the header.** Export becomes the filled button; Share and Schedule become outlined or text; Configure moves out of the action row entirely, since it is a settings action, not a task action.
4. **Remove the fourteen sparklines** or reduce them to the tiles where trend is actually part of the decision. Applied uniformly, they are visual noise that adds weight without adding information.
5. **Order for serial position** — most decision-relevant first, since first and last positions carry the most weight.

**(c) Verification.** Squint test or greyscale pass first, as a five-second check that the intended hierarchy survives and Export is still the first action the eye lands on — greyscale also confirms nothing depends on hue alone. Then a **first-click test** on a static image with 15–20 users for "where would you click to export this?", because a correct first click strongly predicts eventual success. Then a moderated pass with 5–8 users per segment on the real decision task, not on "find Export" — finding the button is necessary, but the dashboard's actual job is answering a question. After ship, watch time-to-first-action and Export completion rate, with a guardrail on whether the demoted metrics are now being missed by users who need them.

*Marking:* a strong answer names the mechanism (pop-out requires difference from all distractors; isolation requires a plain field) and prioritises demotion as heavily as promotion. A weak answer says "add hierarchy and make Export stand out" without explaining why fourteen tiles with sparklines is the cause, and offers no verification beyond opinion.

**26.**
**(a) Laws and principles.** **Doherty Threshold (~400 ms)** — six seconds is fifteen times past the threshold at which interaction feels continuous, so the system reads as broken and the user retries. **Response-time bands** — six seconds sits in the 1–10 s band, where an indeterminate spinner is insufficient and determinate, staged progress is required. **Postel's Law / robustness** — the system must be liberal in what it accepts, and a user tapping twice is the realistic input, not the pathological one. **Peak–End Rule** — a double charge is a catastrophic negative peak that will dominate the memory of the entire product regardless of how good everything else was. **Fitts's Law, inverted** — a large, isolated "Pay" button makes the second tap almost free.

**(b) Fixes.** *Design:* acknowledge the tap in under 100 ms with an immediate state change on the button itself — label change to "Authorising…", disabled state, and a visible spinner *on the control the user touched*, not elsewhere on the page. Replace the indeterminate spinner with staged determinate messaging ("Authorising payment… Confirming order…") so the six seconds is legible rather than ambiguous. Add a brief post-tap dead zone so a reflexive second tap lands on nothing. Choose **pessimistic** UI here, not optimistic — this is precisely the case where showing success early and reversing it is worse than the wait. *Engineering:* make the payment request **idempotent** with a client-generated key, so a duplicate submission cannot produce a duplicate charge.

Design fixes alone are insufficient because they only address the taps you can see. A disabled button does not prevent a network-level retry, a back-button re-post, a double-submit from a flaky connection, or a user reloading and resubmitting. The idempotency key is the only fix that makes double-charging structurally impossible; the design fixes make the wait tolerable and reduce the *rate* of duplicate submissions. Ship both: idempotency is correctness, the design work is experience.

**(c) Monitoring.** Primary: duplicate-charge rate per 10,000 transactions (target zero) and payment-step abandonment. Secondary: median and p95 authorisation latency, since a six-second p50 usually hides a much worse tail. Guardrail: **refund and chargeback rate**, plus payment-related support contacts — because the cheap way to make abandonment look better is to hide failures, and refunds catch that. Also watch checkout completion rate, so you can distinguish "fewer duplicate taps" from "fewer people getting through at all."

*Marking:* full credit requires **idempotency as the real fix** *and* **sub-100 ms acknowledgement as the perceived fix**, plus an explicit statement that design alone cannot solve it. Naming only the spinner, or only the disabled button, is a half answer. A strong answer also picks pessimistic UI deliberately and says why.

**27.**
**(a) Correcting the reasoning.** Agree with the goal first: the settings screen is unmanageable and that is a real problem worth solving. Then correct the mechanism. Hick's Law is **logarithmic**, so the saving from 40 to 8 options is roughly the difference between log2(41) and log2(9) — not a fivefold gain, and small in absolute terms. The law also assumes **equally probable options**, which settings never are: a handful are changed constantly and most are touched by almost nobody, so ordering and grouping do far more work than deletion. Most decisively, **a settings screen is a visual search problem, not a decision problem** — the user arrives knowing what they want and needs to find it, and Hick's Law does not describe finding. Finally, **Tesler's Law**: the complexity does not vanish when the option is deleted; it relocates to support tickets, to workarounds, and to the users who can no longer do their job.

**(b) Alternative.** 1. Instrument the screen and get usage per setting over a full seasonal cycle. 2. Run a card sort with 15–30 users to find the groupings and, more importantly, the *names* they use. 3. Restructure into 5–6 labelled sections validated by the sort, so proximity and common region carry the structure. 4. Add search over setting names, descriptions, and synonyms — this is what most users will actually use. 5. Promote the top-changed settings to the top of the screen. 6. Move verified-low-usage settings behind an "Advanced" disclosure rather than deleting them. 7. Only then consider removing options with near-zero usage, one at a time, behind a flag so it is reversible.

**(c) Risk and bounding.** The risk is that low usage is not the same as low importance: a setting used by 0.3% of accounts may be load-bearing for your largest customer, an accessibility accommodation, or a regulatory requirement in one market. Averages conceal exactly this. I would bound it by segmenting usage by plan, tenure, region, and assistive-technology signal before touching anything; by cross-checking the removal candidates against support tickets and account-management escalations; by removing behind a flag with a fast rollback; and by keeping a defined threshold — nothing gets deleted in the same quarter it is deprecated. Second risk: search only helps if users' vocabulary is in the index, which is why the card sort's naming output feeds the synonym list.

*Marking:* the strong answer keeps the PM's goal while rejecting the mechanism, and offers something measurable. Simply saying "Hick's Law does not say that" is half an answer; so is agreeing and cutting to eight. Naming the low-usage-is-not-low-importance risk unprompted is the senior move.

**28.**
**(a) Laws and effects.** **Peak–End Rule** is the leading candidate. Satisfaction instruments sample the average or the recent moment, but word of mouth and renewal decisions are driven by the *remembered* experience — the worst moment and the ending. A product can have a good average and a terrible peak. **Duration neglect** is why a bad month can outweigh eleven good ones. The **Aesthetic–Usability Effect** is a methodological caution: if the product is attractive, self-reported scores are inflated relative to actual task performance, so a good SUS is weaker evidence than it appears. **Zeigarnik and Goal-Gradient** raise a different possibility — that many users never reached core value at all, in which case renewal is being judged against an experience that never happened. **Jakob's Law** if a recent redesign reset learned models, which would concentrate churn in tenured users.

There is no contradiction: the satisfaction scores and the churn are measuring different things. CSAT is transactional and sampled from people still present; the renewal decision is a judgement about the whole relationship made by a population that includes everyone the surveys have already lost.

**(b) First investigation.** Segment churn by tenure and by whether the account ever hit the activation milestone — that single cut usually separates "the value never landed" from "the value landed and then something broke." Then interview 8–10 recently churned users, with the interview deliberately structured around two things: the worst moment in the relationship, and the renewal experience itself, since the renewal *is* the ending being judged. Pair with behavioural data — support contact history, incident timeline, billing events — so you can triangulate rather than relying on recall. Also inspect the renewal mechanics directly: a surprise price rise, a silent auto-renew, or a difficult cancellation is a bad ending manufactured by the company.

**(c) What would change my mind.** If churn is flat across tenure and unrelated to activation, and the interviews surface no common low point, then Peak–End is the wrong frame and I would look instead at whether the product's value is genuinely time-limited — a tool people finish using, where churn is a natural end of the job rather than a failure. Equally, if churn concentrates in a single acquisition channel or segment, the problem is upstream in acquisition and no experience fix will move it. And if satisfaction scores are drawn only from users who contacted support or from a heavily self-selected panel, the premise of the question is a sampling artefact.

*Marking:* strong answers explain *why* good scores and bad churn are compatible rather than treating one as wrong, and name a concrete first cut of the data. Weak answers list laws without connecting them to an investigation, or propose "run a survey," which repeats the instrument that already failed.

**29.**
**(a) Interpreting the signals.** A **high search-to-navigate ratio** means navigation is failing to carry people to content — though for a large catalogue, search dominance can be normal, so the signal matters as a *change* or in comparison to a baseline. **Zero-result queries for "send back"** is a direct vocabulary gap: users' word for the concept is not in your index and probably not on your navigation labels either, which is a labelling failure, not a content failure — the policy exists, it is just named something else ("Returns & Refunds", or worse, "Order Management"). **Pogo-sticking between the index and articles** is weak information scent: the link labels and snippets do not let users predict what is behind them, so they open, reject, and go back. Together the three say the content exists and is misnamed and mis-signposted.

**(b) Two-week validation sequence.** Days 1–3: content inventory of the help section with traffic and last-updated dates, plus a full pull of search logs, zero-result queries, and support-ticket topics — all free and continuous. Days 3–5: open card sort with 15–30 users on 30–60 help topics, principally to harvest the vocabulary they use. Days 5–7: draft two candidate structures and label sets. Days 7–11: tree test both with 30–50 users each, on tasks phrased in the users' words rather than yours; record success, directness, and first click. Days 11–13: fix the labels that produced high success with low directness — those are ambiguous labels on a workable structure — and re-test only the weakest tasks. Day 14: first-click test on the designed index screen.

**(c) Ship first.** The **label and synonym fix**, not the navigation redesign: add "send back", "return", "refund" as synonyms in search, rename the section to the users' term, and rewrite the index link labels and snippets to carry scent. This ships in days rather than quarters, is reversible, addresses the mechanism the evidence actually points to (vocabulary and scent), and requires no structural migration or redirects. A navigation redesign is expensive, risks breaking things that currently work, and would be an unvalidated bet on structure when the evidence points at naming. If the tree test then shows the structure itself is failing, you have earned the right to restructure with evidence.

*Marking:* a strong answer treats the three signals as pointing at *naming and scent* rather than jumping to a redesign, distinguishes card sort from tree test by the question each answers, and justifies the cheap fix on reversibility and evidence. Weak answers propose an IA overhaul immediately.

**30.**
**(a) Test validity checks.** Was it **powered** — was a minimum detectable effect and sample size calculated before launch, or was the test stopped when it looked good (**peeking**, which massively inflates false positives)? Did it run at least one **full weekly cycle** to avoid day-of-week composition effects? Was there **one pre-registered primary metric**, or is 12% the survivor of twenty comparisons? Are the **guardrail metrics** intact — latency, error rate, support contacts, revenue per user? Is the effect **12% relative on a small base**, and what is the confidence interval — statistical significance is not importance. Could this be a **novelty effect**, where a new prompt wins temporarily because it is new? Finally, is the assignment clean and is the population representative?

**(b) Downstream metrics.** The accidental-click report is the important signal, because it suggests the lift may be measuring mis-taps rather than intent. So: **immediate cancellation or refund rate** among upgraders in the variant; **downgrade rate within the first billing cycle**; **retention at 30 and 90 days** for the upgraded cohort, compared with control upgraders; **support contacts** mentioning unwanted charges; **chargeback rate**; and **long-run revenue per user**, not conversion. A change that lifts conversion and lifts refunds by more is a loss dressed as a win. I would also check whether the prompt's hit area overlaps a common tap target, which would explain accidental clicks mechanically.

**(c) Ship or refuse.** Ship if the lift survives the guardrails — refunds, cancellations, and 30-day retention are flat or better — and the qualitative complaint is about *unfamiliarity or assertiveness* rather than about being misled. "Pushy" is a legitimate design note to act on, but it is not disqualifying on its own. Refuse regardless of the lift if the mechanism is deception or mis-taps: if the prompt's win depends on users not understanding what they agreed to, on a confirm button placed where a dismiss button used to be, on false urgency, or on a hit area that captures accidental taps. That is a dark pattern, and the ethical test applies — it would not survive the user seeing exactly how it works. In that case I would rebuild the prompt honestly and re-test; if the honest version does not win, the finding is that the offer is not compelling, which is more useful than a lift built on confusion.

*Marking:* the strong answer separates "is the test trustworthy" from "is the result good", names peeking and novelty specifically, and gives a bright line for refusal that is about mechanism rather than sentiment. A weak answer either defers to the number or rejects it on the strength of one participant's comment.

**31.**
**(a) The critique, in order — structure before surface.**
1. **Primary task.** "What is this screen for? If it is completing this form, everything on it should serve that, and I will judge each element against it."
2. **Grouping.** "The section headers are not reading as headers because the space above a header equals the space between fields — proximity is not encoding the section structure, so I read one long list. I would make between-section spacing roughly double the within-section spacing."
3. **Field–label association.** "Each label sits equidistant between two inputs, so proximity is ambiguous and users will associate labels with the wrong field, especially when scanning or when the layout reflows. Tighten label-to-its-own-field to the smallest step on the spacing scale and keep field-to-field larger."
4. **Emphasis.** "Three filled buttons means there is no primary. Emphasis is relative, so one filled primary and the rest outlined or text restores the pop-out. Colour alone should not carry it — weight, size, and position should too."
5. **Error handling.** "Errors are communicated by a red border only. That is colour alone, it carries no information about what is wrong, and it disappears for anyone who cannot perceive the hue."
6. **Verification.** "I would squint or view it in greyscale to check the groups survive and the primary action is still the first thing my eye lands on, then validate with a first-click test rather than assuming my grouping matches users'."

**(b) Replacement message.** For an invalid date of birth: "**Enter your date of birth as DD/MM/YYYY — for example, 14/03/1989.**" The construction rule: an error message states **what went wrong, where, and what to do about it**, in the user's language rather than the system's, without blame, and placed adjacent to the field it concerns so it is within the locus of attention. "Invalid input" fails all three parts; "Error 422" fails all four. Where possible, prevent the error instead — a date input that accepts multiple formats and normalises them (Postel's Law) is better than a well-written rejection.

**(c) Accessibility failures.**
- **1.4.1 Use of Color (A)** — the red border is the sole indicator of error state. Needs text and an icon alongside.
- **3.3.1 Error Identification (A)** — errors must be described in text, not implied by styling.
- **3.3.3 Error Suggestion (AA)** — where a correction is known, suggest it; the format example does this.
- **3.3.2 Labels or Instructions (A)** and **1.3.1 Info and Relationships (A)** — the ambiguous label placement is a visual failure, but if the label is not programmatically associated with its input it is also a structural one; a screen reader will announce the wrong label or none.
- **4.1.3 Status Messages (AA)** — the error summary must be announced without moving focus, via a live region.
- **1.4.11 Non-text Contrast (AA)** — the red border itself must reach 3:1 against the adjacent background to be perceivable at all.

*Marking:* the strong answer critiques structure before surface, names the mechanism for each point (proximity, relative emphasis, colour-alone), and gives a specific fix with a number attached. A weak answer says "add spacing and make the button pop" and treats accessibility as a separate afterthought rather than as part of the same critique.

**32.**
**(a) What is wrong, and the reframe.** The brief states a solution and hides its own goal. Two specific problems. First, **three retention offers before confirm is a roadblock**, a named dark pattern: it converts a decision the user has already made into an obstacle course, and it produces cancellations anyway — just angrier ones. Second, **burying the cancel link in the footer is obstruction**, and in several jurisdictions it is now a regulatory exposure rather than a design preference; consumer-protection rules increasingly require cancellation to be as easy as signup. The reframe: the goal is not "make cancelling hard", it is **"reduce avoidable churn and learn why people leave."** Those are different problems with different solutions, and the second one is achievable. I would also point out that the brief's version harms the metric it intends to help, because the memory of a hostile cancellation is what determines whether the user ever returns or recommends you — a Peak–End problem with a direct commercial cost.

**(b) The flow I would defend.** Cancel is discoverable where users look for it — in account settings, one level from the subscription — and reachable in the same number of steps as signing up. On the first screen, **one** question: why are you leaving, with a small set of real options and a free-text field. Then, **conditional on the reason and only where it is genuinely relevant**, one targeted alternative: if the reason is price, offer the cheaper tier; if it is "not using it right now", offer a pause with a clear end date; if it is a missing feature or a bad experience, offer nothing and route the feedback to the team. If the reason is "I never got it working", offer help, once. Confirm clearly, state exactly what happens to their data and access and when, send a confirmation email, and make resubscribing genuinely easy. No confirmshaming copy, no timers, no "are you sure?" repeated. The pause option is the honest version of retention and typically the highest-performing one.

**(c) The commercial argument.** Frame it in the language of value, not ethics. Reason-coded cancellation data is a continuously running research instrument that tells you which churn is addressable and which is not — that is worth more than a small number of coerced retentions. A pause converts a permanent loss into a temporary one, and paused users resurrect at far higher rates than churned users, at near-zero acquisition cost. Coerced retentions are low-value: they concentrate in involuntary churn, refunds, chargebacks, and support cost, and they suppress the one metric that compounds — willingness to return and recommend. And the regulatory exposure is now real: enforcement against subscription traps is active, and the cost of being on the wrong side of it dwarfs the retention delta. "Easy to leave, easy to come back" is the version that maximises lifetime value rather than this quarter's cancellation count.

*Marking:* the strong answer names the specific dark patterns (roadblock, obstruction, confirmshaming), reframes the goal rather than refusing the task, ships a concrete alternative, and argues it commercially. A weak answer either complies with the brief or declines it on moral grounds without offering a defensible flow and a business case.

**33.**
**(a) Diagnosis.** 140 components at 30% adoption is a system that grew by accumulation rather than by demand. Likely causes: **components at the wrong level of abstraction** — too specific to reuse, or so generic that every consumer reimplements the meaning; **the pattern layer is missing**, so the system supplies buttons but no answer to "how do we do forms, empty states, errors, tables", which is where teams need the most help and where consistency is actually created; **states are incomplete**, so teams fork the moment they need loading, error, or disabled; **contribution is closed or slow**, so forking is faster than contributing — forking the button is almost always a symptom of a broken contribution loop, not of a bad button; **no escape hatch**, so a team with a legitimate one-off has no sanctioned route and goes around the system entirely; **design–code drift**, so the Figma library and the code library disagree and neither is trustworthy; and **documentation without a "when not to use"** section, so misuse is common and the system gets blamed for it.

**(b) First-quarter plan.** Stop building. 1. **Audit against production**: which components are actually used, where teams have forked, and what they forked *to*. The forks are your highest-quality requirements document. 2. **Talk to the three lowest-adoption teams** about what specifically slowed them down; adoption is a service problem before it is a technical one. 3. **Fix the top five components' completeness** — all states, accessible by default, content guidance, and a "when not to use" section — rather than shipping new ones. 4. **Open the contribution loop**: a documented path, a named reviewer, a service-level expectation for response, and public credit. 5. **Add a sanctioned escape hatch** so a one-off is a legitimate, labelled decision rather than a fork. 6. **Ship two or three patterns**, starting with forms and empty states. 7. **Deprecate aggressively** — components with near-zero usage cost trust and maintenance. 8. **Add drift detection**: token linting, a periodic production-versus-library audit, and versions released together with a changelog.

**(c) Metrics.** Meaningful: **component adoption rate weighted by production surface** (what share of rendered UI comes from the system, not how many components exist); **fork count and its trend**; **contribution throughput and time-to-merge**, which is the real health signal for the loop; **time-to-first-screen for a new team**; **accessibility defects per screen in system-built versus hand-built UI**, which is where the system's largest multiplier shows up; and **qualitative sentiment from consuming teams**, sampled regularly. The vanity metric I would refuse to report is **total number of components** — it only goes up, it is negatively correlated with the outcome we want, and reporting it rewards exactly the behaviour that produced the problem. I would also resist raw "downloads" or "installs" for the same reason.

*Marking:* strong answers read the fork as a contribution-loop failure rather than as bad behaviour, stop building before fixing, and pick a metric that can go down. Weak answers propose evangelism, better documentation, or a mandate without addressing why the system is slower than not using it.

**34.**
**(a) Core design problems.** **Capability expectation** — a text box implies unbounded competence, so users ask for things the system cannot do and blame the product for the mismatch. **Uncertainty is invisible** — the confident sentence and the fabricated sentence look identical, which is the defining hazard of the surface. **Verification cost** — if checking the answer takes as long as finding it manually, the feature has negative value for exactly the users who most need it to be right. **Correction and steering** — a wrong answer with no way to redirect forces the user to abandon and start again. **Non-determinism** — the same question can give different answers, which breaks the mental model of a tool and makes the system unteachable. **Provenance** — with a customer's own documents, "which document said this, and where" is the whole product. **Failure asymmetry** — a fabricated answer about a contract clause is not a mildly wrong answer; the cost of a mistake varies enormously by question and the interface currently treats every answer the same.

**(b) Heuristics I would write for it.**
1. **Set capability expectations at the boundary.** Show what it can and cannot answer where the user forms intent, not in a help page — because the input affordance is what sets the expectation.
2. **Show sources for every claim, inline and specific.** Rationale: with document-grounded answers, a citation to the passage converts an unverifiable assertion into a checkable one, and collapses verification cost.
3. **Expose uncertainty in a form the user can act on.** Rationale: a hedge in prose is ignored; "I found this in one document and it contradicts another" is actionable.
4. **Make correction cheap and in-place.** Rationale: steering an answer must cost less than re-asking, or users abandon the feature rather than fix it.
5. **Make the cost of a mistake visible and proportional.** Rationale: a summary and a contractual figure warrant different levels of friction and confirmation.
6. **Always offer a deterministic fallback.** Rationale: keyword search over the same documents must remain one click away; the assistant is an accelerator, not a replacement, and users need a path they can trust when it matters.
7. **Never fabricate a citation, and prefer refusal to invention.** Rationale: an honest "I could not find this" preserves trust; a plausible wrong answer destroys it permanently, and trust in this surface is not recoverable at the same rate it is lost.
8. **Keep the user in control of what is read and retained.** Rationale: these are the customer's documents, and the privacy and permissions model is part of the interface, not infrastructure.

**(c) Designing for the failure cases.** Treat the two failure modes as distinct designs. For **fabrication**: bind every assertion to a retrieved passage and render the passage inline; if no passage supports it, do not render the assertion — design the refusal state as a first-class outcome with a useful next step ("no document mentions this; search all documents for X", "try these related passages"), not as an apology. For **no useful answer**: make it a productive dead end rather than a blank — show what was searched, what was found but rejected, and offer query reformulation and the deterministic search fallback. Add lightweight feedback capture at the point of failure, because the failures are the roadmap. Instrument the ratio of answers where a source was opened, the correction rate, and the fallback-to-search rate. And define, up front, the classes of question the assistant will refuse and route elsewhere — legal, medical, or contractual specifics where the cost of a confident error is unbounded.

*Marking:* the strong answer treats uncertainty, provenance, and verification cost as the design problem rather than as model limitations, and designs the failure states in as much detail as the success state. A weak answer describes a chat UI and adds a disclaimer.

**35.**
**(a) Triage axis.** Not by WCAG number and not by screen. Triage on **severity as harm**: how many users are affected, how badly, how frequently, and whether there is any workaround. The key axis is **blocking versus degrading** — an issue that makes a task impossible for a whole population outranks an issue that makes it unpleasant for everyone. Cross-cut that with **task criticality** (a blocker on signup or checkout outranks a blocker on a settings page nobody visits) and **breadth** (an issue in a shared component appears on all twelve screens and is one fix). Ninety findings on twelve screens is almost certainly a much smaller number of underlying causes, so the first analytical step is deduplication: group by root cause, not by instance.

**(b) Fix order and reasoning.**
1. **Keyboard traps and anything that makes a critical task impossible** (2.1.1, 2.1.2). These are total exclusions; nothing else competes.
2. **Missing or broken form labels and error identification on the critical path** (3.3.1, 3.3.2, 1.3.1, 4.1.2). An unlabelled input on signup excludes screen-reader users from the product entirely.
3. **Missing focus indicators** (2.4.7). One of the most common and most damaging failures, and usually a small number of token and component fixes.
4. **Custom controls without name, role, or value** (4.1.2), because these look fine and are entirely opaque to assistive technology.
5. **Contrast failures on text and component boundaries** (1.4.3, 1.4.11). High volume, high breadth, and usually fixable at the token layer in a single change — which is why they often come early in practice despite being degrading rather than blocking.
6. **Status messages not announced** (4.1.3) — the user acts and receives no confirmation.
7. **Reflow and target size** (1.4.10 at 320 CSS px, 2.5.8 at 24×24) — real and important, but generally degrading rather than blocking.
8. **Remaining single-screen, low-traffic issues.**
The reasoning throughout: fix by root cause and by breadth, prioritise exclusion over inconvenience, and take the token-layer fixes early because they clear large numbers of findings for one unit of work. Trade-off to state: this order optimises for harm removed per sprint, which means some easy wins wait — acceptable, provided the blocking issues genuinely land in sprint one.

**(c) Stopping regeneration.** An audit-and-fix cycle without a structural change simply reschedules the same work. So: **build accessibility into the design system** — components accessible by default is the single biggest multiplier, because it moves correctness from every consumer to one place. Add **automated checks in CI** (they catch perhaps a third of issues, which is a third you never triage again) plus **linting on token misuse**. Add **accessibility acceptance criteria to the definition of done**, and specify it in handoff — focus order, accessible names, semantics, and announcements are design decisions, not implementation details. **Test with real assistive technology on the real flows** each release, because conformance can pass while the flow remains unusable. Run **keyboard-only and screen-reader passes in design review**, not after. And track defects per screen for system-built versus hand-built UI, so the argument for the system's value stays evidenced.

*Marking:* strong answers deduplicate 90 findings into root causes and triage on harm and breadth rather than on conformance level, and treat prevention as part of the answer. Weak answers sort by A/AA/AAA or promise to fix everything.

**36.**
**(a) Why consumer minimalism is wrong here.** The stakeholder is importing a heuristic from a context with opposite constraints. A consumer app serves infrequent, low-expertise users doing short tasks, where whitespace and progressive disclosure reduce the cost of not knowing what to do. This table serves **trained experts doing repetitive work for eight hours**, for whom the dominant cost is not learning but **navigation and scanning per unit of information**. Hiding columns behind disclosure does not remove complexity — **Tesler's Law** — it moves it into extra interactions performed hundreds of times a day, which is a direct throughput cost and a fatigue cost. Density is a *feature* for expert tools; the actual problem to solve is not "too much information", it is "information that is hard to scan." **Aesthetic–Usability** is the trap here: the cleaner version will demo better and perform worse, and the stakeholder will be judging the demo.

**(b) Design moves that improve scanning without reducing density.**
- **Typography and alignment**: tabular numerals, right-align numeric columns, left-align text, align on the decimal. This alone transforms comparability at no density cost.
- **Reduce boundaries, use the spacing scale**: remove full-cell borders; a very light hairline or zebra striping (uniform connectedness) supports row tracking at high density without the visual weight of a grid. State the trade-off honestly — at this density hairlines genuinely help, so this is one of the few cases where more lines is right.
- **Group columns** into labelled logical clusters with a slightly larger gap between clusters than within, so proximity encodes structure across 25 columns.
- **Freeze the identifying column and the header** — this is a direct Miller's Law application: the header scrolling out of view forces the user to hold column identity in memory.
- **Encode status pre-attentively** — a small shape or position cue plus text, never colour alone, so exceptions pop out in a 200 ms scan.
- **Full keyboard operability**: arrow navigation, type-ahead, shortcuts for the top actions, and range selection. For an eight-hour user, keyboard is the primary input and Fitts's Law says the mouse trip to a toolbar is a real, repeated cost.
- **Bulk actions with a persistent selection count and a genuine undo** — reversibility matters more than confirmation for repetitive work, because confirmation dialogues get dismissed reflexively.
- **Persist state across sessions**: column widths, sort, filters, and scroll position. Losing them is a daily tax.
- **Density control** as an explicit user setting, defaulting to compact.
- **Reduce eye-strain surface**: lower-contrast rules, restrained colour, no decorative elements competing at the periphery.

**(c) Measurement.** Task-level and behavioural, not attitudinal: **time on task for the three most frequent real workflows**, measured with realistic data volumes; **error rate and correction rate** on those tasks; **actions per completed unit of work** (a proxy for navigation cost); **scroll and horizontal-scroll distance per task**; and **throughput per shift** if operations already tracks it. Attitudinally, **SEQ per task** and a fatigue question late in a shift rather than a general satisfaction score. Guardrail: error rate must not rise as speed improves — faster wrong work is not an improvement. I would benchmark before the change so the comparison is real, and I would test with the actual operations team, not with proxies.

*Marking:* the strong answer refuses the consumer analogy with a reason (different user, different cost function, Tesler's Law) while still delivering improvements, and measures throughput and errors rather than satisfaction. A weak answer either complies and reduces density or refuses without offering anything.

**37.**
**(a) The artefact.** A **service blueprint** for the whole journey: the customer's actions across every channel, the frontstage touchpoints they see, the backstage actions staff take, and the support processes and systems underneath, with lines of interaction, visibility, and internal interaction drawn explicitly. Screen-level testing cannot show what a blueprint shows: the **handoffs between channels**, where the experience is owned by nobody. Each screen can pass its own usability test while the journey fails at the seams — the app tells the customer a card is on its way, the letter arrives with different information, the call-centre agent cannot see the app's request, and the branch asks the customer to repeat everything. Those failures live in the gaps, and no screen owns a gap. A blueprint also makes visible the backstage causes — a system that does not sync, a policy that forces re-verification, an SLA nobody communicates — which are the actual sources of most of the poor rating.

**(b) Likely failure points.** **Loss of context at every handoff** — the customer re-explains the situation to each channel, which is the single most common complaint in multi-channel service. **Inconsistent information** — the app's estimated arrival, the letter's wording, and the agent's script disagree, and the customer cannot tell which is true. **Status invisibility between events** — after the request and before the card arrives there is a silent gap, which is where anxiety and the inbound call both originate. **Repeated identity verification** across channels. **Dead ends** — the app can start the request but not change the delivery address, forcing a channel switch with no warning. **The ending** — the card arrives with no activation guidance, or activation fails and there is no clear route back. **The emotional peak** is usually early: the moment of realising the card is lost, when the customer needs immediate reassurance that spending is blocked and a replacement is coming.

**(c) Highest-leverage fix.** **Continuity of state across channels** — one status, visible to the customer and to every member of staff, updated proactively at each stage. It is highest-leverage for three reasons. It removes the re-explanation cost, which is the most-cited irritant and the one that makes customers feel unrecognised. It fills the silent gap with proactive status, which removes the anxiety peak *and* removes the inbound calls that gap generates, so it pays for itself operationally — a second-order effect worth quantifying for stakeholders. And under **Peak–End**, it improves both the worst moment (the panicked start, now answered with immediate confirmation that the card is blocked and a replacement is ordered) and the ending (a card that arrives when it was said to, with activation that works). Nothing else in this journey moves both the peak and the end for one piece of work.

*Marking:* strong answers name the blueprint and explain specifically what it reveals that screen testing cannot — the seams, and the backstage causes. They also connect the fix to a measurable operational benefit rather than to sentiment. Weak answers propose a journey map with no backstage layer and list generic touchpoint improvements.

**38.**
**(a) Reasoning errors.** First, **stretching a layout is not adapting it**: line length is a legibility constraint, and a full-width stretch produces 150-character measures that are genuinely hard to read, while the vertical single-column rhythm wastes the one thing desktop has and mobile does not — horizontal space for comparison and context. Second, **a top tab bar is not the desktop equivalent of a bottom tab bar**; the bottom bar exists because of the thumb arc, and on desktop the motor model is a mouse with Fitts's Law clamping at screen edges, so the constraint that produced the pattern no longer exists. Third, the plan **treats the difference as screen size when it is a difference in input, context, posture, and task**: pointer precision and hover, keyboard as a first-class input, multi-window and multi-tasking, longer sessions, and different intent — desktop users typically arrive to do the deeper, longer, more complex version of the task. Fourth, it ignores **Jakob's Law in the desktop context**: desktop users carry strong conventions of their own, and a phone layout on a monitor reads as unfinished rather than as consistent.

**(b) Adaptation decisions, by category.**
- **Layout**: constrain measure for reading content regardless of viewport; use the extra width for parallel information — list-plus-detail rather than list-then-detail, persistent filters, side-by-side comparison — rather than for bigger versions of the same thing.
- **Navigation**: a persistent left or top navigation that shows structure rather than hiding it; more items can be exposed because there is room and no thumb constraint. Preserve the same information architecture and labels across platforms even though the presentation differs — the model should be identical, the chrome should not.
- **Input**: keyboard shortcuts, tab order, hover affordances and tooltips, right-click context menus where appropriate, multi-select and drag with a single-pointer alternative (2.5.7). Never make hover the only route to a function.
- **Density and targets**: increase density moderately, but keep targets at least 24×24 CSS px (2.5.8); pointer precision permits smaller than touch, not tiny.
- **Interaction patterns**: replace bottom sheets and full-screen modal steps with inline panels, popovers, and side drawers; long flows can become fewer, denser screens because the working area supports it.
- **Content and states**: more can be shown, so empty states, errors, and help can be inline rather than pushed to separate screens; but re-check every state at the new size rather than assuming they scale.
- **Continuity**: state, drafts, and progress must carry across devices, because the same user will start on one and finish on the other.
- **Responsive integrity**: the layout must still satisfy 1.4.10 reflow at 320 CSS px equivalent and remain usable at 200% zoom — desktop is not an excuse to abandon that.

**(c) What to test first, and with whom.** First, an **IA and navigation check with a tree test**, because the biggest risk is that the mobile structure was shaped by mobile constraints and does not survive exposure — that is cheap to test and expensive to discover late. Then a **first-click test** on the new navigation. Then moderated usability sessions on the two or three tasks that are genuinely *different* on desktop — the long, complex, comparison-heavy ones — since those are where the stretched layout will fail and where a scaled-up mobile flow will feel most wrong. Recruit two groups deliberately: **existing mobile users**, to check that the model still matches what they learned and to detect change aversion (which is not the same as a bad design, and needs separating), and **desktop-first users with no history in the product**, to check the design stands on its own. Add a keyboard-only pass and a 200% zoom pass to the same sessions rather than treating them as a separate audit.

*Marking:* strong answers reframe the difference as input, context, and task rather than screen size, and keep the IA constant while changing the presentation. Weak answers list breakpoints and component swaps without explaining what actually differs about desktop use.

**39.**
**(a) What is wrong with the definition.** "Completed the product tour" measures compliance with our onboarding, not the user experiencing value — it is a **proxy for a proxy**. The 80%/12% gap is the definition failing loudly: the metric is nearly saturated and has no relationship to the outcome, which means it cannot guide any decision, and worse, it will reward optimisations that make the tour easier to finish while the product gets no better. A real activation definition names the **first moment the user experiences core value** and is chosen because it *predicts* retention: "sent a first message", "imported a first dataset", "completed a first transfer", "invited a teammate". I would derive it empirically — find the early behaviours that most sharply separate the day-30 retained cohort from the churned one, then choose the earliest, most-attributable one as the definition rather than picking it by intuition. Then validate it: users who hit it should retain markedly better than those who do not, and the difference should hold when controlling for obvious confounders such as channel and prior intent.

**(b) Causes and their distinct fixes.** Separate three populations, because they need entirely different work.
- **Cannot** — usability and technical failure. People who are trying and are blocked: a broken step, a confusing form, an unsupported browser, an integration that fails silently, a permissions wall. Fix with usability testing and funnel instrumentation at step level; these are design and engineering defects.
- **Will not** — the value is not clear, or the ask is too early. People who could complete the step but see no reason to, or who are asked for effort (connect your bank, invite your team, upload your data) before they have seen anything worth the effort. Fix by resequencing — deliver a visible win before the costly ask — by using sample data or a template to shortcut the empty state, and by making the payoff legible at the point of the ask. This is a Fogg ability-and-motivation problem: usually raise ability and reduce the ask, rather than exhorting harder.
- **Should not** — we acquired the wrong users. No onboarding change fixes this, and it is the cause teams most often miss while redesigning screens. Fix upstream: acquisition targeting, landing-page honesty about who the product is for, and qualification. Diagnose it by segmenting activation by channel and campaign — a channel whose users never activate is an acquisition problem wearing an onboarding costume.
Also worth naming: **should have but we cannot see it** — instrumentation gaps, where users did reach value through a path the events do not capture. Check this before concluding anything.

**(c) Cohort analysis and the result that changes the roadmap.** Build **cohort retention curves by join week, split by whether the cohort hit the candidate activation event**, and segment by acquisition channel, platform, and plan. The decisive question is whether the activated curve **flattens** — a flattening curve is the product-market-fit signal, meaning a durable group keeps returning; a curve declining toward zero even among activated users means the activation definition is still wrong or the product has no durable value, and no onboarding work will save it. Specific results and their consequences: if activated users retain far better and activation rate is low, the roadmap is onboarding and the path to first value. If activated users retain no better, stop the onboarding work and fix the definition or the product's core value — that would be the finding that changes the roadmap most, because it invalidates the entire premise. If activation and retention vary dramatically by channel, the roadmap item is acquisition, not design. I would also check involuntary churn separately, since failed payments masquerading as disengagement is a common and cheap win.

*Marking:* the strong answer rejects the proxy, derives the replacement empirically rather than asserting one, splits cannot/will not/should not, and names a result that would invalidate its own hypothesis. Weak answers propose a better tour.

**40.**
**(a) Behavioural analysis.** In the **Fogg Behaviour Model (B = MAP)**, the push notification is the **prompt**, the streak supplies **motivation**, and the daily action's **ability** cost determines whether the prompt converts. The design leans almost entirely on motivation, which is the expensive and least reliable lever — and the motivation it supplies is **loss aversion** rather than desire for the underlying benefit: the user is not being drawn toward value, they are being pushed away from a loss. In the **Hook Model**, the streak is **investment** — accumulated value that makes the next loop more likely and raises the cost of leaving — and the notification is the **external trigger**, with the intended endpoint being an internal trigger where the habit self-sustains. **Zeigarnik and Goal-Gradient** amplify it: an incomplete streak is an open loop, and the closer the number climbs to a milestone the stronger the pull. The specific mechanism at issue is the **loss-framed warning at the pause step**, which weaponises the accumulated investment against the user's own stated intention to stop — that is where behavioural design stops serving the user's goal and starts overriding it.

**(b) Ethical test, applied.** The test: **would this design still work if the user could see exactly how it works and why we built it?** And: does it help the user reach a goal *they already hold*, or a goal we hold on their behalf? Applied to each part. The **streak itself passes** — a user who has chosen to build a daily habit is served by a visible record of consistency; shown the mechanism, they would still want it. The **daily push notification is borderline**, and depends entirely on consent and control: opted-in, timed by the user, and easy to turn off, it supports the goal; defaulted on and unsuppressible, it serves our engagement metric. The **loss-framed warning at the pause step fails**. Pausing is a deliberate act by a user exercising control; interposing "you'll lose your 47-day streak" is designed to make them feel worse about a decision they have already made, which is **confirmshaming** applied at the exit — the same structure as a roadblock in a cancellation flow. It also converts a mechanic that was helping the user into one that punishes them for a life event, which is precisely the second-order effect that turns streaks into a source of anxiety. Conclusion: ship the streak, fix the pause, make the notification genuinely optional.

**(c) The version I would ship, and monitoring.** Keep the streak, and design it to survive real life: **streak freezes or rest days** built in, so a missed day is recoverable and the mechanic does not punish illness, travel, or a weekend; **forgiveness on the first miss**, because the abandonment cliff is at the first break, and a user who loses 47 days in one night usually never returns. Make **pausing frictionless and neutral** — "Pause for a week? Your streak is held" — which is honest, serves the user, and retains better than the coercive version. Make the **notification opt-in, user-scheduled, and adaptive**, with an easy off switch that does not delete the streak, and cap frequency. Frame the streak around the **benefit** ("you've read on 47 days") rather than the **threat** ("don't lose your streak"), so the motivation points at the value rather than at the loss. Monitor for harm, not just engagement: **notification opt-out and mute rates** and **app-level notification disabling**, which is the loudest possible negative signal; **behaviour after a break** — do users return or churn, which tells you whether the mechanic is supportive or punitive; **anxiety and pressure language** in reviews, support contacts, and survey free-text; **usage that looks like compliance rather than value** — sessions that hit the streak condition and end within seconds, which means we are producing a number rather than a habit; and **retention 30 days after a streak break**, which is the single sharpest test of whether the mechanic served the user or trapped them. Guardrail: engagement gains must not come with rising mute rates or falling post-break return rates.

*Marking:* strong answers separate the three components and reach different verdicts on each, rather than approving or condemning the whole mechanic; they apply the ethical test explicitly to the pause step; and they propose monitoring that could *detect harm*, not just confirm engagement. A weak answer says streaks are manipulative, or says they are fine because users like them, without a test or a monitoring plan.

---

## Scoring bands

| Score | Reading | What to do next |
| --- | --- | --- |
| **34–40** | Interview-ready on fundamentals | Stop studying concepts; start practising delivery |
| **27–33** | Solid, with specific gaps | Revise the modules your misses cluster in, then retake |
| **Under 27** | Foundations not yet secure | Re-run the per-module quizzes before retaking this |

**34–40.** You know the material. The remaining gap between this score and an offer is almost entirely **delivery**, not knowledge: whether you can produce these answers aloud, under time pressure, in a conversation where the interviewer interrupts. Move to mock interviews and record yourself; the gap between your written answer and your spoken one is the thing to close. Then work on your portfolio and case storytelling — at this level, interviews are lost on narrative structure and on failing to state trade-offs, not on recall. Practise saying the limitation of your own recommendation unprompted; it is the highest-signal move available and it is a habit, not a fact.

**27–33.** The foundation is real but uneven. Do not re-read everything — that is the least efficient possible response. Instead, use the table below to map every question you missed back to its module, and look for **clusters**: three misses in Module 09 is a research gap worth a week; three misses spread across nine modules is noise and needs nothing more than a second pass at the flashcards. Revise the clustered modules by testing first and reading second, then retake this exam.

**Under 27.** Retaking this exam now would measure the same gap again. Go back to the per-module quizzes in `modules/NN-*/quiz.md` and work through them in order, since each is scoped tightly enough to tell you exactly what is missing. Return here when you are consistently hitting the per-module targets.

### Map your misses

| Questions | Module |
| --- | --- |
| 1, 11, 12 | 01 Foundations |
| 2, 18, 25 | 02 Psychology & Cognition |
| 3, 13, 26, 27, 28 | 03 UX Laws |
| 4, 16, 25, 31 | 04 Gestalt |
| 5, 31, 36 | 05 Heuristics & Evaluation |
| 25, 31, 36, 38 | 06 Visual Design |
| 15, 20, 22, 26, 31 | 07 Interaction Design |
| 8, 29, 38 | 08 Information Architecture |
| 12, 19, 28, 30 | 09 Research |
| 6, 14, 31, 35, 38 | 10 Accessibility |
| 7, 21, 33 | 11 Design Systems |
| 9, 17, 30, 39 | 12 Metrics & Strategy |
| 10, 23, 24, 32, 34, 37, 40 | 13 Advanced Topics |

Several questions appear against more than one module, which is deliberate: the applied scenarios are cross-module by design, and that is what makes them the closest thing here to a real interview. If a scenario went badly, check which of its constituent modules you also missed in Parts A and B — that is usually the actual gap.

**Retesting.** Leave at least a week before retaking, and preferably two. Sitting it again within a day or two measures your memory of this answer key, not your knowledge of the material, and the score will flatter you badly. The interval is the point: retrieval after a delay is what builds durable recall, and a slightly harder second attempt is worth far more than an easy one.

---

<!-- nav -->
[← Previous: Mixed Exam 2 — Practice](mixed-exam-2.md) · [↑ Quizzes](README.md) · [Next: Flashcards →](flashcards.md)
