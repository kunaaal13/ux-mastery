# App Critique

## In one line

The critique round is not a test of taste — it is a test of whether you can perceive a screen systematically, name what you perceive in professional vocabulary, and rank problems by consequence rather than by how much they annoy you.

## What is actually being tested

Interviewers are watching for five things, roughly in this order of weight:

| Signal | What it looks like when present | What it looks like when absent |
| --- | --- | --- |
| **Framing before judging** | You state who the user is, what the primary task is, and what the business needs, before saying anything is wrong | You open with "the button colour is odd" |
| **Structured perception** | You move through the screen in a deliberate order and can say *why* your eye went where it went | You bounce randomly and repeat yourself |
| **Vocabulary** | Gestalt, hierarchy, affordance, heuristic, severity — used correctly and sparingly | Either no vocabulary at all, or a shower of jargon used decoratively |
| **Prioritisation** | Three ranked problems with severity and reasoning about frequency and impact | A flat list of twenty things |
| **Epistemic honesty** | You separate "this is a fact about the interface" from "this is a hypothesis about behaviour" and say what you would validate | Everything asserted with equal confidence |

The commonest failure is not being wrong. It is being unstructured — producing thirty accurate observations in no order, which reads as junior no matter how accurate each one is.

The second commonest failure is inventing a user. If you critique a dense enterprise dashboard as though it were a consumer app, every finding is technically true and strategically worthless. Density is a *feature* for an analyst who lives in a tool eight hours a day (Module 07).

## The 20-minute structure

This expands the format introduced in Module 05, with what to actually say at each stage.

| Minutes | Stage | What you do | What you say out loud |
| --- | --- | --- | --- |
| 0–2 | **Frame** | Establish user, task, context, business goal — as assumptions if you are not told | "I am going to assume this is for a first-time user on a phone, on mobile data, trying to complete a single order. Tell me if that is wrong." |
| 2–5 | **Happy path** | Walk the primary task as a first-timer, narrating perception before judgement | "My eye lands here first because it is the largest, warmest element. I expect it to be the primary action. It is actually a promotion." |
| 5–12 | **Edges** | Empty, error, loading, long content, offline, small screen, accessibility | "I want to see what happens when the address is not serviceable, because that is where I would expect this flow to fall apart." |
| 12–16 | **Categorise** | Group findings by heuristic, rate severity 0–4 | "That is a #1 visibility of system status issue, severity 3 — it happens on every order, and there is no recovery." |
| 16–19 | **Prioritise and propose** | Top three, a fix for each, cheap version and right version | "If I had one sprint I would do the inline validation. If I had a quarter I would restructure the step model." |
| 19–20 | **Validate** | Name what you could not assess and what data would settle it | "I have no idea whether the promo carousel earns its position. I would look at tap-through against scroll depth before removing it." |

Two mechanical notes. First, **say the time structure out loud at the start** — "I will spend about five minutes on the main flow, then go after the edge states, then rank what I have found." Interviewers relax immediately, because they now know you are not going to ramble. Second, **keep a visible list**. On a shared screen, type findings into a text file as you go. It stops you repeating yourself and it makes the prioritisation step trivial.

## The vocabulary to narrate perception

Critique quality is mostly vocabulary quality. Without the words, you can only say "this feels cluttered". With them, you can say why, and a why is actionable.

### Layer 1 — What the eye does (Gestalt, Module 04)

| Term | Use it to say |
| --- | --- |
| **Proximity** | "These two controls are eight pixels apart and the label is twenty-four pixels above, so the label reads as belonging to the field above it, not below." |
| **Similarity** | "Three visually identical chips do three different kinds of thing — one filters, one navigates, one is a status. Similarity is promising a consistency the system does not have." |
| **Common region** | "The card boundary groups the price with the delivery time, which is the correct pairing. The rating sits outside it and floats." |
| **Continuity** | "The eye follows the left edge down the list, so the right-aligned prices are read second, in a separate pass. That is fine for scanning, costly for comparison." |
| **Closure / figure-ground** | "The modal's scrim is too light, so the background competes and the dialogue does not read as the only live layer." |
| **Uniform connectedness** | "The stepper's segments are connected by a line, which correctly signals sequence." |

