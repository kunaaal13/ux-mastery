# Answering Frameworks

## In one line

A framework is not a script — it is a way of guaranteeing that the three things every interviewer scores (structure, reasoning, and evidence of consequence) actually appear in the eight minutes you have.

## Why frameworks at all

Interviewers are scoring under time pressure, usually against a rubric they have to fill in within ten minutes of you leaving the room. A candidate who rambles well is scored as "hard to read" — which converts to a no-hire far more often than a merely average candidate who was legible.

The trade-off is real and should be named: a framework used mechanically sounds robotic and caps you at a mid score. The point is to internalise the shape so thoroughly that you can improvise inside it. Use the framework to decide *what to say next*, never as a phrase to recite ("So, using the STAR framework, my situation was…" is a tell).

| Framework | Use for | Typical length |
| --- | --- | --- |
| STAR / STAR+L | Behavioural and experience questions | 2–4 min |
| CIRCLES | Product-design and "design an X" prompts | 30–45 min |
| Critique framework | "Critique this app / this screen" | 20–30 min |
| Whiteboard structure | Live app-design or portfolio deep-dive whiteboarding | 45 min |
| Three-beat process answer | "Walk me through your process" | 90 sec |

---

## STAR and STAR+L

### The shape

| Letter | Content | Share of airtime |
| --- | --- | --- |
| **S**ituation | Context needed to make the rest legible | 10% |
| **T**ask | What *you specifically* were responsible for | 15% |
| **A**ction | The decisions you made, in sequence, with reasoning | 50% |
| **R**esult | What changed, with a number or a concrete observable | 25% |
| **L**earning | What you would do differently, and what you now do by default | folded into R, ~10s |

Those proportions are the entire point. In a three-minute answer that is roughly **18 seconds of situation, 27 seconds of task, 90 seconds of action, 45 seconds of result**.

### The "80% situation" mistake

The single most common failure in behavioural interviews is spending 80% of the answer on Situation. It happens because the situation is the easiest part to talk about — you lived it, it needs no self-appraisal, and it feels like you are being thorough. The interviewer hears context with no candidate in it.

**Not this:**

> "So we were a fintech, about 40 people, Series A, and the product was a lending platform for SMEs — quite complicated because there were three user types, the borrower, the broker, and our internal credit team, and the credit team had this legacy tool that was built in 2016 before I joined, and the borrower flow had been rebuilt twice…"

Three minutes in, no decision has been described.

**This:**

> "We were an SME lending product with three user types. Our broker drop-off was 62% at the document-upload step and nobody knew why. I owned the redesign end to end, working with one engineer and a credit ops lead."

Nineteen seconds. Everything the listener needs. Now you have 2:40 for the part that gets scored.

### Diagnostic: run the pruning test

Write the story out. Delete any Situation sentence that, if removed, would not make a later Action sentence confusing. Almost always three or four sentences go.

### The Action section

This is where the interview is actually won. The trap is describing activities ("I ran a workshop, then I did some interviews, then I made wireframes") instead of decisions. Activities are a résumé. Decisions are a designer.

**Not this:** "I interviewed eight brokers and then redesigned the upload flow."

**This:** "I interviewed eight brokers and expected to hear that the upload UI was confusing. Instead, six of eight told me they were uploading from a phone, in a client's office, from documents the client had emailed them. The problem was not the UI, it was that we required desktop-grade file handling in a mobile moment. So I dropped the redesign I had started and reframed the brief around capture-on-mobile: camera-first upload, per-document progress, and resumable sessions, because their sessions were being killed by lift signal."

Note what happened there: an expectation, disconfirming evidence, a reframe, and a decision with a reason. That's the whole game.

### The Result section

Rules:

- Lead with a number if you have one. If you do not have one, lead with a concrete observable ("the credit team stopped keeping the parallel spreadsheet they had been running for two years").
- Give the baseline as well as the after. "Conversion went up 12%" is unreadable without knowing 12% of what.
- Name attribution honestly. "Drop-off went from 62% to 31% over the following quarter. We also cut the broker onboarding email in the same period, so I would not claim all of it — but the step-level drop-off is the cleanest signal we had, and it moved within two weeks of ship."

Honest attribution is a *strength* signal, not a weakness. Interviewers hear inflated claims constantly and discount all of them. Being the one candidate who says "I can't fully separate my effect from the other change" buys credibility for the numbers you *do* claim.

