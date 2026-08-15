# Case Study Structure

## In one line

A case study is an argument that you make good decisions under real constraints — not a documentary of everything that happened.

## The weighting

Most portfolios are process documentaries: sticky notes, personas, and a hero shot. They fail because the reviewer cannot find a single decision you made or a single trade-off you weighed. Allocate space and speaking time as follows.

| Section | Weight | The question it answers |
| --- | --- | --- |
| Context | 10% | Where were we, and what do I need to know to follow this? |
| Problem | 20% | What was actually broken, and how do you know? |
| Constraints | 5% | What was I not free to change? |
| Process | 25% | How did I get from not knowing to knowing? |
| Solution | 25% | What did I decide, and why that rather than the alternatives? |
| Impact | 10% | What changed, honestly? |
| Reflection | 5% | What would I do differently? |

The two 25% blocks — process and solution — are where hiring decisions are made. Context and impact routinely eat 60% of a candidate's slides; that is the single most common structural failure.

---

## Context — 10%

Enough to make the rest legible. No more.

**Include:**
- Product and who uses it, in one sentence.
- Your role, stated precisely, and the team shape.
- Timeframe.
- Where the project came from — a metric, a support pattern, a strategy bet, a mandate.

**Cut:**
- Company founding history, funding rounds, org charts.
- A tour of the whole product when the project touched one flow.
- "The Team" slide with six avatars.

**Role precision matters more than role seniority.** "I was the only designer, working with two engineers and a PM; I owned research, IA, and UI, and the PM owned prioritisation" is worth more than "Lead Product Designer". Reviewers are trying to work out what you personally did, and vagueness here is read as inflation.

**Not this:**
> "Acme is a leading provider of cloud-based workforce management solutions, founded in 2014, serving over 400 enterprise customers across 12 countries…"

**This:**
> "Acme is shift-scheduling software used by shift managers in retail and hospitality. I was one of two designers; I owned the scheduling surface. Six months, a PM and four engineers. The project started because support tickets about 'lost shifts' had tripled in two quarters."

---

## Problem — 20%

Twice the weight of context, because the quality of the problem statement predicts the quality of everything downstream.

**A strong problem section has four things:**

1. **The symptom** — the observable thing that made someone care. A number, a ticket volume, a churn pattern, a sales objection.
2. **The evidence** — what you looked at to move from symptom to diagnosis, and how much of it there was.
3. **The reframe** — the difference between the problem as handed to you and the problem as you came to understand it. This is often the most valuable sentence in the entire case study.
4. **The problem statement** — one sentence, specific enough to be falsifiable, with a success criterion attached.

**The brief you were given versus the problem you found.** Almost every good project has a gap between these. Show it explicitly.

> "I was asked to redesign the shift-swap screen because managers said it was confusing. What the evidence showed was that the screen was fine, and the confusion came from a state the screen couldn't express: a swap that had been approved by one manager and was awaiting a second, which our data model treated as 'pending' and our UI rendered identically to 'not yet reviewed'. The problem wasn't the screen, it was that we had one label for two situations with different consequences."

If your problem statement is the same as the brief you were handed, say so and say why you checked — but be aware the reviewer will read it as either an unusually clean brief or an unexamined one.

**Problem statement format that works:**

> "Shift managers cannot tell whether a swap request needs their action, which causes an average of 2.4 days of delay per swap and generates the 'lost shift' tickets. Success is swap resolution time under 24 hours without increasing wrongly-approved swaps."

---

## Constraints — 5%

Short but non-optional. Constraints are what make your decisions readable as decisions rather than preferences. A design produced with no stated constraints is unassessable, because the reviewer cannot tell whether you chose the option you chose or the only option available.

| Constraint type | Examples |
| --- | --- |
| Technical | Legacy data model, no realtime infrastructure, a vendor component you cannot restyle |
| Time | Eight weeks to a contractual deadline; a conference launch |
| Team | One engineer part-time; no research budget; no access to users |
| Regulatory | Records must be immutable; consent required before capture |
| Organisational | Two teams own halves of the flow; the design system was mid-migration |
| Existing users | 40,000 people trained on the old model; no big-bang migration possible |

One slide or one short paragraph. Then use them: every time you rule out an option later, point back at the constraint that ruled it out.

---

## Process — 25%

The purpose of the process section is **not** to show that you know the method names. It is to show how your understanding changed. Two things must appear.

