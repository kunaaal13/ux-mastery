# Quiz — Module 13: Advanced Topics

12 questions. Target: 9/12.

---

### Part A — Recall

**1.** In the Fogg Behaviour Model, behaviour requires:
- a) motivation and ability
- b) motivation, ability, and a prompt
- c) a trigger and a reward
- d) habit and investment

**2.** The Hook Model's four stages are trigger, action, variable reward, and:
- a) retention
- b) investment
- c) habit
- d) reinforcement

**3.** Which is a "roach motel" dark pattern?
- a) hidden fees at checkout
- b) easy to subscribe, hard to cancel
- c) a guilt-laden decline option
- d) a fake countdown timer

**4.** In AI interfaces, the goal for trust is:
- a) maximum trust
- b) calibrated trust
- c) minimum trust
- d) trust proportional to accuracy claims

**5.** In a service blueprint, the line of visibility separates:
- a) user actions from frontstage actions
- b) frontstage from backstage actions
- c) backstage from support processes
- d) physical evidence from user actions

---

### Part B — Short answer

**6.** State the three-question ethical test for behavioural mechanisms.

**7.** Name six dark patterns and one regulation that addresses deceptive design.

**8.** Give the two assumptions of classical UI design that generative AI breaks, and one design consequence of each.

**9.** Give five things that break when a product moves to a new locale.

**10.** Give four second-order questions to ask before shipping a change.

---

### Part C — Applied

**11.** Growth asks you to add a fabricated "only 2 left in stock" badge, citing a competitor. Respond with what you would do and say.

**12.** You are asked to add an AI assistant to a banking app. Outline your approach, including where you would and would not give it authority, and what you would measure.

---
---

## Solutions

**1. b)** Motivation, Ability, and a Prompt converging at the same moment. No prompt means no behaviour regardless of the other two.

**2. b)** Investment — what the user puts in, which increases the value of returning and raises switching cost.

**3. b)** Easy in, hard out.

**4. b)** Calibrated trust — trust proportional to actual reliability. Over-trust produces unchecked errors; under-trust produces abandonment.

**5. b)** Frontstage (visible to the user) from backstage (not visible). The line of interaction sits above frontstage, separating user actions.

---

**6.** (1) **Whose goal does this serve** — the user's own goal, or only the business's at the user's expense? (2) **Would I be comfortable explaining exactly how it works** to the user? (3) **Is the reverse as easy as the forward** — cancelling as easy as subscribing, opting out as easy as opting in? Failing any one is the signal to stop, regardless of performance.

**7.** Six from: roach motel, sneak into basket, hidden costs/drip pricing, confirmshaming, misdirection, trick questions, forced continuity, privacy Zuckering, bait and switch, disguised ads, nagging, obstruction, preselection, false urgency/scarcity.
Regulations: the EU's GDPR (consent must be freely given, specific, informed, unambiguous — pre-ticked boxes fail) and the Digital Services Act (explicitly prohibits dark patterns on covered platforms); the US FTC's enforcement on negative-option billing and deceptive design; India's CCPA dark-pattern guidelines (2023) and the DPDP Act for consent.

**8.** (1) **Deterministic output** — the same input no longer produces the same result. Consequence: consistency cannot be relied on as a usability property, so the design must support verification and cheap retry/correction rather than assuming a stable mental model of behaviour. (2) **Finite, discoverable controls** — an open-ended input surface hides what the system can do. Consequence: capability communication becomes a primary design job (concrete examples, honest refusals that say what would work), because users cannot infer the boundary from the interface.
A third acceptable answer: errors used to be states; now they can be fluent and confident, so error *recognition* — provenance, sources, uncertainty — becomes a design requirement rather than a nicety.

**9.** Five from: text expansion (German/Finnish ~30% longer) breaking fixed-width layouts; RTL mirroring of layout, direction, and icons; name structures (mononyms, patronymics, multiple surnames, name order); address formats (postcode patterns, state/province presence); phone-number formats; date order ambiguity (DD/MM vs MM/DD) and number grouping (lakh/crore vs thousands); currency symbol position and decimal conventions; colour meanings (red/green financial conventions invert in parts of East Asia); icon and gesture meanings; payment methods (cards vs UPI vs wallets vs cash-on-delivery); connectivity, device capability, and data cost.