### Layer 2 — What the eye does first (hierarchy, Module 06)

Name the four variables that create hierarchy and say which one is doing the work: **size, weight, colour/contrast, and position/whitespace**. Then say whether the resulting order matches the task order.

The sentence pattern that lands: *"Visual hierarchy says X is most important; task hierarchy says Y is. They are fighting, and the interface is winning."*

Also carry: **scanning pattern** (F-pattern for text-dense, Z or layer-cake for structured), **contrast ratio**, **optical alignment**, **rhythm and spacing scale**, **density**, **anchor** (the element the eye returns to).

### Layer 3 — What the interface promises (interaction, Module 07)

| Term | Use it to say |
| --- | --- |
| **Affordance / signifier** | "The row is tappable but nothing signifies it — no chevron, no press state, no cursor change." |
| **Mapping** | "The left arrow moves the carousel right. The mapping is inverted." |
| **Feedback** | "There is no acknowledgement between tap and result, so on a slow connection I will tap twice." |
| **Constraint** | "The date picker allows past dates, which cannot be valid here — the constraint should be built in rather than validated after." |
| **State** | "This has a default, hover, focus, active, loading, disabled, error and success state to define, and I can see three of them." |
| **Mode** | "Edit and view look nearly identical, which is a mode error waiting to happen." |
| **Latency budget** | "Anything over about a second here needs a determinate progress indicator, not a spinner." |

### Layer 4 — What is wrong, formally (heuristics, Module 05)

Name the heuristic by number and phrase. Do not just say "usability issue".

| # | Heuristic | Typical critique-round sighting |
| --- | --- | --- |
| 1 | Visibility of system status | No feedback after submit; unclear which filters are active |
| 2 | Match with the real world | Internal jargon in user-facing labels ("SKU", "entity", "provision") |
| 3 | User control and freedom | No undo, no back, destructive action with no exit |
| 4 | Consistency and standards | Two different date formats; a non-standard back gesture |
| 5 | Error prevention | Free-text where a picker is possible; no confirmation on irreversible acts |
| 6 | Recognition over recall | Codes the user must remember between screens |
| 7 | Flexibility and efficiency | No saved addresses, no keyboard shortcuts in a power tool |
| 8 | Aesthetic and minimalist design | Six competing calls to action |
| 9 | Help users recover from errors | "Error 4012" with no next step |
| 10 | Help and documentation | Help exists but is not reachable from the point of failure |

### Layer 5 — How bad it is (severity)

Use Nielsen's 0–4 and say the reasoning, because severity without reasoning sounds arbitrary. Severity is **frequency × impact × persistence**, weighted by how central the task is.

> "I am calling that a 3 rather than a 4. It is on the main path and it is annoying, but it is recoverable in one tap and users learn it after the first order. A 4 for me is data loss, a dead end, or a revenue path that simply stops."

Being willing to *downgrade* your own finding is one of the strongest seniority signals available in this round.

## The edge states checklist

Most severe problems are not on the happy path. Run this list explicitly and out loud — interviewers score it.

| State | What to ask | Typical failure |
| --- | --- | --- |
| **Empty** | First run, no data, and zero-results-after-filter — three different states | A blank panel with no explanation or next action |
| **One item** | Does the layout survive a single row? | A grid designed for twelve looks broken with one |
| **Long content** | Long names, long addresses, three-line product titles, 24 tags | Truncation mid-word with no tooltip; broken alignment |
| **Loading** | Under 300 ms, 1 s, 10 s, and never | One spinner for all four; no skeleton; no timeout message |
| **Error** | Field-level, form-level, network, server, permission | Errors above the fold, form cleared, no field focus |
| **Offline / flaky** | What happens on a train | Silent failure; irreversible action fired twice |
| **Permission denied** | Camera, location, notifications refused | Dead end with no manual alternative |
| **Stale data** | Price changed, item sold out mid-flow | Failure only surfaces at payment |
| **Success** | Is the outcome confirmed and is there a next action? | Confirmation with nowhere to go |
| **Destructive** | Delete, cancel, remove | No confirmation, or confirmation with no undo |
| **Accessibility** | Keyboard order, focus visibility, target size, contrast, labels, dynamic type at 200% | Focus invisible; icon-only buttons unlabelled; 32 px targets |
| **Internationalisation** | Longer strings, RTL, currency, name order | Fixed-width buttons that break in German |
| **Small and large screens** | 320 px wide; tablet; a phone with a large accessibility font | Horizontal scroll; unreachable primary action |

