# Drills

## In one line

Thirty-four short, repeatable exercises that build one specific skill each — the design equivalent of scales, to be run in the ten to thirty minutes you actually have rather than the free weekend you do not.

## How to use these

Concepts are learned by reading; skills are learned by producing work and getting a verdict on it. Every drill below therefore has four parts: **what it builds**, **the steps**, **the time**, and **done well when** — a concrete standard you can hold your own output against, because the thing that stops solo practice working is the absence of a verdict.

Rules that make the difference:

- **Produce an artefact every time.** A written sentence, an annotated screenshot, a list. Thinking about a drill is not doing it.
- **Time-box hard.** These are deliberately short. A drill that expands to ninety minutes stops being repeatable, and repeatability is the entire point.
- **Repeat the ones you are worst at.** The drills you enjoy are the ones you have already learned.
- **Keep the output.** A folder of forty annotated screenshots is a portfolio of your critique ability and a swipe file at the same time.
- **Vary the subject, not the drill.** Run the same drill on a different product each time. The skill transfers only when the surface changes.

Drills are grouped by the skill they build. There is no required order, though the perception drills are the cheapest place to start because they need nothing but a screen.

---

## Perception, hierarchy, and visual craft

### Drill 1 — The squint test

**Builds:** the ability to see pre-attentive structure rather than the details you have been staring at.
**Time:** 10 minutes.

**Steps**
1. Screenshot any screen from a product you did not design.
2. Degrade it four ways in turn: physically squint, apply a heavy Gaussian blur, zoom the image to 25%, and convert to greyscale.
3. For each version, write down the answers to four questions: what groups do I see, where does my eye land first, can I still find the primary action, and is figure distinguishable from ground?
4. Now look at the undegraded screen and write what you *thought* the answers would be.

**Done well when:** at least one of your four predictions was wrong. If your predictions are always right you are either choosing screens that are too simple or you are grading yourself after the fact. The greyscale pass in particular should regularly reveal something that was carried by colour alone.

---

### Drill 2 — First-stop mapping

**Builds:** the vocabulary to narrate a hierarchy in an interview, in order, rather than gesturing at it.

**Time:** 10 minutes.

**Steps**
1. Take a screenshot. Look away for ten seconds, then look back for exactly one second and look away again.
2. Write down, in order, the first three things you registered.
3. Now write down what the *designer* clearly wanted you to register first, second, third — inferred from size, weight, colour, position, and isolation.
4. Where the two lists disagree, name the mechanism that caused the disagreement (a competing filled button, an image that outweighs the headline, a badge that beats the price).

**Done well when:** you can state the disagreement as a mechanism, not a preference — "three filled buttons destroy the pop-out effect, so search became serial" rather than "the buttons are confusing."

---

### Drill 3 — Spacing audit

**Builds:** the single most transferable visual-design skill, and the fastest fix available on most screens.

**Time:** 20 minutes.

**Steps**
1. Take a screenshot of a form, settings page, or content-dense screen.
2. Measure — actually measure, in pixels — the vertical gap between every adjacent pair of elements. Annotate them on the image.
3. List the distinct values you found. Most real screens produce eight to fifteen.
4. Identify every place where the gap *between* two groups is equal to or smaller than the gap *within* a group.
5. Re-propose the whole screen using a four-value scale (for example 4 / 8 / 16 / 40) and state which value each relationship gets and why.

**Done well when:** you found at least one genuine proximity failure, and your proposed scale has four or five values rather than a new set of twelve. The named failure mode to look for is between-group spacing that does not exceed within-group spacing, which makes section structure perceptually invisible no matter how heavy the headings are.

---

### Drill 4 — Contrast audit

**Builds:** the habit of measuring rather than eyeballing, and fluency with the WCAG figures.

**Time:** 15 minutes.

**Steps**
1. Pick a screen. List every distinct text-on-background pairing and every meaningful non-text element (input borders, icons, focus rings, chart series, disabled states).
2. Sample the actual colours and compute each contrast ratio with a checker.
3. Grade each against **4.5:1** for normal text, **3:1** for large text, and **3:1** for UI component boundaries and meaningful graphics.
4. Note every failure and propose a specific replacement value that passes.
5. If the product has a dark mode, repeat. Palettes that pass in light mode routinely fail in dark.

