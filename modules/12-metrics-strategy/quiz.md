# Quiz — Module 12: Metrics & Strategy

12 questions. Target: 9/12.

---

### Part A — Recall

**1.** HEART stands for Happiness, Engagement, Adoption, Retention, and:
- a) Revenue
- b) Task success
- c) Trust
- d) Time on task

**2.** In AARRR, the stage where design typically has the most leverage is:
- a) Acquisition
- b) Activation
- c) Revenue
- d) Referral

**3.** A retention curve that flattens indicates:
- a) a measurement error
- b) a cohort that keeps returning — a product-market fit signal
- c) users are churning faster
- d) seasonality

**4.** In Kano terms, a feature that causes severe dissatisfaction when missing but no satisfaction when present is:
- a) a delight attribute
- b) a performance attribute
- c) a basic expectation
- d) an indifferent attribute

**5.** RICE stands for Reach, Impact, Confidence, and:
- a) Engagement
- b) Effort
- c) Efficiency
- d) Execution

---

### Part B — Short answer

**6.** Write the Goals → Signals → Metrics chain for a password-reset flow.

**7.** Give the three questions to ask before adopting any metric.

**8.** Give three primary metrics with their natural counter-metrics.

**9.** State the four-link chain connecting a design change to a business outcome, with an example.

**10.** Give the three-way split for diagnosing low activation, and say which one teams most often miss.

---

### Part C — Applied

**11.** Your team ships a redesigned onboarding. Signups rise 12%, but day-30 retention of that cohort falls. What is likely happening, and what would you do?

**12.** An executive asks: "What is the ROI of the design work we did this quarter?" You have no revenue attribution. Answer them.

---
---

## Solutions

**1. b)** Task success.

**2. b)** Activation — reaching first value. Acquisition is largely marketing's lever; activation is where onboarding, clarity, and friction removal pay off directly.

**3. b)** A flattening curve means a stable core of users keeps returning — the standard product-market fit signal. A curve declining toward zero means no durable value, and acquiring more users into it just leaks faster.

**4. c)** A basic expectation. Delight attributes create disproportionate satisfaction when present but are not missed when absent, and they decay into basics over time.

**5. b)** Effort — score is Reach × Impact × Confidence ÷ Effort.

---

**6.** Example chain:
- **Goal:** users who cannot sign in can regain access quickly and without contacting support.
- **Signals:** they complete the reset in one attempt; they do not open a support ticket; they successfully sign in afterwards and stay signed in; they do not request a second reset shortly after.
- **Metrics:** reset-flow completion rate; median time from request to successful sign-in; support contacts about access per 1,000 reset attempts; repeat-reset rate within 7 days (a guardrail — completing the flow but immediately needing it again means the reset did not really work).
Marking note: a strong answer includes a guardrail and defines success as *signing in*, not as *finishing the form*.

**7.** (1) Would a change in this number change what we do? If not, it is reporting, not measurement. (2) What would make this number improve for a bad reason? Name the perverse path before committing. (3) Who is excluded from this number? Analytics sees only people who arrived and whose events fired — anyone blocked earlier is invisible.

**8.** Any three pairs:
- Conversion rate ↔ refund/return/chargeback rate (and revenue per visitor, since conversion can rise while order value falls).
- Engagement / time in product ↔ task success or satisfaction (more time can mean confusion).
- Speed of a flow ↔ error rate and downstream correction rate (faster failure is not improvement).
- Signup volume ↔ activation and retention of that cohort (volume bought with unclear promises churns).
- Support-ticket deflection ↔ resolution rate and repeat-contact rate (deflection can just mean people gave up).

**9.** Chain: **design change → behaviour change → funnel-step change → business outcome.**
Example: moving identity verification from before signup to after first value → fewer users abandon at the verification step → activation rises from 20% to 28% → at current traffic and ARPU that is roughly N additional retained users at day 30, worth approximately ₹Y annually.
Marking note: full credit requires stating the assumptions and a confidence range rather than a single confident number.

**10.** **Cannot** (usability or technical failures block them), **will not** (the value is not clear, or we ask for too much too early), **should not** (we acquired the wrong users — a mismatch between the promise made in acquisition and the product). Teams most often miss **should not**, and instead redesign onboarding repeatedly for users who were never going to activate; the fix there is upstream in targeting and messaging, not in the flow.

**11.** Likely explanation: the redesign increased signups by attracting or persuading users who were not a good fit, or by making a promise the product does not keep — a classic case of optimising an intermediate metric at the expense of the real one. Other candidates: the new flow defers something that previously self-selected serious users; the cohort mix shifted because a marketing change coincided; or the tracking definition of activation changed.
What I would do:
1. **Check attribution and mix** — is the extra 12% concentrated in a channel, geography, or device? Compare like-for-like segments between cohorts before concluding anything.
2. **Compare activation, not just signups** — did the extra signups reach first value? If signups rose and activation rate fell proportionally, we added people who never got value.
3. **Look at what the flow now promises** — read the new copy against what the product delivers. If the lift came from a vaguer or more enticing claim, retention is where that bill arrives.
4. **Talk to 6–8 churned users from the new cohort** about what they expected.
5. **Decide by value, not by the intermediate metric:** if net retained users at day 30 is lower, the redesign is a regression despite the headline number, and I would say so plainly. Fix the promise or reinstate the qualifying friction; ship as an experiment with retention as the primary metric this time.
6. **Change the measurement plan** — signups should never have been the primary metric; activation and day-30 retention should be, with signups as a supporting number.

**12.** Answer:
- **Reframe from ROI to evidence, honestly.** "I cannot give you a revenue-attributed figure, because we do not have the attribution set up — and a made-up number is worse than none. What I can give you is what changed, measured, plus a cost-side calculation that is defensible."
- **Cost-side numbers, which are usually available:** support contacts per 1,000 users on the topics we addressed (before vs after); failed-transaction and error rates; time-to-completion on the core task multiplied by the number of internal staff performing it and their loaded hourly cost, for any internal tooling work; refunds or returns tied to the flows we changed; and onboarding/training time for new staff.
- **Behavioural evidence with a stated chain:** funnel-step conversion before and after, activation rate change, and task-success benchmarks from usability testing — with assumptions and confidence stated, not a false-precision revenue figure.
- **What I would ask for:** "The reason I cannot answer the revenue question is measurable and fixable. I would like event instrumentation and an agreed activation definition before the next quarter's work, plus one experiment per major project, so next quarter I can answer this properly." Turning the question into a measurement commitment is the strongest available response.
- **What I would avoid:** claiming credit for a metric that moved during the same period without isolating the change, and quoting a satisfaction score as if it were ROI.

---

<!-- nav -->
[← Previous: 12.3 Design Strategy](12.3-design-strategy.md) · [↑ Module 12 — Metrics & Strategy](README.md) · [Next: Module 13 — Advanced Topics →](../13-advanced/README.md)
