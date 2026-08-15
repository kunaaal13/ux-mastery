# Quiz — Module 09: Research

14 questions. Target: 10/14.

---

### Part A — Recall

**1.** A usability test is:
- a) attitudinal and generative
- b) behavioural and evaluative
- c) behavioural and generative
- d) attitudinal and evaluative

**2.** "Five users find 85% of usability problems" assumes:
- a) one homogeneous user group and iterative rounds
- b) any user population
- c) a quantitative benchmark study
- d) unmoderated testing only

**3.** Peeking at an A/B test means:
- a) looking at qualitative feedback first
- b) checking results repeatedly and stopping when significant
- c) segmenting after the fact
- d) running the test on internal users

**4.** SUS scores average around:
- a) 50
- b) 68
- c) 80
- d) 90

**5.** For a tree test you would typically recruit:
- a) 5
- b) 8–10
- c) 30–50
- d) 500+

**6.** The most reliable interview question form is:
- a) "Would you use a feature that…?"
- b) "How often do you usually…?"
- c) "Tell me about the last time you…"
- d) "How much would you pay for…?"

---

### Part B — Short answer

**7.** State the difference between attitudinal and behavioural data, and the rule that follows.

**8.** Give two things each that interviews, analytics, and A/B tests cannot tell you.

**9.** Name the five levels from observation to decision.

**10.** Give three guardrail metrics you would set for a checkout conversion experiment, and why each.

**11.** Why report "6 of 8 participants" rather than "75% of users"?

---

### Part C — Applied

**12.** A PM says: "Let's survey users to find out whether they want feature X." Respond with a better plan.

**13.** An A/B test shows a 6% lift in signups for a variant, but usability sessions show users are confused by the new copy. Walk through your decision process.

**14.** You have four weeks and need to decide whether to rebuild the onboarding. Design the research plan: methods, sequence, sample sizes, and what each answers.

---
---

## Solutions

**1. b)** Behavioural (you watch what people do) and evaluative (it assesses a design).

**2. a)** A single homogeneous user group, with iteration between rounds. It says nothing about distinct segments (budget five per segment), and it does not license proportion claims from five people.

**3. b)** Repeatedly checking and stopping at significance. It inflates false positives substantially, because with enough looks a random walk will cross the threshold. Fix: pre-commit to a duration and sample size, or use a sequential testing method designed for continuous monitoring.

**4. b)** ~68 is the average; 80+ is good.

**5. c)** 30–50 gives stable task-level success and directness figures. (Card sorts run 15–30; moderated usability tests 5–8 per segment.)

**6. c)** Asking for a concrete past episode. (a) and (d) are hypotheticals that overestimate intent; (b) asks for a summary the person will approximate badly.

---

**7.** **Attitudinal** = what people say (interviews, surveys); **behavioural** = what people do (usability tests, analytics, A/B tests). The rule: **weight behaviour over self-report when both are available**, because people misremember past behaviour, predict their future behaviour badly, and rationalise. Attitudinal data is still essential — it is the only source of *why* — but it should not be used to estimate what people will actually do.

**8.** Two each:
- **Interviews:** cannot tell you what people will actually do; cannot give accurate frequencies or prevalence.
- **Analytics:** cannot tell you why; cannot tell you anything about people who never arrived (or who churned before instrumentation), and cannot see intent behind an action.
- **A/B tests:** cannot tell you why the variant won; cannot measure long-horizon effects (trust, brand, months-later retention) within a normal test window, and cannot detect effects too small for the powered sample.

**9.** Observation → pattern → insight → recommendation → decision. Most reports stop at the **pattern** and are ignored; jumping straight to a recommendation without stating the insight makes it impossible for others to evaluate or generalise.

**10.** For a checkout conversion experiment, any three with reasoning:
- **Downstream completion or payment success rate** — a variant can raise "clicked pay" while lowering successful orders.
- **Refund/return or cancellation rate** — a lift bought by misleading users shows up here, and a change that raises orders while raising returns is a net loss.
- **Support-contact rate per order** — confusion converted into cost.
- **Error rate and latency** — a technically slower variant can win short-term while degrading the experience.
- **Revenue per visitor rather than conversion alone** — conversion can rise while average order value falls.
The principle: guardrails exist to catch a win that is actually a transfer of cost elsewhere.

**11.** Because a percentage implies generalisation to a population, and a sample of eight supports no such inference — the confidence interval around 75% from n=8 is enormous. "6 of 8" communicates both the frequency and the sample size honestly, keeps the reader calibrated, and prevents the number from being quoted downstream as a population statistic. It also correctly signals that qualitative studies estimate *existence* and *mechanism*, not prevalence.