**Done well when:** you found failures in the places that are actually common — placeholder text, disabled controls, secondary metadata, icon-only buttons, and focus indicators — rather than only checking body copy, which almost always passes. A strong output also notes anything that would fail **1.4.1 Use of Color** by encoding meaning with hue alone.

---

### Drill 5 — Greyscale rebuild

**Builds:** hierarchy that does not depend on colour, which is the only hierarchy that survives contact with real users.

**Time:** 25 minutes.

**Steps**
1. Take a screen that leans heavily on brand colour.
2. Rebuild it in greyscale only, using size, weight, position, and space to carry every distinction the colour was carrying.
3. Then reintroduce exactly one colour, on exactly one element.
4. Compare the two against the original.

**Done well when:** the greyscale version still has an unambiguous primary action and a readable group structure. If it does not, the original was using colour to compensate for a hierarchy that was never built — a very common and very fixable diagnosis.

---

### Drill 6 — Type scale extraction

**Builds:** an eye for typographic system versus typographic accident.

**Time:** 15 minutes.

**Steps**
1. On any content-heavy page, list every distinct combination of font size, weight, colour, and line height.
2. Count them.
3. Reduce the list to the smallest set that preserves every *meaningful* distinction, and name the role of each remaining style (page title, section heading, body, caption, metadata, label).
4. Check the measure (characters per line) of the body text against a 45–75 character target and note the line height relative to size.

**Done well when:** you reduced the count substantially and can defend each surviving style by the job it does, not by how it looks. Note also whether two styles differ by so little that the difference reads as inconsistency rather than hierarchy — a two-pixel size difference communicates nothing and costs the system a token.

---

### Drill 7 — The emphasis budget

**Builds:** the discipline behind the Von Restorff effect, which only works against a plain background.

**Time:** 10 minutes.

**Steps**
1. On any screen, count every element competing for attention: filled buttons, badges, coloured chips, bold text, icons in accent colour, animated elements, tooltips.
2. Rank them by how much attention the *task* justifies.
3. Cut the list to one primary emphasis and at most two secondary ones. Write what each demoted element becomes instead.

**Done well when:** you can state the cost of each demotion — who is worse off and why that trade is acceptable. Removing emphasis is easy; defending the removal is the skill.

---

## Writing and content design

### Drill 8 — Rewriting error messages

**Builds:** the highest-frequency writing task in product design, and one interviewers ask about directly.

**Time:** 20 minutes.

**Steps**
1. Collect five real error messages. Deliberately trigger them: wrong password, expired card, network drop mid-save, invalid file type, a permission you do not have.
2. Grade each against four criteria: does it say **what happened** in plain language, **why** it happened, **what to do next**, and does it avoid blaming the user or exposing internals?
3. Rewrite all five.
4. For each, decide the carrier as well as the words — inline, toast, banner, or modal — and justify the choice by severity and by whether the user must act before continuing.
5. For at least one, propose a design change that means the error never occurs.

**Done well when:** every rewrite names a next action, and at least one of your five is answered with prevention rather than better prose. A weak output rewrites all five as friendlier sentences; a strong one notes that the best error message is the one made unnecessary by an input mask, a sensible default, or accepting the messy input.

---

### Drill 9 — Button label surgery

**Builds:** precision in the smallest, most-read text in any product.

**Time:** 10 minutes.

**Steps**
1. Screenshot a dialog, a form, or a checkout step. List every button, link, and menu item label.
2. For each, ask: does the label describe the *outcome* of pressing it, or the mechanism? Would it make sense read aloud on its own, with no surrounding context?
3. Rewrite the failures. Pay particular attention to confirmation dialogs, where "OK" and "Cancel" routinely produce the opposite of the user's intent.
4. Check the accessible name would contain the visible label text (WCAG 2.5.3 Label in Name) — this matters for anyone driving the interface by voice.