### The L: learning

Ten seconds, at the end, and it must be specific enough to be falsifiable.

**Weak:** "I learned the importance of talking to users early."
**Strong:** "I learned to ask 'where are they physically when they do this?' in the first interview. It's now the second question on every discussion guide I write, and it has changed the brief twice since."

### STAR failure modes

| Failure mode | Symptom | Fix |
| --- | --- | --- |
| 80% situation | Two minutes before you appear in your own story | Prune to three sentences of context |
| "We" throughout | Interviewer cannot find your contribution | Say "the team decided X; I argued for Y and did Z" |
| Activity list | Verbs but no reasons | Every action gets a "because" |
| No result | Story ends at ship | Even "we never measured it, and that was my mistake" beats silence |
| Hero narrative | You were right, everyone else was wrong | Include one thing you got wrong |

---

## CIRCLES — for product-design prompts

Use for "design a X for Y", "how would you improve Z", and most 45-minute product-design rounds. Attributed to Lewis Lin.

| Step | Name | What you actually do |
| --- | --- | --- |
| **C** | Comprehend the situation | Restate the prompt, ask clarifying questions, state assumptions |
| **I** | Identify the customer | Choose *one* segment and defend the choice |
| **R** | Report customer needs | Needs as jobs and pains, not as features |
| **C** | Cut through prioritisation | Pick one need; say what you are deliberately not solving |
| **L** | List solutions | Diverge — three genuinely different approaches, not three skins |
| **E** | Evaluate trade-offs | Compare against explicit criteria |
| **S** | Summarise recommendation | Pick one, state the risk, state what you would measure |

### Spend 40% of the time on steps 1–4

This is the guidance candidates ignore and it is why they fail. In a 45-minute round, that is **roughly 18 minutes before you sketch anything**.

The instinct is that time spent not-drawing is time wasted. The opposite is true: an elegant solution to the wrong problem scores zero, and the interviewer is specifically testing whether you can resist jumping to solutions. Slow framing is the differentiator between a mid-level and a senior score in almost every published rubric.

A workable 45-minute budget:

| Minutes | Step | Output |
| --- | --- | --- |
| 0–5 | C — comprehend | Restated prompt, 4–6 clarifying questions, assumptions on the board |
| 5–10 | I — identify | Two or three candidate segments; one chosen, with reasoning |
| 10–15 | R — report needs | 4–6 needs, ideally from real evidence or named as hypotheses |
| 15–18 | C — cut through | One prioritised need, with an explicit "not now" list |
| 18–28 | L — list solutions | Three approaches, sketched roughly |
| 28–38 | E — evaluate | Criteria table; one option developed in detail |
| 38–43 | S — summarise | Recommendation, risk, metric |
| 43–45 | — | Questions, what you'd validate |

### Comprehend: what to ask

Four to six questions, then stop. Endless clarifying reads as stalling.

- "Is this a new product or an addition to an existing one?"
- "What is the business goal — acquisition, retention, monetisation, or cost?"
- "Any platform or technical constraint I should design within?"
- "Is there a timeframe? Six weeks and eighteen months are different designs."
- "Do we have existing users I can assume access to?"

Then state assumptions out loud, and write them where they stay visible: "I'm going to assume mobile-first, that we have an existing user base of about 100k, and that the goal is retention rather than acquisition. Tell me if any of those is wrong."

### Identify: choose one segment

Listing five personas and designing for all of them is the classic mid-level answer. Name two or three, pick one, and defend it against a business goal:

> "There are three obvious users: the commuter, the weekend leisure rider, and the delivery courier. The courier does the most trips per week and the highest revenue per user, but the segment is small and already well served. I'm going to design for the commuter, because the business goal I was given is retention, and the commuter is the only segment with a natural daily habit loop to build on (Module 13 — behavioural design). I'll flag where the courier case would break my design."

### Report needs

Frame as jobs and pains, not features. "They want a saved-routes feature" is a solution. "They repeat the same journey ten times a week and re-enter it every time; the pain is repeated effort in a hurry, often one-handed on a platform" is a need. The second one generates several solutions; the first one generates one.

### Cut through

Pick one. Say what you are consciously deprioritising and why — this is the sentence that reads as senior:

> "I'm going to solve the repeated-journey pain and explicitly not solve discovery or payment this round, because repeated journeys are the highest-frequency moment and frequency is what builds the habit we need for retention."

### List solutions

Three genuinely different approaches. A test: if all three could be built by the same team in the same sprint with the same data model, they are not different approaches, they are three visual treatments.

- Different *mechanism* (automation vs manual shortcut vs prediction)
- Different *placement* (in-app vs OS-level widget vs notification)
- Different *cost profile* (zero engineering vs heavy ML)

### Evaluate

Use a criteria table, and give the criteria before you score, or the scoring looks reverse-engineered:

| Option | User effort saved | Build cost | Risk if wrong | Accessibility |
| --- | --- | --- | --- | --- |
| Manual saved routes | Medium | Low | Low | Straightforward |
| Predicted next journey | High | High | High — wrong prediction is worse than none | Needs a visible override |
| Home-screen widget | High for repeat users | Medium | Medium | Platform-dependent |

### Summarise

Recommendation, the single biggest risk, and the metric. "I'd ship manual saved routes first, because the prediction approach fails badly when wrong and I have no data yet to train it. Saved routes also *generates* that data. The risk is that manual saving is too much friction to adopt, so the metric I'd watch is the percentage of repeat journeys started from a saved route within four weeks (Module 12)."

---

## The critique framework

For "critique this app", "what's wrong with this screen", and portfolio-review-style teardowns. This mirrors the 20-minute critique format in Module 05.3.

### Six moves

1. **Frame.** Who is this for, what is the primary task, what does the business need? State your assumptions out loud. Two minutes. Skipping this is how candidates end up critiquing a professional tool as though it were a consumer app.
2. **Walk the path.** Go through the primary task as a first-time user, narrating perception: what draws your eye, what you expect to happen, what actually happens. Narrate, do not summarise afterwards.
3. **Probe the edges.** Empty state, error state, loading state, long content, zero results, offline, small screen, keyboard-only, contrast, target size. Most severe findings live here (Module 07, Module 10).
4. **Categorise by heuristic with severity.** Attach each finding to a named heuristic and rate it 0–4 (Module 05). "The error appears after submit and clears the form" → #9 recover from errors, severity 4.
5. **Prioritise and propose.** Top three, with a fix each, and what you would measure. Include a cheap fix alongside the right fix — a recommendation the team cannot afford produces nothing.
6. **Name the limits.** What you could not assess without data or users; what would change your mind. This is the step candidates skip and interviewers remember.

### Two rules that separate good critiques from bad

**Diagnose before you prescribe.** If you open with "I'd make this button blue", the conversation becomes about your taste and you have lost. Open with what breaks and for whom.

**Preference is not a heuristic.** "I don't like the green" is not a consistency violation. Either say what it costs — "the green is the same green used for destructive confirmations elsewhere in the flow, so the mapping between colour and meaning has broken (Module 06)" — or don't say it.

### Model opening

> "Before I critique it, let me say what I think it's for, and you can correct me. This looks like a consumer budgeting app, the primary task is checking whether you can afford something right now, and the business likely needs return visits rather than one-off setup. If that's roughly right, I'll walk the primary task as a new user, then look at the states around it — empty, error, and what happens with a hundred transactions rather than three — because that's usually where the real problems are."

---

## Whiteboard structure

For live design exercises, 45 minutes, in a room or on a shared canvas.

| Minutes | Phase | What is on the board at the end |
| --- | --- | --- |
| 5 | **Clarify** | Restated prompt, questions asked, assumptions written down |
| 5 | **Frame** | The user, the job, the one problem you're solving, success criteria |
| 10 | **Diverge** | Three rough approaches, deliberately unequal |
| 5 | **Converge** | Criteria and a chosen direction, with the reason |
| 15 | **Detail** | The chosen flow drawn — screens, states, edge cases |
| 5 | **Validate** | What you'd test, what would prove you wrong, what you cut |

### Talk continuously — silence is unscoreable

The interviewer is not scoring your drawing. They cannot see your reasoning, and a beautiful sketch produced in silence gets marked "unable to assess". Narrate constantly:

- "I'm going to put the entry point here, because…"
- "I'm hesitating between two layouts — let me say what the trade-off is…"
- "This is deliberately rough; I want to get the flow right before the layout."
- "I'm going to park the settings screen — it matters but it isn't where the problem is."

