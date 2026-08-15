# Quiz — Module 01: Foundations

12 questions. Answer before scrolling. Target: 9/12 to move on.

---

### Part A — Recall (multiple choice)

**1.** According to ISO 9241-210, user experience includes a person's responses:
- a) during use only
- b) during and after use
- c) before, during, and after use
- d) only when the product is working correctly

**2.** In the Double Diamond, the *second* diamond explores:
- a) the problem space
- b) the solution space
- c) stakeholder alignment
- d) delivery timelines

**3.** Nielsen's five usability components are learnability, efficiency, memorability, errors, and:
- a) accessibility
- b) desirability
- c) satisfaction
- d) findability

**4.** An average SUS score is approximately:
- a) 50
- b) 68
- c) 75
- d) 90

**5.** Which statement is a Job-to-be-done rather than a persona?
- a) "Priya, 32, product manager, values control"
- b) "Power users want more keyboard shortcuts"
- c) "When I am commuting with my hands busy, help me capture a thought before I lose it"
- d) "Users aged 25–34 in urban India"

---

### Part B — Short answer

**6.** Give a one-sentence distinction between UX and UI that does not use the words "look" or "feel."

**7.** Name two components of an experience that a designer does not draw but strongly influences.

**8.** Write a Lean UX hypothesis for adding dark mode to a reading app, using the template `We believe that… for… will achieve… We will know we are right when…`.

**9.** Which fidelity would you use to test whether the *order of steps* in a checkout flow works, and why not go higher?

---

### Part C — Applied

**10.** A PM says: "Users are complaining the transfer screen is confusing — redesign it." What are the first three things you do, and what would make you conclude the screen is *not* the problem?

**11.** A feature passes usability testing (95% task success) but has 2% adoption after a month. Structure your diagnosis.

**12.** You have one week and no research budget for a new onboarding flow. Describe the process you would actually run, and name what you are knowingly giving up.

---
---

## Answers

**1. c)** Before, during, and after use — anticipation and memory are both part of the experience.

**2. b)** The solution space. The first diamond (Discover/Define) is the problem space; the second (Develop/Deliver) is the solution space.

**3. c)** Satisfaction.

**4. b)** ~68. Above 80 is considered good; below 50 is poor.

**5. c)** A JTBD is anchored in a *situation* and desired progress, not demographics or feature requests.

**6.** Model answer: "UI is the surface I hand to engineering; UX is the decision about what surface should exist, in what order, and what happens when it fails." Any answer that puts UI as a subset of the decisions UX covers is correct.

**7.** Any two of: latency and performance, pricing and plan structure, support and refund policy, notification and email cadence, onboarding sequencing, data model constraints, error and downtime behaviour, permissions requested by the platform.

**8.** Model answer: "We believe that adding a dark mode for readers who use the app at night will achieve longer evening sessions and fewer complaints about eye strain. We will know we are right when evening session length rises by at least 10% and dark mode is enabled by more than 25% of nightly active readers within four weeks."
Marking: the hypothesis must name a *measurable signal*, not "users will like it."

**9.** Low fidelity — paper or grey-box wireframes, or even a numbered list of steps. Higher fidelity invites feedback about colour, type, and brand, which is noise for a sequencing question, and it makes you reluctant to throw the work away.

**10.** Model answer:
- Look at the funnel data to find where people actually drop, and whether it is the screen or the step before it.
- Read the complaint verbatims and support tickets to find the users' own words.
- Watch 3–5 session recordings or run 5 quick usability sessions on the current screen.
Conclusion that the screen is not the problem: task success in testing is high, drop-off concentrates *before* the screen, and complaints cluster around something the screen cannot fix — for example not knowing the payee's account number, or not trusting the transfer limit. Reframe the problem statement before designing.

**11.** Model structure — separate the funnel:
1. **Awareness** — entry-point impressions; do users ever see it?
2. **Comprehension** — does the label communicate the value? Test the copy, not the flow.
3. **Motivation** — do they want the outcome at all? Interviews and a fake-door test answer this; usability tests cannot.
4. **Ability** — validated already by the 95% success rate.
5. **Trigger** — is there a moment in the user's day that prompts use, and does the product create it?
State explicitly: usability testing only proved step 4, so the failure is upstream.

**12.** Model answer:
- Day 1: proxy research — support tickets, app-store reviews, session recordings, and a 30-minute call with two support agents and one salesperson.
- Day 2: funnel analysis of the current onboarding; write one framed problem statement.
- Day 3: sketch three concepts at different ambition levels; review with engineering for cost.
- Day 4: mid-fi prototype of the chosen concept with real content.
- Day 5: five guerrilla usability sessions; fix the top two issues.
- Ship behind a flag with an instrumented funnel and a defined success metric.
Knowingly given up: any confidence about *why* users churn beyond the flow itself, segment differences, longitudinal effects, and accessibility validation with assistive-technology users. Say so out loud — naming the trade-off is the point of the question.