### 1. Discarded options

Show at least two directions you tried and abandoned, with the reason. A case study in which every idea worked is either fiction or a project with no difficulty in it — reviewers read both the same way.

For each discarded option:

| Element | Example |
| --- | --- |
| What it was | A per-swap approval inbox, separate from the schedule |
| Why it looked good | Cleanest mental model; matched how managers described the task |
| Why it died | Testing showed managers wouldn't leave the schedule view — they used it as the source of truth all day, and a separate inbox went unvisited in four of five sessions |
| What it taught | The fix had to live inside the schedule, not beside it. That constraint shaped everything after. |

That last row matters: a discarded option that taught you nothing is just noise. Every abandoned direction should have narrowed the space.

### 2. The turning point

Name the moment when evidence changed your direction. Call it out explicitly — literally label it in the deck or the page. It is the single highest-signal element in a case study because it proves that research affected the outcome rather than decorating it.

> **The turning point.** In session three, a manager approved a swap I had assumed was uncontroversial, then immediately opened a second tool to check something. I asked what. She was checking whether the person taking the shift was already at overtime, because approving into overtime came out of her budget. None of our five interviews before that had mentioned overtime, because I had been asking about the swap flow and not about what she was accountable for. That reframed the design from 'make the state clear' to 'put the consequence of approving in front of her at the moment she approves' — which is a different and much more useful product.

**Do this / not that in process:**

| Not this | This |
| --- | --- |
| "I conducted user research." | "Five contextual interviews with shift managers during their actual shift-planning hour, because I wanted to see the other tools open on their screen." |
| A photo wall of sticky notes | The three themes the stickies produced, and which one you acted on |
| "I created personas." | "We already had personas; they didn't distinguish the two managers types that mattered here, so I built one axis instead: managers with budget accountability versus those without." |
| Every artefact you produced | The three artefacts that changed a decision |
| A linear method pipeline | The point where you went backwards, and what sent you back |

**On methods:** name them precisely and name the sample size. "Five moderated sessions, remote, unmoderated follow-up with 40" is credible. "User research" is not. If your sample was tiny, say so and say what that means: "Five sessions, which is enough to find the big usability failures and not enough to size the problem — I used the support ticket data for sizing" (Module 09).

---

## Solution — 25%

### Annotate decisions, not descriptions

The most common failure in a portfolio is a beautiful screen with a caption that describes what is visible. The reviewer can see it. What they cannot see is why.

| Not this (description) | This (decision) |
| --- | --- |
| "A clean dashboard with the key metrics at the top." | "Overtime cost sits above the approve button rather than in a detail panel, because the turning point told us the decision hinges on it and managers wouldn't go looking." |
| "We used a card layout for the shifts." | "Cards rather than a table, because managers scan for a person more than they compare across columns, and cards let the conflict badge sit on the offending shift rather than in a status column three columns to the right (Module 04 — proximity)." |
| "Colour-coded status." | "Three statuses, colour-plus-icon-plus-text rather than colour alone. Colour alone failed our contrast check for the amber state and would have been unreadable for the roughly 8% of male managers with a colour vision deficiency (Module 10)." |
| "A confirmation modal." | "Confirmation only for approvals that push someone into overtime — about 12% of approvals. Confirming everything trains people to dismiss it, and the whole value here is that the 12% get noticed." |

The pattern: **decision, reason, and where the reason came from.** Ideally the reason points back at your research or your constraints.

### Show states, not just the happy path

Include, at minimum:

- **Empty** — first run, no data, and the difference between "nothing yet" and "nothing matched".
- **Loading** — and what happens if it is slow.
- **Error** — what breaks, what the user can do about it, and whether their input survives.
- **Edge content** — the longest name, the busiest week, forty items instead of three.
- **Permission variants** — what a manager without budget accountability sees.

Showing states unprompted is one of the clearest seniority signals available. Most portfolios show one perfect screen with three plausible rows of data; a portfolio that shows the ugly week reads as built by someone who has shipped (Module 07).

### Show accessibility as design, not as a compliance slide

Weave it into the decisions rather than appending an "accessibility" section at the end. Good things to show:

- Focus order through the primary flow, drawn.
- Keyboard operation of the one custom component you built.
- Contrast values for the status colours, with the numbers (4.5:1 for body text, 3:1 for large text and UI components).
- Target sizes (24×24 CSS px minimum under WCAG 2.2; 44×44 is the practical mobile target).
- What screen reader announcement fires when the state changes, and why you chose that wording.
- One accessibility problem you found late and what it cost to fix.

That last one is worth a lot. "We shipped the sheet with a broken focus trap and caught it two weeks later in an audit" is more convincing than any claim of compliance (Module 10).

### Show the system, if there is one

If the work touched a design system: which components you reused, which you extended, which you had to build new, and what you contributed back (Module 11). Reviewers at any company with a system will care about this more than about the screen.

---

## Impact — 10%

### Be honest about attribution

This section is short and it is where credibility is won or lost. Reviewers have heard "increased conversion by 40%" so many times that the number does no work at all. What does work is a number with its uncertainty attached.

**Structure:**

1. The baseline.
2. The after, with the time window.
3. What else changed in the same window.
4. What you would claim, and what you would not.

> "Swap resolution time went from a median of 2.4 days to 9 hours over the eight weeks after rollout, against a 24-hour target. 'Lost shift' tickets fell about 60% over the same period. Two caveats: we rolled out to the highest-volume accounts first, so the population is not the same as the baseline population, and support also added a macro for these tickets in week three, which will have affected ticket volume independently. I'd claim the resolution-time number — that one is instrumented per swap and it moved within days of each account getting the change. I'd treat the ticket number as directional."

### When you have no numbers

Many real projects ship without measurement, or you left before the data came in, or the numbers are confidential. Do not invent, and do not skip the section.

Acceptable substitutes, roughly in order of strength:

| Substitute | Example |
| --- | --- |
| Qualitative evidence with a source | "In post-launch sessions, five of six managers found the overtime cost unprompted; before, none had." |
| Behaviour change you can name | "The ops team stopped maintaining the parallel spreadsheet they'd run for two years." |
| Adoption without a target | "Rolled to 100% of accounts in six weeks with no rollback." |
| Honest absence | "We didn't instrument it. That was my mistake — I should have made the metric a launch requirement, and it is now the first thing I write into a brief." |

The honest absence, delivered without squirming, scores better than a vague claim. What loses points is "it was very well received."

### Say what did not work

One line naming something in the shipped design that underperformed, and what you did about it. A case study with no post-launch problem is a case study that stopped paying attention at ship.

---

## Reflection — 5%

Three sentences, not a page. It must be specific enough to be falsifiable and it must have changed your behaviour since.

**Weak:** "I learned the importance of collaboration and of testing early."

**Strong:** "I spent three weeks on the separate-inbox direction because I designed from what managers *said* they did rather than watching them. I now schedule the first two sessions as observation during the real task, not interviews — it has changed the brief on both projects since."

Optionally add: what you would do with another month, and what you would do with only a week. Both answers say something about your judgement.

---

## Presentation mechanics

### Time

Most portfolio reviews are **45 minutes total**: roughly 15–20 minutes of presentation per case study, then questions, then their questions and yours. Confirm the format with the recruiter; if they say "45 minutes", plan for 35 of content and expect to be interrupted into 45.

**Two case studies, not five.** Two deep cases beat five shallow ones every time. Five signals that you cannot judge what matters. Pick:

- One that shows **depth** — ambiguity, research, a genuine reframe, a hard trade-off.
- One that shows **range** — a different problem type, a different constraint, a different phase. A fast constrained project is a good second case precisely because it shows judgement under pressure.

Keep a third in reserve, unpresented, for "do you have anything with more [X] in it?"

### One slide, one idea

If a slide needs a paragraph of narration to make sense, it is two slides. Slide count is not a virtue — a 40-slide deck of single ideas presents faster than 15 dense ones, because the audience is never decoding while you are talking.

Practical rules:

- One heading per slide that states the idea as a claim, not a label. "Managers wouldn't leave the schedule view" beats "Research findings".
- Never read your slides aloud. If the slide says it, say something else.
- Screens large enough to read on a laptop over video compression. Two screens per slide maximum.
- Annotations as callouts on the screen itself, not as a paragraph underneath.
- Dark or light, but test it on a shared screen. Video compression destroys low-contrast greys.

### Lead with the punchline

Open every case study, and ideally every section, with the conclusion. Reviewers form an impression in the first two minutes and spend the rest confirming or revising it. Making them wait ten minutes for the point wastes the part of their attention you actually had.