**Done well when:** every label survives being read in isolation, and your destructive-action dialog now has a verb on the confirming button ("Delete 4 files") rather than a generic assent.

---

### Drill 10 — Empty state writing

**Builds:** the state everyone forgets and every new user sees first.

**Time:** 20 minutes.

**Steps**
1. Pick a product surface that holds a list (files, messages, transactions, projects).
2. Write the copy and describe the layout for four distinct empty states: **first use** (nothing has ever been here), **user-cleared** (you finished everything), **no results** (a filter or search returned nothing), and **error or offline** (we could not load it).
3. For each, name the single action you want the user to take next, and put it in the design.

**Done well when:** your four states are genuinely different in tone and content. Collapsing first-use and no-results into one message is the standard failure, and it produces a screen that congratulates someone on an empty inbox when in fact their filter is broken.

---

### Drill 11 — Deleting words

**Builds:** the discipline that reduces extraneous cognitive load faster than any layout change.

**Time:** 10 minutes.

**Steps**
1. Take any onboarding screen, tooltip, or explanatory paragraph.
2. Cut it by half without losing information.
3. Cut the result by half again.
4. Read the final version and mark anything that has now become ambiguous. Restore only that.

**Done well when:** the second cut is still comprehensible and you can name exactly what the third-round restoration bought. The point is not brevity for its own sake — it is discovering how much of the original was serving the writer rather than the reader.

---

### Drill 12 — Microcopy in the gaps

**Builds:** anticipation, in Tognazzini's sense: bringing the user what they need at the moment they need it.

**Time:** 15 minutes.

**Steps**
1. Walk a flow you did not design — a sign-up, a booking, an application.
2. At every step, write down the question a user would be asking silently at that exact moment ("will this charge me?", "can I change this later?", "why do you need my date of birth?").
3. Find where each question is answered. Note how many are answered nowhere, or answered three screens later.
4. Write the one sentence that answers each unanswered question, and say exactly where it goes.

**Done well when:** you found at least three unanswered questions and your answers are placed at the point of anxiety, not in a help centre. This drill is the single best preparation for the interview question "how would you reduce drop-off in this flow?"

---

## Interaction, states, and flows

### Drill 13 — The state matrix

**Builds:** thoroughness, and the fastest available way to sound senior when asked to design anything.

**Time:** 20 minutes.

**Steps**
1. Pick one component or one screen.
2. Enumerate every state: empty first-use, empty after clearing, no results, loading, partial, populated, overflowing, error, offline, success, permission-denied.
3. For each, write one line describing what the user sees and what they can do.
4. Mark the two or three that carry the most risk in this particular context, and design those properly.
5. Note which states the real product has actually built.

**Done well when:** you find at least two states the shipped product does not handle. Overflow (what happens with a 90-character name, or 400 rows) and permission-denied are the most commonly missing.

---

### Drill 14 — Latency choreography

**Builds:** the difference between actual and perceived performance, and correct use of the Doherty Threshold.

**Time:** 15 minutes.

**Steps**
1. Find an operation in a real product that takes more than a second. Time it.
2. Classify it into a response band: under ~100 ms (feels instant), ~400 ms (the Doherty Threshold, where interaction stays fluid), 1–10 s (needs a determinate indicator), over 10 s (needs a way to leave and be notified).
3. Write what the interface currently does at each of: 0 ms, 100 ms, 1 s, and completion.
4. Redesign the sequence. Specify the immediate acknowledgement, the waiting treatment, and the completion feedback.
5. Decide whether the operation should be optimistic or pessimistic, and justify it by the cost of a failure.

**Done well when:** your redesign acknowledges the input in under 100 ms regardless of how long the operation takes, and your optimistic/pessimistic call is argued from reversibility — optimistic for likes and reorders, pessimistic for payments and irreversible deletes.

---

### Drill 15 — Undo instead of confirm

**Builds:** judgement about when to interrupt someone and when to let them proceed.

**Time:** 15 minutes.