You will not have time for all thirteen. Pick the five most likely to be load-bearing for the product in front of you and say why you picked them: *"For a checkout, I care most about error recovery, stale data, and offline, because those are where money leaks."*

## How to critique without sounding negative

The round is called a critique, but the interviewer is often hearing "how will this person talk about my team's work in a design review". Tone is a scored dimension even when nobody admits it.

Six habits that carry the tone:

1. **Separate observation from judgement.** "The primary action sits below the fold on a 667 px viewport" is an observation. "That is bad" is a judgement. State the observation, then the consequence, then let the judgement be obvious.
2. **Name the constraint you would have had.** "This is the shape you end up with when legal requires the disclosure inline — so the real question is where the disclosure goes, not whether it exists."
3. **Say what is working, specifically.** Generic praise is worthless; specific praise proves you are reading carefully. "The step indicator is honest — it shows three steps and there are three, which is rarer than it should be."
4. **Use the conditional for hypotheses.** "I would *expect* drop-off here" rather than "users drop off here". You do not have their data.
5. **Attack the artefact, never the imagined designer.** "This pattern breaks down at long addresses", not "whoever built this did not think about long addresses".
6. **Offer a cheap fix alongside the right fix.** Teams cannot always do the right fix. Showing you know that is a collaboration signal (Module 11).

The phrase to have ready when you genuinely think something is severely broken:

> "I want to be direct about this one, because I think it is the most expensive problem on the screen — and I might be missing a constraint that forced it, so tell me if I am."

That sentence lets you be blunt without being rude, and it invites the interviewer to give you information.

## When the interviewer built it

A common variant: "critique our own product." Sometimes the person across the table designed the screen you are looking at. This is a trap only if you handle it as a social problem rather than a professional one.

**What not to do:** soften into uselessness. "It is great, maybe the spacing could be slightly different" scores worse than anything you could say honestly. Interviewers read hedging as either dishonesty or an inability to see problems, and both are disqualifying.

**What to do:**

1. **Ask for the constraints first, sincerely.** "Before I start — is there anything about the history here I should know? Constraints, a rollout in progress, a platform limitation?" This is not flattery. It genuinely improves the critique, and it signals that you assume there were reasons.
2. **Lead with the strongest genuine positive, stated specifically.** One sentence, evidence-based, then move on.
3. **Frame findings as questions where you are uncertain and as statements where you are not.** "How did you land on putting verification before the first order? I would have expected it after, and I am curious what forced it" is collaborative. "Verification is in the wrong place" is not, when you do not know.
4. **Rank ruthlessly anyway.** The ranking is the deliverable. Do not blunt it.
5. **Expect the push-back and welcome it.** If they say "we tried that and it failed", the correct response is curiosity, not retreat: "That is useful — what did failure look like? If it failed on conversion rather than comprehension, that changes what I would try next."

The tell they are looking for: can you disagree with a senior person, hold your position when you have grounds, and change it when you are given new information. Both halves are scored. Candidates who never move look rigid; candidates who fold on the first push-back look unreliable.

If they push back on something where you are genuinely right and have grounds:

> "I hear that, and I would still rank it first — not because the pattern is unusual, but because it is on every order and there is no recovery path. If the data says users get through it fine, then I am wrong and I would want to see that. What does the funnel look like at that step?"