> "This is a project about a problem that turned out not to be the problem we were given. We were asked to redesign a screen; what we shipped was a change to what one label meant. Swap resolution went from 2.4 days to 9 hours. Let me show you how we got there."

Same rule inside sections: "Research changed our direction once, in session three. Here's what happened."

### Anticipate interruption

Good interviewers interrupt. Assume you will be stopped every three to four minutes, and design for it:

- **Never build a payoff that depends on ten uninterrupted minutes.** Each section must survive being cut short.
- **Know your cut plan in advance.** Which slides go if you are at minute 25 with two sections left. Practise the 10-minute version of each case.
- **Answer the question asked, then return deliberately.** "Good question — [answer]. That actually comes up two slides on, so let me carry it there." Do not say "I'll get to that" and move on; it reads as rigid.
- **If the interruption is a challenge, engage it.** "That's fair, and it's the weakest part of the design. Here's what I traded to get it." Defending everything is worse than conceding one thing well.

### Delivery

- **Practise out loud, timed, at least three times.** Reading it in your head is 30% faster than saying it and hides every sentence you cannot actually say.
- **Have the file locally.** Not only in a cloud tool, not only behind a VPN.
- **Have a PDF fallback** in case screen share, fonts, or the prototype fails.
- **Do not live-demo a prototype** unless you have a video fallback. Prototypes fail on other people's networks.
- **Watch the clock, visibly.** Saying "I'm at 20 minutes, I have one section left — do you want me to finish it or move to questions?" reads as extremely composed.

---

## What to have ready for Q&A

Anticipate the standard eight. Have a prepared 60-second answer to each, plus a slide in an appendix where useful.

| Question | What they're testing | Have ready |
| --- | --- | --- |
| "What would you do differently?" | Self-awareness | One real mistake with the cost, and what changed since |
| "What was the hardest trade-off?" | Judgement | A decision with two defensible sides and why you picked one |
| "What did you disagree with the team about?" | Collaboration under friction | A specific disagreement, how it resolved, whether you were right |
| "How did you know that was the right problem?" | Rigour | Your evidence chain and its weaknesses |
| "What did the engineers push back on?" | Practicality | A constraint that changed the design, and how you found the alternative |
| "What would you have done with half the time?" | Prioritisation | Which 30% you'd keep and why |
| "How did you measure it?" | Outcome thinking | Instrumentation, baseline, and what you couldn't measure |
| "What was your specific contribution?" | Attribution honesty | A clean line between yours, the team's, and inherited |

**Appendix slides worth carrying:** the discussion guide, the raw research findings, an early discarded direction in full, the component inventory, the accessibility annotations, the instrumentation plan. Being able to say "I have that — one second" and produce it is disproportionately impressive.

---

## NDA and confidential work

Almost every candidate has some. The failure is either refusing to discuss anything, which leaves you with nothing to present, or leaking, which is itself a hiring signal — the reviewer will assume you would do the same with their work.

### What you can almost always do

| Technique | How |
| --- | --- |
| **Abstract the domain** | "A B2B scheduling tool" rather than the client's name. Present the problem class, not the account. |
| **Index the numbers** | "Drop-off fell by roughly half" or "baseline 100, after 42" rather than absolute revenue. |
| **Redact the surface** | Blur or greek the data, replace real customer names, remove logos. Keep layout and interaction. |
| **Rebuild the screens** | Redraw the flow in a neutral style. Legitimate, and it also usually presents better than production screenshots. |
| **Present process only** | Show the reasoning, the discarded options, and the decision criteria, with sketch-level fidelity throughout. |
| **Use a personal project as the visual case** | Pair it with a verbal-only account of the confidential work. |

### How to say it

Say it once, early, plainly, and then get on with it. Apologising repeatedly wastes time and draws attention to what is missing.

> "This one is under NDA, so the screens are redesigned in a neutral style and the numbers are indexed rather than absolute. Everything about the reasoning and the decisions is accurate. If you want to dig into anything specific I'll tell you what I can."

If asked for something you genuinely cannot share:

> "I can't share that one — it's a named client and the work isn't public. What I can do is talk you through how I approached the same problem type, or go deeper on this project instead. Which is more useful?"

Interviewers respect this. A candidate who protects a former employer's confidence is demonstrating exactly the behaviour they want from a future employee. What they will not accept is *only* confidentiality — you must arrive with something presentable, even if you had to build it yourself.