**Steps**
1. List five destructive or consequential actions across products you use.
2. For each, note what the product currently does: confirmation dialog, typed confirmation, undo window, or nothing.
3. Decide what it *should* do, using three factors: reversibility of the underlying operation, frequency of the action, and the cost of the mistake.
4. Where you propose undo, specify the window length and where the undo affordance lives.

**Done well when:** you did not answer "undo" for all five. Undo is usually better than a dialog, but it is not available when the operation genuinely cannot be reversed, and a confirmation for a high-frequency action trains a dismissal reflex that makes the confirmation worthless anyway. Naming that trade-off is the skill.

---

### Drill 16 — Form teardown

**Builds:** the most commonly assigned take-home task in the field.

**Time:** 30 minutes.

**Steps**
1. Screenshot a real form with eight or more fields.
2. For each field ask: is it required, and can we get it later, infer it, or drop it entirely?
3. Check label placement and association, input types and keyboards, autocomplete attributes, validation timing, and what happens on error.
4. Check the tab order by walking it with the keyboard.
5. Rewrite the form as a list of fields in your proposed order, with the justification for every deletion and every grouping.

**Done well when:** you removed or deferred at least two fields and can defend it against the business reason they exist. Field removal is the highest-leverage change available in almost any form, and the interesting part of the drill is arguing for it, not spotting it.

---

### Drill 17 — Keyboard-only audit

**Builds:** the accessibility check with the best ratio of effort to findings.

**Time:** 20 minutes.

**Steps**
1. Put your mouse or trackpad physically out of reach. This matters.
2. Complete one meaningful task in a real product using only Tab, Shift+Tab, Enter, Space, Escape, and arrow keys.
3. Record: can you see where focus is at all times (2.4.7 Focus Visible); does focus order follow the visual order (2.4.3); can you reach and operate every control (2.1.1); can you always escape a component (2.1.2 No Keyboard Trap); does a sticky header ever hide the focused element (2.4.11).
4. Note every point where you got stuck, and what you would change.

**Done well when:** you completed the task or documented precisely where it became impossible. Custom dropdowns, modals, carousels, and date pickers are where this drill usually breaks, and a missing or removed focus indicator is the most common single finding in the whole discipline.

---

### Drill 18 — Motion specification

**Builds:** the ability to specify motion in a handoff rather than waving at it.

**Time:** 15 minutes.

**Steps**
1. Pick three transitions in a product: a modal opening, a list item being removed, a tab switching.
2. For each, write the specification an engineer could build from: what property changes, over what duration, with what easing, and what triggers it.
3. Ask of each: what does the motion *explain*? Where did the thing come from, where did it go, what is related to what?
4. Specify the reduced-motion behaviour for each.

**Done well when:** every animation you kept explains a spatial or causal relationship, and anything that was purely decorative is either cut or given a duration short enough to be invisible on the hundredth viewing. Motion that delights on first use and costs 300 ms on every subsequent use is a net loss.

---

## Research and synthesis

### Drill 19 — JTBD statements from quotes

**Builds:** synthesis — turning what people said into what they were trying to do.

**Time:** 25 minutes.

**Steps**
1. Take ten verbatim quotes. Use real interview transcripts if you have them; otherwise mine app-store reviews, support forums, or Reddit threads about a product.
2. For each, write a Job-to-be-Done statement in the form: **When [situation], I want to [motivation], so I can [expected outcome]**.
3. Cluster the ten statements. Name each cluster by the job, not by the user type.
4. Mark which statements you had to invent detail for.

**Done well when:** your statements are anchored in a *situation* rather than a demographic, and you can point at the words in the quote that justify each clause. The failure mode is writing a persona in JTBD clothing ("As a busy professional, I want…"), which smuggles an assumption about who the user is into what should be a statement about a circumstance.

---

### Drill 20 — Feature to problem statement

**Builds:** the reframing move that separates a designer from a ticket-taker, and the thing interviewers are testing when they hand you a solution.

**Time:** 20 minutes.

**Steps**
1. Collect five feature requests. Use a public roadmap, a changelog, or requests from your own team.
2. For each, ask "what would have to be true for this to be the right answer?" and then "what problem is this person actually experiencing?"
3. Rewrite each as a problem statement naming the user, the situation, the obstacle, and the evidence you would want.
4. For at least two, propose an alternative solution that addresses the same problem differently, and say what would distinguish the two empirically.