## Worked example one — mobile food-delivery checkout

*Transcript-style. Read it aloud once; the point is the rhythm, not the specific findings.*

---

"Let me frame first. I will assume this is a consumer food-delivery app, the user is on a phone, they are hungry, often one-handed, often on mobile data, and this is a repeat user rather than a first-timer — most orders in this category come from returning users. The business goal is order completion and average order value, and the operational goal is that the address and timing are correct so the delivery does not fail. Correct me if any of that is wrong.

**The happy path.** My eye lands first on the large green button at the bottom — good, that is the primary action and it has the strongest contrast and the largest area. It says 'Place order', which is honest. Second thing my eye catches is the yellow promo strip near the top, because yellow against this neutral background has more chroma contrast than anything else on the screen. So the second-strongest element on a checkout page is a promotion. That is a hierarchy inversion: visual hierarchy says the promo is second-most important, task hierarchy says the address and the total are.

Working down. The address block is at the top, in body-sized grey text with no label and no obvious tap affordance. There is a small chevron on the right. That chevron is the only signifier that this is editable. On a delivery product, delivering to the wrong address is the single most expensive failure mode — it is a refund, a redelivery, and a support contact. So the most consequential editable field on the screen is also the lowest-contrast, weakest-affordance element on the screen. That is my first candidate for the top three.

Below that, the item list. Proximity is doing good work here — quantity, name and price are tightly grouped per row with generous space between rows, so each row reads as one object. The quantity stepper is at the right edge, roughly 32 pixels square by eye. That is below the 44 pixel minimum, at the far edge of the screen, on a one-handed device. Two problems in one: target size and reach.

Then the price breakdown. Subtotal, delivery fee, taxes, and a line called 'Handling'. 'Handling' is unexplained — that is a #2 match-with-the-real-world issue, and in this category unexplained fees are a known driver of abandonment at the last step. There is no info affordance on it.

The total is set in the same weight and size as the line items above it. The one number the user is deciding on has no typographic emphasis. Small fix, real effect.

**Now the edges, which is where I expect the real problems.**

Address serviceability: what happens if the saved address is outside the delivery radius, or the restaurant has stopped delivering there since the last order? I would want to know whether that surfaces here or at the payment step. If it surfaces after payment authorisation, that is a catastrophe-class issue.

Stale cart: the restaurant runs out of an item while I am in checkout. Does the total silently change? Does the item vanish? If the price changes between the screen I am looking at and the charge that lands, that is both a trust failure and, in many markets, a compliance problem.

Payment failure: this is the one I care most about. If the card is declined, does the app keep the cart, keep the address, keep the tip, and return me to a state where I can pick a different method in one tap? Most implementations of this drop something. The fix is not a visual one — it is making sure the cart is server-side and the failure returns to a payment-method sheet rather than to the cart.

Offline: I tap 'Place order' on a lift and the request hangs. Two risks. One, no feedback, so I tap again and place two orders — that is an error-prevention failure with a financial consequence. Two, the app tells me it failed when the server actually accepted it. The button should disable and enter a loading state on first tap, and the order should carry an idempotency key so a retry cannot double-charge. That last part is an engineering conversation, but it is a design consequence, so I would raise it.

Accessibility: the promo strip is yellow text on white, which I would bet is under 3:1, and the fee explanations are grey-on-white body text that is likely under 4.5:1. The stepper buttons are icon-only with no visible label, so I would want to check they carry accessible names. And at 200% dynamic type, a fixed-height bottom bar with a button in it usually clips.

**Findings, categorised and rated.**