**12.** Better plan and the reasoning:
- **Name the problem with the survey:** asking people whether they want a feature is a hypothetical attitudinal question; it reliably overestimates interest, because saying yes is free and respondents are agreeable and self-selected. It also cannot tell us whether the underlying need exists.
- **Reframe the question:** the real questions are (a) does the underlying problem exist and matter, (b) how are people solving it today, and (c) would they actually adopt it.
- **Plan:**
  1. **Existing evidence first** — support tickets, search logs, sales-call notes, and analytics for workaround behaviour. Free and immediate.
  2. **6–10 interviews per segment** asking about the last time they faced the problem and what they did instead — the workaround is the strongest evidence of real demand.
  3. **A behavioural demand test** — a fake-door or concept test measuring actual click-through and follow-through, or a smoke-test landing page. This measures behaviour, not stated intent.
  4. **Survey last, if at all** — once we know the vocabulary and the segments, a survey can size the prevalence of the *problem* (behavioural questions: "how many times last month did you…"), which is a question surveys can answer.
- **What I would tell the PM:** "Surveys are good at sizing something we already understand; they are bad at deciding whether to build something. Let's use it for sizing after we know what we are sizing."

**13.** Decision process:
1. **Validate the test itself** — was it powered and pre-registered, did it run at least a full weekly cycle, was there peeking, are the traffic splits balanced, and is the population representative (not, say, only new users)?
2. **Check guardrails and downstream metrics** — signups are an intermediate metric. Look at activation, first-value completion, day-7/day-30 retention of the new signups, support contacts, and any refund or cancellation signal. A lift in signups from confusing copy often produces lower-quality signups that churn, which is a loss disguised as a win.
3. **Read the qual for mechanism.** Confusion has two flavours: *unfamiliarity* (transient, resolves as users learn — consistent with change aversion) or *misunderstanding of what they are agreeing to* (persistent and harmful). The sessions should tell me which; if participants signed up while holding a false belief about what they were getting, the lift is extracted from a misunderstanding.
4. **Decide by the mechanism:**
   - If the copy misleads → do not ship, regardless of the lift. State it plainly: the metric moved because users were wrong about the offer, and that cost lands in retention and support.
   - If it is merely unfamiliar and downstream metrics hold → ship, monitor retention by cohort for several weeks, and fix the copy clarity separately since clarity should not cost us the lift.
   - If downstream metrics are unavailable → that is the real problem; instrument them before making this call, and hold the decision if the risk is material.
5. **Communicate:** "the quant tells me the size, the qual tells me the mechanism, and the mechanism decides whether the size is real."

**14.** Four-week plan to decide on an onboarding rebuild:
- **Week 1 — Frame and use what exists (cheap, fast).**
  - Funnel analysis of the current onboarding, segmented by platform, geography, and acquisition channel; identify where drop-off concentrates. *Answers: where and how big.*
  - Cohort retention comparison between users who complete onboarding and those who do not. *Answers: does onboarding completion even correlate with the outcome we care about.*
  - Support tickets and app-store reviews mined for onboarding themes; session recordings of 20 drop-offs. *Answers: candidate causes.*
  - Deliverable: a problem statement and a hypothesis, plus a decision about whether the problem is worth four weeks.
- **Week 2 — Understand why (qual, generative).**
  - 8 interviews with recent signups (4 who completed, 4 who dropped), asking about the actual episode. *Answers: motivation, context, expectations, and what they thought the product was for.*
  - 6–8 moderated usability sessions on the current onboarding, split across segments. *Answers: specific failure points with severity ratings.*
  - Deliverable: severity-rated problem list plus insights — separating "the flow is broken" from "we attract the wrong users" from "the value is not clear before the ask."
- **Week 3 — Design and test candidates (evaluative, cheap).**
  - Two or three concepts at mid fidelity, driven by the insights; if the diagnosis is structural, one concept should defer or remove steps rather than polish them.
  - 5–8 moderated sessions per concept (or one concept in two rounds of 5, iterating between). *Answers: does the new flow work.*
  - First-click test on the entry screen with 20–30 people. *Answers: does the start point read correctly.*
  - Deliverable: a validated direction with known remaining risks.
- **Week 4 — Size the bet and plan measurement.**
  - Estimate impact: apply the observed failure rates to the funnel to project a plausible range, and state the assumptions explicitly.
  - Define the launch experiment: primary metric (activation, not signups), guardrails (retention, support contacts, quality of signups), the powered sample size, and the run duration.
  - Deliverable: a recommendation — rebuild, targeted fixes, or neither — with the evidence, the cost estimate from engineering, and the measurement plan.
- **Stated limits:** four weeks cannot measure long-term retention effects; the interview sample will under-represent users who churned long ago and anyone using assistive technology unless deliberately recruited; and analytics only describes users who arrived, so it says nothing about the acquisition mismatch that may be the real cause.