**10.** Four from: **Who else is affected** (support staff, moderators, sellers, admins, other household members)? **What behaviour does this incentivise** — how will it be gamed? **What happens at scale** — is a mild effect at n=1 a systemic harm at n=10m? **What happens when it fails**, including whole-channel failure, not just a request error? **What does this foreclose later** structurally? **What is the cost to the people downstream** — does this move work onto support or operations?

**11.** What I would do and say:
1. **Establish the fact first.** "Is the stock actually low?" If it is not, this is a false statement of fact to induce a purchase — which in most of our markets is a regulatory problem, not a design preference. In India the CCPA's dark-pattern guidelines name false urgency explicitly; the EU's DSA and consumer law cover it; the FTC has acted on it. That framing usually ends the discussion faster than an ethics argument, and it is accurate.
2. **Name the measurable business risk, not just the principle:** refunds and chargebacks, complaint and support volume, app-store and payment-provider policy exposure, and the brand cost when someone reloads the page and sees the number reset — which they will, and screenshot.
3. **Offer the honest version that serves the same goal:** show *real* inventory when it is genuinely low; show real demand signals ("18 people bought this today" — if true); show a genuine deadline (a real sale end); or improve the actual conversion levers — clearer value, better defaults, fewer steps, trust signals, and removing the friction that is really costing us.
4. **Propose the measurement that would catch harm:** if we ship any urgency mechanic, track refunds, cancellations, complaint rate, and repeat-purchase rate alongside conversion — a lift that raises returns is a loss.
5. **On "the competitor does it":** competitors ship untested and sometimes unlawful things; their doing it is evidence about their risk appetite, not about effectiveness. I would offer to test the honest variant against the current baseline instead.
6. **If overruled** on a fabricated claim, I would state the position once in writing with the regulatory citation and escalate through the appropriate channel. Not as a stand-off — I would keep working on everything else — but knowingly stating a false fact to users is the line where "disagree and commit" does not apply.

**12.** Approach to an AI assistant in a banking app:
- **Start with the job, not the interface.** Banking has a small set of high-frequency intents (balance and transactions, "why was I charged this", transfers, disputes, card controls, statements). For several of these the best design is not a chat box at all — it is better search, a smarter default, or an inline explanation on the transaction row. I would establish which intents genuinely benefit from open-ended interaction before building a conversational surface.
- **Authority by reversibility** — the deciding axis:
  - **Free to act:** read-only tasks — summarising spending, finding a transaction, explaining a fee, categorising, answering product questions with a source link.
  - **Suggest and confirm with a full preview:** anything that moves money or changes account state — transfers, standing orders, card freezes, limit changes. The preview must show the exact amount, recipient, and date, and confirmation must be an explicit user action, never inferred from conversation.
  - **Never autonomous:** payments to new payees, anything irreversible, closing accounts, disputes and legal declarations, and anything with a regulatory reporting consequence.
- **Trust and safety design:** cite sources for factual claims (which term, which statement line); express uncertainty rather than guessing; refuse clearly and say what *would* work; never fabricate a figure — for anything numeric, read from the system of record and show the provenance. A wrong balance stated fluently is a severity-4 failure.
- **Fraud and social-engineering risk** — specific to banking: the assistant must never ask for credentials or OTPs, must be resistant to prompt injection via transaction descriptions or payee names (which are attacker-controlled text), and must not be usable to enumerate account details after a session hijack. Step-up authentication before any state change.
- **Escape hatch:** an obvious route to the deterministic path (the normal transfer flow) and to a human, at every point — especially in disputes and fraud, where users are distressed and the cost of a wrong answer is high.
- **Accessibility and inclusion:** the assistant must not become the only way to do anything; plain language; full keyboard and screen-reader support; and it must work for users whose English is a second language, which is a large share of the customer base.
- **Memory and privacy:** legible, editable, deletable; minimal retention; clear disclosure of what is used for training, and consent that meets the applicable data-protection law.
- **Measurement:** task completion for the intents it targets and containment rate (resolved without a human), paired with hard guardrails — misinformation rate sampled by human review, escalation rate, complaint and dispute volume, failed or reversed transactions initiated through the assistant, and satisfaction of users who *did* escalate. I would treat the misinformation and reversed-transaction rates as launch blockers with pre-agreed thresholds, not as metrics to watch afterwards.
- **Rollout:** internal staff first, then a small cohort, read-only capabilities before transactional ones, with a kill switch.

---

<!-- nav -->
[← Previous: 13.5 Systems & Service Design](13.5-systems-and-service-design.md) · [↑ Module 13 — Advanced Topics](README.md) · [Next: Interview Prep →](../../interview-prep/README.md)