| # | Finding | Heuristic | Severity | Reasoning |
| --- | --- | --- | --- | --- |
| 1 | Payment failure may lose cart, address or tip state | #3, #9 | 4 | Blocks a revenue path, unrecoverable in the moment, high frequency (declines are common) |
| 2 | No loading state on 'Place order'; double-submit possible offline | #1, #5 | 4 | Financial consequence, silent, user cannot detect it |
| 3 | Address is the lowest-affordance element on the screen | #6, signifiers | 3 | High cost per occurrence, moderate frequency, recoverable but only via support |
| 4 | Unexplained 'Handling' fee | #2, #10 | 3 | Occurs on every order, drives abandonment, cheap to fix |
| 5 | Total not typographically distinguished | Hierarchy | 2 | Every order, low individual impact |
| 6 | Quantity steppers below 44 px and edge-placed | #7, WCAG target size | 2 | Frequent, mildly frustrating, learnable |
| 7 | Promo strip outranks task-critical content visually | #8, hierarchy | 2 | Constant, but plausibly a deliberate commercial trade-off |
| 8 | Likely contrast failures on grey and yellow text | WCAG 1.4.3 | 3 | Affects a defined population on every screen |

**Top three prioritised fixes.**

One, **make payment failure non-destructive.** Cart and address held server-side, decline returns to a payment sheet with the previous method pre-selected and an explanation of the failure reason where the processor gives us one. Cheap version: preserve state and return to checkout rather than the cart. Right version: a dedicated recovery sheet with alternative methods surfaced.

Two, **give 'Place order' a real state machine** — disabled-with-spinner on tap, idempotency key on the request, an explicit timeout message at ten seconds with a 'check order status' path rather than a naked retry. This is severity 4 and cheap, so it is the highest priority-per-effort item on the list.

Three, **promote the address into a proper, labelled, obviously tappable block**, with the serviceability check run when checkout opens rather than at payment. Cheap version: label, contrast, and a visible edit control. Right version: move the serviceability and timing check to checkout entry so failures happen before the user has committed.

**What I would validate.** I am asserting a lot from a static screen. Specifically: I would want funnel data by step to see whether the address or the payment step actually loses people, because my ranking assumes payment. I would want the rate of declines and what happens after one — do those sessions recover in-session, or do they end? I would want support-ticket categories for wrong-address deliveries, since that is my whole argument for finding three. And I would want to watch five sessions of one-handed use, because my target-size claim is a measurement, but my reachability claim is a guess about how people hold the device. If the data contradicts me on the address, I would drop it to fourth and promote the fee explanation, which is cheaper anyway."

---

## Worked example two — desktop analytics dashboard

*Same structure, deliberately different posture: density is not automatically a problem here.*

---

"Framing. I will assume this is an internal or B2B analytics tool, the user is an analyst or an operations manager, they are on a large desktop screen, they use this daily rather than occasionally, and they are here to answer a specific question rather than to browse. The business goal is probably time-to-answer and reducing ad-hoc requests to the data team. That framing matters because it changes what counts as a problem: for this user, density is a feature and whitespace is a cost. I am not going to critique this for looking busy.

**Happy path.** My eye goes first to the top-left region, which is correct for a left-to-right, top-to-bottom scan of a structured layout — and the four KPI tiles are there, which is the right thing to put in the strongest position. But all four tiles are visually identical in weight, so I cannot tell which is the primary metric. If one of these is the north-star metric and three are supporting, similarity is flattening a hierarchy that should exist (Module 12).

Each tile has a number, a label, and a delta with an arrow. The delta arrows are green up and red down. Two problems: colour is the only channel carrying direction, which fails for a red-green colour-blind user, and 'up is good' is not universally true — if one of these tiles is 'Error rate' or 'Churn', then up is bad and green up is actively misleading. I would want an explicit good/bad semantic, not a directional one.

The deltas say '+12%'. Against what? There is a global date-range picker in the top right, and I cannot tell from here whether the comparison is the previous period, the same period last year, or a fixed baseline. That ambiguity is a #1 visibility-of-system-status problem, and on a dashboard, an unlabelled comparison is worse than no comparison, because it will be quoted in a meeting.