**Done well when:** your problem statements do not contain the original solution hiding inside them. "Users need a dashboard" is a solution; "users cannot tell whether last night's job succeeded without opening four screens" is a problem, and it admits answers other than a dashboard.

---

### Drill 21 — Write a survey question, then break it

**Builds:** an instinct for the ways self-report data goes quietly wrong.

**Time:** 20 minutes.

**Steps**
1. Write five survey questions on a topic you care about.
2. Now attack your own questions. For each, check: is it double-barrelled ("was checkout fast and easy?"); is it leading ("how much did you enjoy…"); is the scale balanced with a labelled midpoint and consistent direction; is it attitudinal where a behavioural question would be more reliable; would two respondents interpret it the same way?
3. Rewrite each question to survive its own critique.
4. Write one sentence on who will *not* answer this survey and how that biases the result.

**Done well when:** at least three of your five original questions failed, and you converted at least one attitudinal question ("how often do you usually…") into a behavioural one ("how many times did you do X in the last seven days?"). The non-response sentence is the part people skip and the part that most often invalidates the study.

---

### Drill 22 — Severity rating

**Builds:** the ability to hand a team a prioritised list rather than a pile of complaints.

**Time:** 20 minutes.

**Steps**
1. Take a list of ten usability findings — from your own heuristic evaluation, or generate them from any drill above.
2. Rate each on frequency, impact, and persistence, then assign an overall severity from 0 (not a problem) to 4 (catastrophic).
3. Sort the list by severity.
4. Now sort it again by severity *against implementation cost*, and write the three you would fix this sprint.
5. Justify one case where a lower-severity issue beat a higher-severity one on the second list.

**Done well when:** your ratings distinguish an issue everyone hits once and works around from an issue a few people hit and cannot recover from. Anything that loses a user's work should sit at the top regardless of frequency — protecting users' work is the highest-severity failure class in almost any product.

---

### Drill 23 — Method selection under constraint

**Builds:** the answer to "how would you research this?", which is asked in nearly every research-adjacent interview.

**Time:** 15 minutes.

**Steps**
1. Write down five research questions, deliberately varied: one generative, one evaluative, one about prevalence, one about causation, one about vocabulary.
2. For each, name the method, the sample size and how you derived it, and — critically — **the limitation you would state out loud**.
3. Then redo all five under a hard constraint: one week, no budget, no recruiting.
4. Say what you would pair each method with to triangulate.

**Done well when:** every answer names its limitation unprompted, and your no-budget versions use the free continuous evidence that already exists — search logs, support tickets, session recordings, analytics, and five colleagues in a corridor. Resourcefulness is the trait actually being scored.

---

### Drill 24 — The say-do gap hunt

**Builds:** healthy scepticism about attitudinal data.

**Time:** 15 minutes.

**Steps**
1. Find a public claim about user preference — a survey result, a press release, a "users told us" line in a blog post.
2. Write down what behavioural evidence would confirm it.
3. Write down what behavioural evidence would contradict it, and which you would expect to find.
4. Do the same for a claim you have made yourself about your own product or portfolio.

**Done well when:** you applied the same scrutiny to your own claim as to the stranger's. People misreport their behaviour, cannot predict their future behaviour, and rationalise their past behaviour, and that applies to designers describing their own process.

---

## Information architecture

### Drill 25 — Navigation reverse-engineering

**Builds:** the ability to see structure underneath a visual design.

**Time:** 20 minutes.

**Steps**
1. Pick a product with substantial navigation.
2. Write out its full hierarchy as an indented text tree, three levels deep, without looking at the visual design once you start.
3. Classify each navigation element: global, local, contextual, or utility.
4. Note every item whose label you could not confidently place, and every item that appears in two places (polyhierarchy — sometimes correct, often a symptom).
5. Write three tasks a user might have and trace the path for each.