If you genuinely need thirty seconds to think, *say so*: "Give me twenty seconds to think about the edge case here." A declared silence is fine. An undeclared one reads as being stuck.

### Whiteboard mechanics

- **Write the frame in a corner and leave it there.** User, job, success metric. Refer back to it when you make decisions — "this option is better against the criterion I wrote up here."
- **Boxes and arrows before pixels.** Flow first, layout second, visual detail only if there is time.
- **Draw the ugly states.** Empty, error, loading, long content. Drawing an empty state unprompted is a strong senior signal.
- **Label as you go.** Unlabelled boxes are unreadable to a reviewer who looks at the photo later.
- **Handle the interruption.** Interviewers interrupt on purpose to see whether you can absorb new information. Do not defend; integrate. "That changes the third option — if most users are on desktop, the widget approach loses its main advantage. Let me redo the comparison."

---

## The three-beat "walk me through your process" answer

Ninety seconds, and almost always asked. The failure mode is reciting the double diamond as a generic five-stage pipeline, which tells the interviewer nothing except that you have seen a diagram.

**Beat 1 — the principle (15s).** What your process is *for*, in your own words.

**Beat 2 — the shape, made specific (45s).** Named stages with what you actually produce, hung on one real project.

**Beat 3 — how it flexes (30s).** How the process changes under constraint. This is the beat that separates senior from junior, because it shows the process is a tool you own rather than a ritual you perform.

Worked example:

> "My process is really about reducing the cost of being wrong — front-load the cheap ways to find out you're solving the wrong problem, before anything expensive gets built.
>
> Concretely, on the broker upload project: I started with framing, which meant getting the team to agree what problem the 62% drop-off actually represented, because two people thought it was a UI problem and one thought it was a document policy problem. Then discovery — eight broker interviews and a look at session recordings — which is where the mobile finding came from. Then definition: one problem statement and success criteria, signed off before anything got drawn. Then iteration: three concepts, two rounds of five-person usability tests, then a staged rollout with the drop-off metric instrumented before launch.
>
> That's the full version, and I get it maybe a third of the time. When I don't, I cut the middle, not the ends: I'll do three interviews instead of eight and one round of testing instead of two, but I won't skip agreeing the problem, and I won't skip instrumenting the metric — because those are the two places where skipping costs you the whole project rather than some polish."

---

## Answering "why?" three levels deep

Interviewers probe by repeating "why?". Most candidates have one level of answer, some have two, very few have three. **The third level is where offers are decided.**

| Level | Question being answered | Signal |
| --- | --- | --- |
| 1 | What did you do? | You were present |
| 2 | What principle made that the right call? | You understand your craft |
| 3 | What did it cost, and how did you know it worked? | You have shipped and lived with consequences |

### Worked example

**Q: "Why did you use a bottom sheet there?"**

**Level 1 — what you did.**
> "It gave us more room for the filter options without leaving the results screen."

Fine, but this is a description. Anyone reading the screen could say it.

**Level 2 — the principle.**
> "Filtering is a modal sub-task inside a larger task, and the user needs to see the result count change as they filter. A full-page navigation would break that feedback loop and lose their scroll position, which is a Doherty threshold and a user-control problem (Modules 03, 05). A bottom sheet keeps the results partly visible and keeps the thumb in the reachable zone on mobile (Fitts's law)."

Good. Most strong candidates stop here.

**Level 3 — the cost and the evidence.**
> "It cost us two things. First, bottom sheets are genuinely worse for screen reader and keyboard users unless you get focus trapping and the escape route exactly right — we shipped it wrong the first time and a keyboard user could tab out of the sheet into the page behind it, which we caught in an accessibility audit two weeks after launch and fixed (Module 10). Second, we lost the ability to deep-link to a filtered state, which the marketing team wanted for campaigns, and we had to build that back later as a URL-driven open.
>
> How I knew it was still right: filter-apply rate went from 8% to 19% of sessions, and the median time between opening filters and applying them dropped from 22 seconds to 9. If those hadn't moved, the sheet wasn't buying anything and I'd have reverted to the full page, which was cheaper to maintain."

That answer contains a mistake, a trade-off the business felt, and a falsifiable threshold. It is very hard to fake, which is exactly why it is scored so highly.

### How to build level 3 into your stories

Before the interview, for each of your two or three main projects, write down:

- One thing the decision cost — in maintenance, in accessibility, in another team's ability to do their job, in future flexibility.
- One number or observable that told you it worked.
- What number would have made you reverse it.

Three bullets per project. It is an hour of preparation and it changes the outcome of the round.

---

## Questions you cannot answer

You will get one. The correct behaviour is not to bluff, and it is not to collapse.

### The three-part response

1. **Say the boundary plainly.** "I haven't worked on native voice interfaces, so I'd be making that up."
2. **Reason from adjacent ground.** "What I can tell you is how I'd approach it from the principles I do have…"
3. **Say how you'd close the gap.** "…and the first thing I'd do is find someone who has shipped one, because the failure modes in voice are not the ones I'd predict from screen work."

Worked example:

> **Q: "How would you handle localisation for a right-to-left language?"**
>
> "Honestly, I've never shipped RTL, so I'd be guessing at the specifics and I'd rather not. What I do know from adjacent work is the general shape: it isn't a mirror operation, because some elements — media scrubbers, numerals, chart axes — don't flip, and directional icons need review one by one. So structurally I'd expect the work to be a design-system-level change with logical rather than physical properties for spacing (Module 11), plus a review pass with a native reader rather than a tool, because the tool will catch layout and miss idiom. And I'd want that native reviewer in the room from week one rather than at QA. But I'd be leaning heavily on someone who has actually done it."

That answer scores well. It demonstrates calibrated confidence, transferable reasoning, and knowing when to defer — three things senior rubrics explicitly reward.

### Why bluffing fails badly

The interviewer usually asks the question *because* they are an expert in it. A confident wrong answer converts a small knowledge gap into a large judgement problem: if you'll bluff here, you'll bluff in a design review, and nobody can trust your other claims. The knowledge gap costs you a point. The bluff costs you the round.

### Do this / not that

| Not this | This |
| --- | --- |
| "Well, I'd probably just do the standard thing…" (vague hedge) | "I don't know. Here's how I'd find out." |
| "I don't know." (full stop, silence) | "I don't know that specifically — here's the closest thing I have." |
| Making up a number | "I remember the direction but not the figure — it improved materially, and I'd want to check before quoting it." |
| Answering a different question you do know | "That's not something I've done. Can I tell you about the closest case, or would you rather move on?" |

The last one is worth practising: explicitly offering the interviewer the choice is a small move that reads as very composed.

---

## Choosing a framework live

| The prompt sounds like | Use |
| --- | --- |
| "Tell me about a time when…" | STAR+L |
| "Design a…" / "How would you improve…" | CIRCLES |
| "What do you think of this?" / "Critique…" | Critique framework |
| "Here's a brief, use the whiteboard" | Whiteboard structure |
| "Walk me through your process" | Three-beat |
| "Why did you do that?" (repeated) | Three levels deep |
| Anything outside your experience | Boundary / adjacent / gap-closing |

If you are unsure which mode a question is in, ask: "Do you want the story of a specific time this happened, or how I'd approach it generally?" Nobody has ever been marked down for that question.

---

## Common mistakes across all frameworks

- **Naming the framework out loud.** Use the structure; don't announce it.
- **Front-loading context.** Applies to STAR, critique, and whiteboard equally.
- **Solutions before problems.** The most consistent junior tell there is.
- **Uncosted principles.** Every principle you cite should come with what it trades away. A principle presented as free reads as something you read rather than something you used.
- **No metric.** Every design answer should end with what you'd measure and what would prove you wrong (Module 12).
- **Ignoring the interruption.** Interviewers interrupt to test adaptability. Integrate, don't defend.
- **Perfect stories.** A story with no mistake in it reads as either rehearsed or dishonest.

## Check yourself

1. What proportion of a STAR answer should be Action, and what is the most common proportional error?
2. What share of a CIRCLES answer belongs to the first four steps, and why does that feel wrong to do?
3. Name the six moves of the critique framework, and which one candidates skip.
4. Give the six-phase minute budget for a 45-minute whiteboard exercise.
5. What are the three levels of a "why" answer, and what specifically lives at level 3?
6. Give the three-part structure for a question you cannot answer, and explain why bluffing costs more than the gap.

---

<!-- nav -->
[← Previous: Interview Prep](../README.md) · [↑ Interview Prep](../README.md) · [Next: Case Study Structure →](case-study-structure.md)