Below that, the main chart. It is a multi-series line with, I count, nine series and a legend on the right. Nine series exceeds what anyone can track; beyond about five, the chart becomes decorative. The legend is separated from the lines, so reading it costs a saccade and a colour match per series — that is a recognition-versus-recall problem (#6), solvable with direct labelling of the top few series and demoting the rest.

The filter bar sits above the chart. Filters appear to be applied — I can see a couple of controls with values — but I cannot tell at a glance which filters are active and which are at default, because active and inactive states look nearly identical. On a dashboard, a filter you forgot you applied is the single most common source of a wrong decision. That is my leading candidate for the top three.

The table below is dense, which is fine. Column headers are the same weight as the cells, which is not — the header row should be structurally distinct so it survives scrolling. I cannot tell whether the header sticks on scroll. If it does not, this table is unreadable past twenty rows.

Numbers in the table are left-aligned and appear to be proportional-width. Numeric columns should be right-aligned and tabular so digits line up and magnitudes are comparable at a glance. That is a small typographic fix with a genuine cognitive payoff for the exact task this tool exists for.

**Edges.**

Empty and zero-results: on a dashboard, there are three different empties — no data yet because the pipeline is new, no data because the filter excludes everything, and no data because something broke. They need different messages, and the third one needs to be unmistakable. A dashboard that renders zeros when the pipeline failed will get a decision made on a false number. That is severity 4 in an analytics product and it has nothing to do with visual design.

Loading: with nine series and a wide date range, this query is slow. Is there a skeleton per widget, or does the whole page block? Per-widget loading is strongly better here because the KPI tiles will resolve first and often answer the question alone. And is there any indication of *data freshness* — 'as of 09:14' — because for an operational dashboard, staleness is the failure mode people get burned by.

Long content: dimension values in that table will include long, ugly machine-generated names. Truncation with no tooltip and no way to see the full value would make several rows useless.

Export and share: analysts do not live in the dashboard, they take things out of it. Is there a copy-link-with-current-filters? If the URL does not encode the filter state, every share is wrong, and this is the highest-value, lowest-cost feature on this list.

Accessibility and ergonomics: keyboard access to the filter bar and the table, focus visibility on a dark-ish theme, and a check that the series palette is distinguishable without colour. Also, at this density, target sizes will be small — acceptable for a mouse-driven expert tool, but the interactive rows still need a visible hover and focus state.

**Findings and severity.**

| # | Finding | Heuristic | Severity | Reasoning |
| --- | --- | --- | --- | --- |
| 1 | Failed-pipeline state indistinguishable from genuine zeros | #1, #9 | 4 | Produces confidently wrong decisions; invisible to the user |
| 2 | Active filters not visually distinct from defaults | #1, #6 | 4 | High frequency, silent, causes wrong answers |
| 3 | Comparison basis of deltas unlabelled | #1, #2 | 3 | Every view, gets quoted externally, cheap to fix |
| 4 | Nine series with detached legend | #8, #6 | 3 | Main chart is the centrepiece and is unreadable |
| 5 | Direction encoded only by colour, semantics assumed | WCAG 1.4.1, #4 | 3 | Excludes a known population, misleads on inverse metrics |
| 6 | Numeric columns left-aligned, non-tabular figures | Hierarchy, #7 | 2 | Constant low-grade cost to the core task |
| 7 | KPI tiles have no internal hierarchy | Hierarchy | 2 | Slows orientation, easy to fix |
| 8 | Filter state likely not in the URL | #7 | 3 | Breaks the dominant sharing workflow |
| 9 | No visible data-freshness timestamp | #1 | 3 | Staleness is the classic operational-dashboard failure |

**Top three.**

One, **make data trustworthiness visible**: an explicit freshness timestamp, and a distinct, loud state for pipeline failure that never renders as zero. Cheap version: a banner and a timestamp. Right version: per-widget health, with the widget refusing to draw when its source is stale beyond a threshold.

Two, **make filter state legible and portable**: active filters rendered as removable chips in a fixed region with a count and a 'clear all', and the full filter state encoded in the URL so a shared link reproduces the view. These are the same problem viewed from inside and outside the session.

Three, **fix the main chart's readability**: cap the default to the top five series with the rest collapsed into 'other', direct-label the visible series at their line ends, and label the comparison basis on the deltas. Cheap version: direct labels and a 'top five' default. Right version: let the user pin series, and remember the pinning.

**What I would validate.** I am guessing at the primary question this dashboard answers, and that guess drives my whole ranking. I would sit with three analysts and watch them answer one real question each, timing to first answer and counting how many times they scroll back to check a filter. I would look at which widgets are actually interacted with — dashboards accumulate widgets nobody has used in a year, and removal is usually the highest-value change available. And I would check the share/export logs, because if nobody shares links, my point about URL state is worth much less than I am claiming."

---

## Fifteen practice targets

Product categories rather than named products, so the practice stays about method. For each: run the 20-minute structure, write the findings table, and force yourself to a ranked top three.

| # | Target | Look hardest at |
| --- | --- | --- |
| 1 | Mobile banking transfer flow | Error prevention and recovery; confirmation before irreversible action; how a beneficiary is identified and re-verified; timeouts mid-transfer |
| 2 | Ride-hailing booking screen | State visibility during matching; cancellation policy legibility; map-versus-controls hierarchy; what happens when no driver is found |
| 3 | Airline seat selection | Density and legend legibility; disabled-versus-unavailable-versus-premium distinction; price changes on selection; small-screen reachability |
| 4 | Hotel search results | Filter state visibility; comparison across cards; price display honesty (total versus nightly); empty results after over-filtering |
| 5 | Government form (tax, licence, permit) | Plain language; progressive disclosure; save-and-resume; error recovery; documentation of what you need before you start |
| 6 | Streaming service home screen | Hierarchy across rows; recall burden of "where was I"; search versus browse; the cost of infinite content with no state |
| 7 | Enterprise CRM record page | Information architecture (Module 08); field density; edit-versus-view mode clarity; keyboard efficiency for daily users |
| 8 | Fitness or habit tracker | Onboarding-to-first-value time; streak mechanics and what breaking one feels like; empty state on day zero; notification design |
| 9 | E-commerce product detail page | Decision support (size, fit, returns); image versus specification hierarchy; review credibility; delivery promise visibility |
| 10 | Cloud console (compute or storage) | Destructive-action safeguards; naming and jargon (#2); the cost of a mis-click; discoverability of settings; error message quality |
| 11 | Video-call joining flow | Pre-flight device checks; permission denial handling; the guest-versus-account fork; what a bad connection looks like |
| 12 | Food-ordering restaurant menu | Scanability of a long list; customisation flows; dietary filtering; how an unavailable item is presented |
| 13 | Password reset and account recovery | The full failure tree; email deliverability messaging; what a locked-out user with no phone access can do; security-versus-usability trade-off |
| 14 | Kids' or education app | Age-appropriate targets and language; parental gates; interruption and resume; reward design and its ethics |
| 15 | Healthcare appointment booking | Anxiety-aware tone; clarity of what happens next; slot availability communication; accessibility for older adults and assistive tech |

Two suggested drills. **The five-minute version:** frame, one severity-4 finding, one cheap fix, one thing you would validate — useful because the compression forces prioritisation. **The blind edge-state drill:** without touching the happy path, go straight to error, empty and offline and see whether you can produce three severity-3-or-above findings. If you cannot, you are still critiquing surfaces.

## Check yourself

1. Name the six stages of the 20-minute critique and the one candidates most often skip.
2. Give the three factors that determine severity, and write a sentence downgrading one of your own findings.
3. List eight edge states and say which five you would prioritise for a checkout, with reasoning.
4. Rewrite "this screen is cluttered" three times using vocabulary from layers 1, 2 and 4.
5. What are the two failure modes when critiquing a product the interviewer built, and what is the opening question that defuses both?
6. For a critique you have just done, state which of your findings are facts about the interface and which are hypotheses about behaviour.

---

<!-- nav -->
[← Previous: Case Study Structure](../frameworks/case-study-structure.md) · [↑ Interview Prep](../README.md) · [Next: Design Challenge →](design-challenge.md)