**Done well when:** you found at least one label whose meaning you had to guess. That guess is the finding: it is exactly what a tree test would surface, and label ambiguity produces low directness even when success rates look acceptable.

---

### Drill 26 — Information scent trace

**Builds:** diagnosis of why people cannot find things even when the structure is correct.

**Time:** 15 minutes.

**Steps**
1. Choose a specific piece of content buried three or more levels deep in a real site.
2. Starting from the homepage, at each step write down which link you clicked and — before clicking — how confident you were on a 1–5 scale that it was the right one.
3. Note every point where confidence dropped below 3, and every point where you backtracked.
4. Rewrite the labels that caused the confidence drops.

**Done well when:** your rewritten labels use the user's vocabulary rather than the organisation's. Backtracking and pogo-sticking are the observable symptoms; weak scent at a specific label is the cause, and naming the specific label is what makes the finding actionable.

---

### Drill 27 — Card sort in miniature

**Builds:** familiarity with the method and with how much people's models differ from yours.

**Time:** 30 minutes.

**Steps**
1. Write 30 content items from a domain you know onto cards or sticky notes.
2. Sort them yourself into groups and name the groups. Photograph the result.
3. Get two other people to do an open sort of the same items independently. Do not show them yours.
4. Compare. Note every item that moved, every group name that differed, and every item that no one placed confidently.

**Done well when:** you can state which items are *stable* (everyone agrees) and which are *contested*, and you have a view on what to do about the contested ones — usually cross-listing, better labelling, or accepting that they will be found by search. Note that a card sort tells you how people group and name things; it does not tell you whether they can find things in your structure. That takes a tree test, and conflating the two is the classic screening-question failure.

---

## Accessibility

### Drill 28 — Screen reader first contact

**Builds:** the fastest possible route out of theoretical accessibility knowledge.

**Time:** 25 minutes.

**Steps**
1. Turn on the screen reader already on your machine — VoiceOver on macOS or iOS, Narrator on Windows, TalkBack on Android.
2. Turn the display brightness right down or close your eyes for the first pass.
3. Attempt one simple task on a real site.
4. Record: are images described usefully; do headings form a sensible outline you can navigate by; are form fields labelled; are custom controls announced with a name, a role, and a state (4.1.2); is a status update after an action announced at all (4.1.3)?

**Done well when:** you can name three specific things that made the experience worse and map each to a criterion. Expect this drill to be humbling the first three or four times; that is the point, and it converts accessibility from a checklist into a felt constraint.

---

### Drill 29 — Zoom and reflow

**Builds:** the low-vision check that almost nobody runs and that regularly breaks products.

**Time:** 15 minutes.

**Steps**
1. Take a real page and set browser zoom to 200% (1.4.4 Resize Text).
2. Then set the viewport to 320 CSS px wide equivalent and check for two-dimensional scrolling (1.4.10 Reflow).
3. Then apply increased text spacing — line height, letter spacing, word spacing, paragraph spacing (1.4.12 Text Spacing).
4. Record every place content is clipped, overlapped, hidden, or made unreachable.

**Done well when:** you tested a page with a fixed-height component, a sticky header, or a data table, because those are where reflow actually fails. A page of body text passing at 200% proves very little.

---

### Drill 30 — Target size and reach

**Builds:** applied Fitts's Law on touch, where the desktop intuitions do not transfer.

**Time:** 15 minutes.

**Steps**
1. On a phone, screenshot a screen with several tappable elements.
2. Measure each target. Grade against **24×24 CSS px** as the WCAG 2.2 AA minimum (2.5.8), noting that platform guidance recommends considerably larger.
3. Map the thumb arc for one-handed use and mark which targets fall outside it.
4. Note anything destructive that sits within easy reach, and anything frequent that sits outside it.
5. Propose a revised layout.

**Done well when:** you noticed that screen corners — the cheapest targets with a mouse, because the pointer is clamped by the screen edge — are among the *most expensive* on touch, where there is no clamping, the finger occludes the target, and reach dominates. That inversion is a standard interview question.

---

## Metrics, strategy, and judgement

### Drill 31 — Measurement plan for a shipped feature