### Also

- Check your employment agreement before showing anything, including "internal only" screens.
- Never leave a deck with real client data on a public portfolio URL. Password-protect it or gate it.
- Do not name colleagues who have not agreed to be named.
- Public app store screenshots and marketing pages are usually fair game — the shipped product is public even if the process is not.

---

## The 90-second one-page version

You need this for recruiter screens, for the "tell me about a project" opener, for networking, and as the spine of the full presentation. Write one for each of your two cases and rehearse them until they are automatic.

### Template

> **[One sentence: what the product is and who uses it.]**
>
> **[One sentence: the symptom that started it — with a number.]**
>
> **[Two sentences: the problem as given versus the problem you found, and what evidence changed it.]**
>
> **[One sentence: the constraint that shaped the solution.]**
>
> **[Two sentences: what you shipped, framed as the central decision rather than a feature list.]**
>
> **[One sentence: the discarded direction and why it died.]**
>
> **[Two sentences: impact with a baseline, plus one honest caveat.]**
>
> **[One sentence: what you'd do differently.]**
>
> **[Closing offer: which part they'd like to go deeper on.]**

### Worked example

> "Acme is shift-scheduling software used by managers in retail and hospitality. Support tickets about 'lost shifts' had tripled in two quarters, and swaps were taking a median of 2.4 days to resolve.
>
> I was asked to redesign the shift-swap screen because it was 'confusing'. What five contextual interviews showed was that the screen was fine — we had one label, 'pending', covering two states with different consequences, and managers had no way to tell which needed them. The turning point was watching a manager approve a swap and then immediately open a second tool to check whether it pushed someone into overtime, because overtime came out of her budget. Nobody had mentioned that in any interview, because I'd been asking about the swap flow rather than what she was accountable for.
>
> The hard constraint was that the data model couldn't be changed inside the release window, so I couldn't split the state at the source.
>
> So the design put the consequence in front of the decision instead: the approve action shows the overtime cost inline, and confirmation fires only for the roughly 12% of approvals that cross the threshold — confirming everything would just have trained people to dismiss it.
>
> I spent three weeks first on a separate approvals inbox, which tested badly: managers wouldn't leave the schedule view, so the inbox went unvisited in four of five sessions. That's what told me the fix had to live inside the schedule.
>
> Resolution time went from 2.4 days to about 9 hours over eight weeks, against a 24-hour target. I'd caveat that we rolled to the highest-volume accounts first, so the population isn't identical to the baseline.
>
> What I'd do differently: I designed from what managers said before I'd watched them work, and it cost three weeks. I now put observation before interviews as a default.
>
> Happy to go deeper on the research or on the states — whichever is more useful."

That is roughly 300 words and lands at about 100 seconds spoken. Trim to your own pace.

---

## Case study smells

Signals that get a portfolio rejected before the interview:

| Smell | What the reviewer concludes |
| --- | --- |
| Five case studies, all shallow | Cannot judge what matters |
| No problem statement, only a brief | Executes, does not diagnose |
| Every idea worked | Fiction, or a project with no difficulty |
| Personas and empathy maps with no downstream use | Performs process rather than using it |
| Hero shots on gradients, no states | Has not shipped or maintained |
| "Increased engagement by 40%" with no baseline | Numbers are decoration |
| "We" for the whole case study | Contribution is unfindable |
| No constraints mentioned | Decisions are unassessable |
| Reflection section is generic | Has not thought about it since |
| Accessibility as a compliance slide at the end | Treats it as someone else's job |

## Check yourself

1. Give the seven sections and their percentage weights. Which two carry the hiring decision?
2. What four elements make a strong problem section, and which one is usually the most valuable sentence in the case study?
3. Why must a case study include discarded options, and what makes a discarded option worth including?
4. Rewrite "A clean dashboard with key metrics at the top" as a decision annotation.
5. What four things does an honest impact section contain, and what is the best substitute when you have no numbers?
6. Name four legitimate ways to present NDA work, and the one thing you must not do.
7. How many case studies should you bring, and what should each one be chosen to show?

---

<!-- nav -->
[← Previous: Answering Frameworks](answering-frameworks.md) · [↑ Interview Prep](../README.md) · [Next: App Critique →](../question-bank/app-critique.md)