**Builds:** the answer to "how would you measure the success of this design?", asked in essentially every product-design interview.

**Time:** 25 minutes.

**Steps**
1. Pick a feature that shipped recently in a product you use.
2. Run the GSM chain explicitly: **Goal** in user terms, **Signals** that would indicate progress, **Metrics** that count those signals.
3. Choose one primary metric and pair it with a guardrail that would catch the cheap way of moving it.
4. Write the perverse path: what would make this number improve for a bad reason?
5. Write who is invisible to this measurement — the people who never arrived, never loaded, or never got an event fired.
6. State the decision each number would change. Delete any metric that fails that test.

**Done well when:** you deleted at least one metric at step 6, and your guardrail is genuinely capable of catching the failure — conversion paired with refund rate, engagement paired with satisfaction, speed paired with error rate. A metric nobody would act on is reporting, not measurement.

---

### Drill 32 — Vanity metric autopsy

**Builds:** the ability to challenge a number politely and precisely.

**Time:** 10 minutes.

**Steps**
1. Find three metrics being reported publicly — in an investor update, a launch post, a company blog.
2. For each, decide whether it is vanity or actionable, using one test: can this number go *down*, and if it did, would we know what to do?
3. Rewrite each as an actionable equivalent: a rate rather than a total, a cohort rather than a cumulative, a per-user value rather than an aggregate.

**Done well when:** you can explain to a non-designer, in one sentence, why total registered users cannot inform any decision while week-four cohort retention can.

---

### Drill 33 — Second-order effects

**Builds:** the systems thinking that distinguishes senior judgement, and a favourite senior interview probe.

**Time:** 20 minutes.

**Steps**
1. Take any design change — yours or a shipped one.
2. Write the intended first-order effect.
3. Then write six second-order effects across four surfaces: on other users of the same product, on the support and operations teams, on the business incentives, and on user behaviour six months out.
4. Mark which of the six you would monitor, and how.

**Done well when:** at least two of your second-order effects are genuinely undesirable and you can still argue for shipping. Naming only the good downstream effects means you were advocating, not analysing. Internal tools and support workload are the surfaces designers most reliably forget.

---

### Drill 34 — Ethics stress test

**Builds:** a usable test you can apply in a real meeting, rather than a sentiment you cannot act on.

**Time:** 15 minutes.

**Steps**
1. Find three persuasive mechanics in the wild: a countdown timer, a low-stock badge, a streak, a pre-checked box, a friction-heavy cancellation flow.
2. Run each through three questions. **Is the constraint real** — is inventory actually held, does the price actually change? **Is it described accurately** — does the copy match the mechanism? **Does it survive scrutiny** — does the timer reset on reload, does the count change randomly?
3. Then apply the general test: does this help the user reach a goal *they* hold, and would we be comfortable explaining the mechanism to them?
4. For any that fail, write the version you would ship instead and the argument you would make to the person who asked for the original.

**Done well when:** you wrote the counter-proposal and the argument, not just the objection. Refusing without offering an alternative that meets the business goal is how designers lose these conversations, and the business goal — usually urgency, or retention — is almost always legitimate even when the mechanic is not.

---

## Choosing a drill

| If you have | Run |
| --- | --- |
| 10 minutes and a phone | 1, 2, 7, 9, 11, 32 |
| 15 minutes and a browser | 4, 12, 14, 15, 18, 24, 26, 29, 30, 34 |
| 20 minutes and quiet | 3, 8, 10, 13, 17, 20, 21, 22, 25, 33 |
| 25–30 minutes | 5, 16, 19, 27, 28, 31 |
| An interview this week | 8, 12, 13, 16, 20, 22, 23, 31, 33 |
| A portfolio to build | 3, 5, 16, 19, 25, 27, 31 |
| A specific weakness after a quiz | Whichever drill sits under that module's skill above |

Rotate. A drill you have run five times on five different products has taught you the skill; a drill you have run once has taught you the drill.

---

<!-- nav -->
[← Previous: Flashcards](../quizzes/flashcards.md) · [↑ Contents](../README.md) · [Next: Books →](../resources/books.md)
