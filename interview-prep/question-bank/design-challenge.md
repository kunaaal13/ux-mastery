# Design Challenge

## In one line

The whiteboard round tests whether you can take an under-specified problem, narrow it deliberately, generate options that are genuinely different from each other, and defend a choice — all out loud, in forty-five minutes, while someone changes the rules halfway through.

## What is actually being tested

| Signal | Weight | What the interviewer writes down |
| --- | --- | --- |
| **Problem framing** | Highest | "Narrowed to a defensible segment and said why" / "Designed for everyone, so designed for no one" |
| **Structured process** | High | "Had a visible spine and never lost the thread" / "Jumped straight to a screen at minute four" |
| **Divergence** | High | "Three genuinely different concepts" / "Three versions of the same concept" |
| **Trade-off reasoning** | High | "Named what each option costs" / "Argued only for the option they liked" |
| **Handling ambiguity** | Medium | "Made assumptions explicit and moved" / "Asked twelve clarifying questions and ran out of time" |
| **Communication under pressure** | Medium | "Thought out loud, easy to follow" / "Long silences, then a finished answer with no visible reasoning" |
| **Adaptability** | Medium | "Absorbed the new constraint and re-derived" / "Defended the original answer against the new facts" |

Note what is *not* on the list: drawing skill, and having the "right" answer. There is no right answer. There are answers whose reasoning you can reconstruct and answers whose reasoning you cannot.

## The prompt types

Four families, each with a different opening move.

### 1. "Design X for Y"

*"Design a vending machine for an airport." "Design a music app for runners." "Design a savings product for gig workers."*

The most open type. The whole game is narrowing. Y is given but is almost always too broad — "runners" contains a couch-to-5K beginner and a marathoner mid-training-block, and they want opposite products.

**Opening move:** confirm the goal, then narrow the user, then narrow the moment. "I am going to design for a specific moment, not the whole category, because that is where a differentiated product comes from."

### 2. "Improve X"

*"Improve the experience of returning an online order." "Improve the airport security queue." "Improve group messaging."*

Feels easier and is usually harder, because candidates skip framing and start listing tweaks. An improve prompt is a critique prompt fused with a design prompt: you must first say what is broken and for whom, with a stated theory of the failure, before proposing anything.

**Opening move:** state the current journey in five or six steps out loud, name where value is lost, and pick one step to attack. "Rather than improve everything by ten percent, I want to find the step that is losing the most people and change its shape."

### 3. "Design under a hard constraint"

*"Design this for offline use." "Design for one-handed use on a phone in bright sunlight." "Design for users who cannot read." "Design for a 2G connection and a device with 1 GB of RAM."*

The constraint is the point. Interviewers use these to see whether you can let a constraint *generate* the design rather than treating it as a filter applied at the end.

**Opening move:** turn the constraint into design consequences before touching a screen. Offline is not "cache things"; offline is a set of decisions about what can be composed without the server, what queues, what conflicts, and how the user knows which of their actions are real yet.

| Constraint | The real design questions it generates |
| --- | --- |
| **Offline / flaky** | What is authorable offline? What queues and in what order? How is queued-versus-synced shown? What happens on conflict? What must never be attempted offline (payments, bookings against shared inventory)? |
| **One-handed** | Where is the thumb arc on the target device? What moves to the bottom? What becomes a sheet rather than a top bar? Which gestures are reachable and which need a fallback? |
| **Low literacy** | Which decisions can become recognition rather than reading? What carries meaning without text — icon plus colour plus position, never one alone? What must be voiced? How do you avoid a design that feels condescending to a numerate adult who simply cannot read this script? |
| **Low bandwidth / low-end device** | What is the first meaningful paint? What is deferred? Image strategy? Is there a text-only or SMS path? What does a 40-second load look like as a designed state rather than a spinner? |
| **Bright sunlight / gloves / motion** | Contrast floors, target sizes, error tolerance, whether precision input is possible at all |
| **Regulated (health, finance)** | What must be disclosed, when consent is captured, what cannot be defaulted, what must be auditable |
| **Shared device** | Whose data is on screen, how do you switch users cheaply, what is private by default |

### 4. The metric prompt

*"Activation is 20%. Fix it." "Retention drops off a cliff at week two." "Support contacts per order are up 30% since the redesign."*

Half design, half analysis. The trap is jumping to redesign. The winning structure is diagnosis first, and the reusable frame is the three-way split from Module 12: users who **cannot** (usability or technical failure), users who **will not** (value not clear, or the ask comes too early), and users who **should not** (wrong users acquired — no onboarding change fixes this).

**Opening move:** interrogate the metric's definition before its value. "First, is activation defined as the moment of first value, or as finishing the tour? Those give completely different diagnoses, and the second one is frequently the actual problem."

Then: segment (platform, channel, geography, cohort), locate the step, split cannot/will not/should not, and only then design — for one segment, at one step.

## How to clarify without stalling

Clarifying questions are scored, but there is a sharp diminishing return. Three to five good questions in the first three minutes reads as rigour. Ten reads as stalling or as an inability to act without permission.

**The rule: ask only questions whose answer would change your design. If any answer leads you to the same place, do not ask it — assume and move.**

The four questions almost always worth asking:

1. **Goal.** "What is the business trying to achieve here — growth, retention, cost reduction, or entering a new segment?" This one changes everything downstream and is rarely volunteered.
2. **Scope of platform and channel.** "Am I designing an app, a web flow, or something that also has to work over SMS or in person?"
3. **Existing or greenfield.** "Is this a new product, or a feature inside something people already use? If it is inside something, what do they already come for?"
4. **What is off the table.** "Are there constraints I should know — no hardware, no new data collection, must ship this quarter?"

Everything else: assume, say the assumption out loud, and offer to revisit.

> "I do not need to know the exact market to start, so I will assume a mid-size city in a country with high smartphone penetration but patchy connectivity, and I will flag it if that assumption starts doing real work in the design."

That sentence is worth more than the answer would have been, because it demonstrates the judgement the question would have outsourced.

**The stalling tells to avoid:** asking for data the interviewer obviously does not have; asking a question you then ignore; asking three questions in a row without saying why any of them matter; and treating the interviewer as a stakeholder to be satisfied rather than a colleague to think with.

## Picking a user segment and defending it

This is where most challenges are won or lost, and it takes ninety seconds.

**The move:** name two or three plausible segments, state what makes them different in a way that *matters for design*, pick one, and give a reason grounded in either user need or business value.

> "For a public-transport ticketing app there are at least three users: the daily commuter who knows the network and wants speed, the occasional local traveller, and the first-time visitor who does not know the network, the fare structure, or the language. Those are not variations of each other — the commuter's core problem is friction on a known task, and the visitor's core problem is not knowing what they do not know. I am going to design for the first-time visitor. Two reasons: the failure cost is highest there, because a confused visitor either does not travel or travels without a valid ticket, and it is where the operator's cost of service — staff answering questions at machines — actually lives. The commuter is better served by a season pass and a card tap, which is a different product."

Three things happened in that paragraph: segments were named and differentiated, one was chosen, and the choice was justified on both user need and business value. That is the whole move.

**How to defend it when challenged.** Interviewers will push. "Why not the commuter, that is 90% of volume?" The correct answer is not to switch and not to dig in blindly:

> "Volume is the argument for the commuter, and if the goal were total transactions I would agree. I chose the visitor because the marginal design work per unit of value is much higher — the commuter already has a working solution and I would be shaving seconds. If you tell me the goal is commuter retention against a competing payment method, I would switch and I would design something quite different, closer to a wallet than a journey planner. Do you want me to take that path instead?"

You have held your reasoning, exposed the condition under which you would change, and handed control back. That is a senior signal.

## Generating genuinely different concepts

The single most common failure: three "concepts" that are the same idea with the buttons in different places.

A test you can apply live: **if two concepts could be A/B tested against each other and the losing one's team would say "fine, just move the button", they are not different concepts.** Real alternatives differ on a structural axis.

Axes that produce real divergence:

| Axis | Concept A | Concept B |
| --- | --- | --- |
| **Who does the work** | User specifies everything | System infers and user corrects |
| **When it happens** | Up front, once | Progressively, in context, at point of need |
| **Input modality** | Typed / tapped | Scanned, spoken, photographed, or NFC |
| **Unit of interaction** | The individual item | The batch or the recurring rule |
| **Where it lives** | In-app | Outside the app: SMS, wallet pass, kiosk, notification, printed |
| **Social shape** | Solo | Shared, delegated, or assisted by another person |
| **Business model shape** | Pay per use | Subscription, prepay, or postpay |
| **Automation stance** | Manual with full control | Automatic with an undo |

The practical method: **pick one axis, generate three points along it, and name each concept in four words.** Names matter because a named concept can be discussed and compared; an unnamed sketch cannot.

> "Concept one, 'Ask me three questions' — the system asks the minimum needed and infers the rest. Concept two, 'Point the camera at the sign' — no typing at all; the input is the physical world. Concept three, 'Buy it at the barrier' — the ticket does not exist until you tap, so there is no purchase decision at all. They differ on where the knowledge lives: in the user, in the environment, or in the system."

Then evaluate against explicit criteria before choosing. Criteria worth naming: fit to the chosen need, time-to-first-value, technical feasibility, cost to operate, accessibility, and failure mode when it does not work.

## Sketching legibly

Nobody is scoring your line quality. They are scoring whether the artefact helps them follow you.

**On a physical whiteboard**

- Write large. If it is not readable from three metres it is not readable on a video feed either.
- Divide the board deliberately at the start: a strip for goal and assumptions, a strip for user and needs, a large area for concepts, a corner for the parked list. Never erase the goal strip.
- One box per screen, roughly phone-proportioned, with the screen's name written above it. Draw four to six boxes with arrows between them rather than one detailed screen.
- Use a consistent shorthand: a box with an X for an image, three horizontal lines for a text block, a rounded rectangle for a button, a circled number for a step in your narration.
- Boxes and arrows first, contents second. Flow before pixels.
- Say what you are drawing while you draw it. Silence while sketching is dead air the interviewer cannot score.

**On a remote board**

- Use rectangles, text and connectors only. Do not fight the tool's pen; freehand on a trackpad is unreadable.
- Keep everything in one viewport region and do not zoom around; the interviewer's view may not follow yours.
- Type your headings — assumptions, segment, needs, concepts, criteria — as text blocks before you start. It gives the session a visible spine and doubles as your notes.
- Screen-share your cursor deliberately: point at what you are talking about.
- Have a template ready: a blank frame with those five headings and a row of six empty phone-sized rectangles. Building it live wastes four minutes.

**Time discipline for the artefact:** a concept should take under three minutes to draw. If you are still drawing at minute five, you are decorating.

## When the interviewer adds a constraint mid-way

This is deliberate and it is one of the highest-signal moments in the interview. Typical injections: "now assume the user has no smartphone", "now assume this has to work for 10 million users on day one", "the CEO says it must launch in six weeks", "legal says you cannot store the address".

**What they are testing:** whether your design has a *reasoning structure* you can re-run, or whether it was a memorised artefact. If the constraint destroys your answer, your answer was a picture rather than a decision tree.

**The four-step response:**

1. **Acknowledge and restate.** "So no smartphone. Let me make sure I have it: the user has a feature phone with SMS, or no phone at all?" One clarifying question is allowed here; two is stalling.
2. **Say what survives.** "The need does not change — they still need to know which ticket is valid for this journey and to prove it at the barrier. What changes is the channel."
3. **Say what breaks, explicitly.** "The camera concept dies entirely. The progressive-inference concept survives but loses its interface, so it would have to become a scripted SMS exchange or a kiosk flow."
4. **Re-derive, do not restart.** Take the surviving concept down the new path, and say the new cost. "That means the visitor's ticket becomes a code they show, which puts load on the barrier staff — so I would want the code to be checkable offline by a handheld scanner, and that is now the critical dependency."

The sentence that scores best in this moment:

> "That is actually a better constraint than the one I gave myself, because it forces the design toward the shared-infrastructure version rather than the app version — and the app version was quietly assuming a data plan I have no evidence for."

Two failure modes to avoid. **Collapsing** — "oh, then none of this works" and starting from zero, which wastes the twelve minutes you have left. **Ignoring** — carrying on with the original design and mentioning the constraint decoratively at the end.

## Worked example one — public-transport ticketing for first-time users

*45-minute format. CIRCLES path, narrated. Timings in the margin are the real ones to aim for.*

### C — Comprehend the situation (0–4 min)

"Let me play back the prompt: design a ticketing app for a city's public-transport network, and I am going to hold the focus on first-time users unless you want otherwise.

Four questions. What is the operator's goal — revenue, fare compliance, reducing staffing at stations, or shifting people off cash? Is this greenfield or does an app already exist? Does it need to cover bus and metro or one mode? And is contactless bank-card tap already supported at the barriers, because if it is, this product is a very different thing.

*[Assume answers: goal is fare compliance plus reduced station staffing; greenfield; multi-modal; no contactless bank tap yet.]*

Good, that helps a lot. Fare compliance plus staffing cost means the operator's pain is people who cannot work out what to buy — they either avoid travel, buy the wrong thing and get fined, or queue at a window. So the business problem and the first-time-user problem are the same problem, which is unusually convenient.

Assumptions I am making and will flag if they matter: smartphone penetration is high but connectivity underground is poor; there is a mix of languages; fares are zone-based rather than flat, because that is what makes this hard."

### I — Identify the customer (4–7 min)

"Three candidate segments: the daily commuter, the occasional local, and the first-time visitor — where 'visitor' includes a tourist, a new resident in their first month, and someone travelling a route they have never taken.

I am choosing the first-time user. The commuter's problem is speed on a known task and is best solved by a pass and a tap, not by an app flow. The first-time user's problem is that they do not know the fare structure, the zones, the validity rules or which of the six ticket types applies to them. That is a knowledge problem, and knowledge problems are what software is good at. It also maps directly onto both operator goals: fines and window queues are concentrated in exactly this group."

### R — Report the customer's needs (7–12 min)

"Let me write the journey as the user experiences it, then attach needs to steps.

| Step | What the user is doing | Need | Current failure |
| --- | --- | --- | --- |
| 1 | Deciding whether to travel by transit at all | Confidence that this is doable and roughly what it costs | Opaque; they take a taxi |
| 2 | Standing at the station facing a machine or an app | Know *which* ticket is valid for *this* journey | Six product names, none of which map to a journey |
| 3 | Paying | A payment method that works for a foreign card or cash | Card declined, no cash acceptance, no alternative |
| 4 | Passing the barrier | Proof that works, fast, possibly with no signal | QR that will not load underground |
| 5 | Interchange or a second leg | Know whether the ticket still covers them | No answer available in the moment |
| 6 | Something goes wrong — wrong zone, expired, gate rejects | Recover without a fine and without shame | Confrontation with staff in a second language |

The needs behind those, stated as needs rather than features: *know what to buy without understanding the fare system*; *pay with what I have*; *prove it without connectivity*; *not be punished for a mistake I could not have avoided*.

The insight I want to build on: the user does not want a ticket. They want to make a journey and not be in trouble. Every existing product sells the first thing."

### C — Cut through prioritisation (12–15 min)

"I am going to prioritise steps 2 and 4 — choosing the right ticket, and proving it at the barrier offline.

Why those. Step 2 is where the knowledge gap actually bites and where every wrong outcome downstream originates. Step 4 is where the design fails catastrophically rather than annoyingly — a QR that will not load at a barrier with a queue behind you is a memorable failure that stops people using the product again. Step 3, payment, matters enormously but is largely a partnerships and payments-rails problem rather than a design one, so I will note it and set it aside.

I am explicitly deprioritising route planning. Map products already solve it well and I do not want to compete with them badly."

### L — List solutions (15–27 min)

"Three concepts, differing on where the knowledge lives.

**Concept A — 'Tell me where you are going.'** The knowledge lives in the system. The user enters or picks a destination; the app returns exactly one recommended ticket with a plain-language sentence: 'This covers you from here to Central, on metro or bus, until 18:40.' No product names, no zone map. One button: buy.

*Sketch:* two screens. Screen one is a single large field, 'Where are you going?', with three suggested nearby destinations underneath. Screen two is a card showing the plain sentence, the price, and a full-width buy button, with a small 'why this ticket' link beneath.

*Strengths:* removes the fare system from the user's head entirely; the single-recommendation model means there is no comparison task. *Costs:* needs a fare engine that is genuinely correct, and being wrong is worse than being unhelpful; requires a destination the user can name, which fails if they only know a landmark.

**Concept B — 'Point your camera at it.'** The knowledge lives in the environment. The user photographs the station sign, the route number on the front of the bus, or the printed fare board; the app resolves location and destination context and offers the ticket. No typing, works across languages.

*Sketch:* camera viewfinder with a reticle, an overlay confirming 'Northgate station, zone 2', then the same recommendation card as A.

*Strengths:* the lowest literacy and language demand of the three; solves 'I do not know what this place is called'. *Costs:* fails at night, in crowds, and where signage is poor; camera permission is a real drop-off point; it is a novel interaction that needs teaching.

**Concept C — 'Just travel, we will work it out.'** The knowledge lives nowhere until afterwards. The user registers a payment method once, gets a tokenised pass, taps in and out, and is charged the correct — and capped — fare at the end of the day. There is no ticket-selection decision at all.

*Sketch:* one screen: a large pass with a tap animation and 'today: 2 journeys, £4.20, capped at £5.60'.

*Strengths:* eliminates the hardest problem rather than solving it; matches what the commuter wants too, so it is one product for both segments; strongest fare-compliance story. *Costs:* by far the heaviest — needs barrier hardware support, a settlement system, and a way to handle a foreign card or a user with no card at all; and it removes price certainty before travel, which is exactly what an anxious first-time user wants.

Those three genuinely differ. A is inference, B is sensing, C is deferral."

### E — Evaluate trade-offs (27–36 min)

"Criteria, weighted by the goals we agreed: correctness of outcome, time to first successful journey, works offline at the barrier, accessibility and language independence, operator cost, and implementation weight.

| | A: Tell me where | B: Camera | C: Tap and cap |
| --- | --- | --- | --- |
| Correct ticket | High, if fare engine is right | High | Guaranteed by definition |
| Time to first journey | ~30 s | ~15 s when it works | ~60 s setup, then zero |
| Works at the barrier offline | Yes, with a locally-signed pass | Yes, same | Depends entirely on barrier hardware |
| Language / literacy independence | Medium — needs a destination name | High | High |
| Operator cost reduction | Good | Good | Best |
| Implementation weight | Medium | Medium-high | Very high |
| Price anxiety before travel | Answered | Answered | Not answered |

I would recommend **A as the shipped product, with B as a secondary entry point into it, and C as the two-year direction.**

Reasoning: A and B are the same recommendation engine with different front doors, so building A first and adding B later is genuinely incremental rather than a pivot. C is where the category is going and I would not want the architecture to preclude it — specifically, I would build the fare engine as a service that can price a completed journey, not only a prospective one, because that is the same engine C needs.

The offline requirement drives one concrete decision across all three: the pass must be a locally-stored, cryptographically-signed credential rendered as a rotating code, not a QR fetched from the server. That is a design decision with an engineering shape, and it is the one I would fight for, because it is the difference between working at the barrier and not."

### S — Summarise (36–40 min)

"To summarise: I focused on the first-time user because their knowledge gap is also where the operator's fine revenue and staffing cost concentrate. Their real need is not a ticket but the confidence that this journey is covered. I recommended a single-recommendation model — tell us where you are going, get one plainly-described ticket — with a camera entry point to remove the language barrier, and a locally-signed offline credential so the barrier never depends on connectivity.

**Success metrics.** Primary: percentage of first sessions that end in a completed journey with a valid ticket. Secondary: time from app open to ticket purchased; barrier rejection rate; window-queue volume at the three busiest stations; fine issuance to first-time users.

**What I would validate first.** Two things. One, whether users can name their destination in a way our system resolves — I would run a fifteen-person test at a station with a paper prototype, because if that fails, concept A collapses and B becomes the primary. Two, whether the single-recommendation model creates anxiety rather than removing it; some users need to see they were not overcharged, so I would test the 'why this ticket' disclosure with and without."

### Follow-ups you should expect

- *"You have made the fare engine responsible for correctness. What happens when it is wrong?"* — Answer with the recovery design: a stated guarantee ("if we recommended it, we cover the difference"), an in-app path at the barrier, and instrumentation that catches systematic mispricing.
- *"How does this work for someone with no smartphone?"* — The mid-way constraint. Re-derive: a kiosk running the same single-recommendation flow, and a printed code, with the credential logic unchanged.
- *"You deprioritised payments. Defend that."* — "It is the highest-risk item and the least design-shaped. I would rather name it as the critical dependency than pretend a screen solves it."

## Worked example two — an internal tool for support agents

*Compressed narration. Internal tools reward different instincts: efficiency over delight, error cost over aesthetics, and a real user you can go and sit with.*

### Comprehend (0–4)

"Questions: what does the support org measure — handle time, first-contact resolution, or CSAT? Are agents specialists or generalists? What is the current tool, and are they using it alongside three others? And is there an escalation path with a different team?

*[Assume: measured on first-contact resolution and CSAT, handle time watched but secondary; generalists; current tool is a ticket queue plus a separate admin console plus a knowledge base in a wiki; escalation to engineering exists and is slow.]*

That combination tells me the interesting problem immediately: the agent's work is spread across three systems, and first-contact resolution is a metric you cannot hit while alt-tabbing. My assumption is that the design problem is context assembly, not the ticket list."

### Identify (4–7)

"Users: the front-line generalist agent, the specialist or escalation agent, the team lead, and — invisibly — the customer on the other end. I am designing for the front-line generalist, because they handle the volume, they have the least context, and their tenure is short so learnability actually matters. A tool that only works for the two-year veteran is a hiring liability."

### Report needs (7–12)

"Shadowing would give me the real list; from what we have assumed, the journey is: ticket arrives → work out who this customer is and what state their account is in → work out what the policy says → act → write it up → close or escalate.

| Step | Need | Where the time goes |
| --- | --- | --- |
| Identify customer | Full account state in one place | Copy-pasting an ID between three tools |
| Diagnose | Recent events: what did this person actually do | Not available at all; agent asks the customer |
| Find policy | The correct, current answer | Wiki search, stale pages, asking a colleague in chat |
| Act | Perform the change safely | Admin console with destructive actions and no confirmation |
| Write up | Record it without retyping | Free-text notes nobody can query later |
| Escalate | Hand over with enough context | A paragraph the engineer has to interrogate |

The need underneath: *see everything relevant about this person without asking them, and act without leaving the conversation.*"

### Cut through (12–15)

"Prioritising diagnosis and action. Rationale: first-contact resolution is the metric, and the two things that break it are 'I do not know what happened to you' and 'I cannot fix it from here'. Write-up matters for the org but not for the metric on the table; I will handle it as a by-product rather than a task."

### List solutions (15–26)

"Three concepts, differing on how much the system decides.

**Concept A — 'One screen, three panes.'** Conversation on the left, customer context in the middle — account state plus a chronological event timeline of what the customer actually did — and actions on the right, scoped to what this agent is permitted to do for this account. Nothing opens in a new tab.

*Trade-off:* highest information density, most screen real estate needed, and it demands that every action be exposed through an API the tool can call — which is the real cost and it is an engineering programme, not a design one.

**Concept B — 'Answer first.'** The system reads the ticket, matches it to a known issue class, and opens with a proposed diagnosis, the relevant policy excerpt, and a pre-filled action the agent approves or rejects. The agent's job becomes verification rather than investigation.

*Trade-off:* enormous speed win when the classification is right; when it is wrong it produces confident errors and agents learn to click through without reading — an automation-complacency risk that has to be designed against with a forced-verification step on anything irreversible.

**Concept C — 'Guided playbooks.'** The tool offers a checklist for each issue type: the agent picks 'refund request', gets a five-step guided flow with the policy inline, the required checks as explicit steps, and the write-up generated from the steps taken.

*Trade-off:* best for a new agent and best for consistency and auditability; slower and patronising for an experienced agent; and playbooks rot unless someone owns them.

These differ on who holds expertise: the interface (A), the model (B), or the process (C)."

### Evaluate (26–35)

"| | A: Three panes | B: Answer first | C: Playbooks |
| --- | --- | --- | --- |
| First-contact resolution | Good | Best when accurate | Good, consistent |
| Handle time | Good | Best | Worse for veterans |
| New-agent ramp | Medium | Poor — hides the reasoning | Best |
| Error cost | Agent-caused, visible | Automation errors, invisible | Lowest |
| Auditability | Weak unless designed | Weak | Strong by construction |
| Build cost | High (API surface) | High (model plus API) | Medium |

Recommendation: **A as the platform, C layered on top for the top ten issue types, B deferred.** A is the substrate — none of the others are possible while the data lives in three systems, so it is the unavoidable first investment. C rides on A cheaply and directly serves the short-tenure generalist. B is attractive and I would not build it until A has produced enough structured event data to make the classification trustworthy; shipping a confident wrong answer to an agent who then tells a customer is a worse failure than a slow answer.

One cross-cutting decision: every destructive action needs a preview-and-confirm with a plain statement of the consequence and the customer's name in it, plus an undo window where the operation permits. Support agents work under time pressure on someone else's account — that is exactly the condition under which slips happen (Module 02)."

### Summarise (35–40)

"Summary: the front-line generalist's problem is not the queue, it is that context and capability are split across three systems, so I unified them into one screen with a customer event timeline and inline scoped actions, then added guided playbooks for the top issue types so a two-week-old agent can resolve on first contact.

**Metrics:** first-contact resolution as primary; handle time and tool-switches-per-ticket as inputs; escalation rate and escalation-return rate as quality guards; CSAT as the outer check; and, for the playbooks, adherence and time-to-competence for new agents.

**What I would validate:** I would sit with six agents for a full shift before drawing anything, and specifically count tool switches and time-to-context per ticket, because my entire framing rests on the claim that context assembly is the bottleneck. If it turns out the bottleneck is waiting for engineering escalations, this is the wrong design and the right one is about the escalation handoff."

## Worked example three — a feature for a low-connectivity market

*Prompt: "Design a way for small shopkeepers to record credit sales — goods sold on account to regular customers — in a market with intermittent 2G, low-end Android devices, and mixed literacy."*

### Comprehend (0–4)

"Questions: is the shopkeeper the only user, or does the customer interact too? Is there an existing paper practice? Is money ever moved digitally, or is this purely a record? And do we need the record to be legally or socially binding between the two parties?

*[Assume: shopkeeper is primary, customer sometimes present; there is a paper ledger practice already, universal and trusted; no digital money movement in v1; the record must be credible to both parties because disputes are the pain.]*

The paper ledger detail is the most important thing said so far. There is an existing behaviour that works, is trusted, and is fast. Anything I design competes with a notebook and a pen, and notebooks have perfect uptime, zero latency and no charging requirement. If my design is not faster than the notebook at the counter, it will not be used, regardless of what it does afterwards."

### Identify (4–7)

"The shopkeeper. Specifically, a shopkeeper running a single small store, recording maybe ten to forty credit entries a day, often mid-transaction with a queue, sometimes with hands occupied, on a shared or low-end device, with variable literacy and near-universal numeracy — that distinction matters enormously and is frequently missed. People who cannot read fluently generally handle money and quantities extremely well."

### Report needs (7–12)

"| Moment | Need | Constraint that bites |
| --- | --- | --- |
| Recording a sale at the counter | Enter it in under five seconds without stopping the transaction | Hands busy, queue waiting, may be no signal |
| Finding a customer's balance | Instant, by person, no scrolling | Names may be ambiguous or unwritten |
| Reminding a customer to pay | Do it without damaging the relationship | Social cost is the real barrier, not the mechanism |
| Settling a payment | Adjust the balance, both parties satisfied | Disputes about what was entered |
| Trusting the record | Believe it will still be there tomorrow | Phone loss, shared device, uninstall |

The dominant need is speed at the counter. The second is dispute-proofing, because the reason ledgers cause pain is disagreement, not arithmetic."

### Cut through (12–15)

"Prioritising the entry moment and the shared-trust moment. Everything else — reports, analytics, reminders at scale — is downstream of having a record that both parties believe."

### List solutions (15–26)

"All three are offline-first by construction: entries are written locally, are immediately valid, and sync opportunistically. Sync state is shown per entry as a small, consistent marker rather than a modal. Nothing in v1 is allowed to require a round trip.

**Concept A — 'Face and amount.'** The customer list is a grid of large photo tiles rather than names, ordered by recency. Tap a face, type the amount on a full-screen numeric keypad, done. Two taps and a number. Literacy demand: near zero. Names are optional metadata.

*Trade-off:* photos require consent and are socially awkward in some contexts; a grid degrades past about forty customers and needs a search fallback, which reintroduces text.

**Concept B — 'Voice ledger.'** Hold a button and say "two hundred to Ramesh"; the app transcribes, shows a large confirmation card with the number and the face, and the shopkeeper taps to accept. Hands-free-ish, extremely fast, works in the local language.

*Trade-off:* on-device speech for the target languages on a low-end phone is the whole feasibility question, and a market counter is a noisy environment; the confirm step is mandatory, which claws back some of the speed advantage but is non-negotiable because a mis-transcribed amount is exactly the dispute we are trying to prevent.

**Concept C — 'Two-party receipt.'** Entry is the same as A, but on completion the customer's phone receives an SMS with the entry and the running balance, and if they have no phone the shopkeeper turns the screen for a co-sign tap. The record is jointly witnessed at the moment of creation.

*Trade-off:* SMS costs money per message and depends on having the customer's number; the co-sign adds three seconds at the counter. But it directly attacks the dispute problem rather than the recording problem.

They differ on what the design treats as the real problem: input effort (A), input modality (B), or trust between two people (C)."

### Evaluate (26–35)

"| | A: Faces | B: Voice | C: Two-party |
| --- | --- | --- | --- |
| Time at counter | ~4 s | ~3 s plus confirm | ~7 s |
| Literacy demand | Very low | Very low | Low |
| Works offline | Fully | Fully, if speech is on-device | Entry yes, notification queues |
| Dispute resistance | Low | Low | High |
| Low-end device fit | Good; photos need aggressive compression | Poor to medium | Good |
| Feasibility in v1 | High | Low | Medium |

Recommendation: **ship A, layer C's co-sign as an optional step, and treat B as a later input mode rather than a concept.** A is feasible now and wins the only fight that matters, which is against the notebook. C's co-sign is a three-second addition that turns the product from a private record into a shared one, which is what makes it worth switching from paper — and it is the part a competitor cannot copy cheaply, because it is a social mechanic rather than a feature.

Constraint-driven decisions I want to state explicitly, because they are the actual content of this design:

- **Every write is local-first and instantly valid.** The user is never blocked, never sees a spinner on entry, and never loses an entry to a failed request. Sync is a background fact, surfaced as a small per-row state.
- **No destructive sync conflicts.** Entries are append-only; a correction is a new entry that references the old one, never an in-place edit. This is a data-model decision that exists purely to protect the trust story.
- **Photos are compressed hard and cached on device**; the grid must render from local storage with zero network.
- **Text is never the only carrier of meaning** — amount, face and colour together. But the tone stays adult: no cartoons, no simplified language that reads as talking down to a competent businessperson.
- **Backup is a first-class feature, not a setting.** A shopkeeper who loses the phone and loses the ledger has been actively harmed. Recovery via phone number needs to work from day one, and I would say so on the very first screen because it is the main objection to leaving paper."

### Summarise (35–40)

"Summary: the competitor is a notebook, so the design target is under five seconds at the counter with no network and no reading. I designed a face-tile entry model, made the data append-only and local-first so nothing is ever blocked or lost, and added an optional customer co-sign to convert a private record into a jointly-witnessed one, which is the reason to switch from paper at all.

**Metrics:** entries recorded per active shop per day as the usage signal; median time-per-entry as the design signal; week-four retention of shops as the value signal; and disputes reported or corrections filed as the quality signal. I would also watch the ratio of app entries to estimated real credit sales, because partial adoption — using the app for some customers and paper for others — is the failure mode that kills this category.

**What I would validate:** first, time-per-entry against a stopwatch at a real counter during a busy hour, because every claim I have made depends on it. Second, whether the co-sign is socially acceptable or whether asking a regular customer to tap your phone reads as distrust — that is a cultural question I cannot answer from here, and it decides whether C survives."

## Twenty-five practice prompts

Run each in 40 minutes with the CIRCLES spine. Write the summary out loud before you look at your notes.

### Easy — one clear user, familiar domain

| # | Prompt | The trap |
| --- | --- | --- |
| 1 | Design an alarm clock for people who habitually oversleep | Solving "wake up" instead of "get out of bed"; the real design is the friction after the alarm |
| 2 | Design a way to split a restaurant bill among friends | Designing the arithmetic, not the awkwardness |
| 3 | Improve the experience of returning an online order | Improving the form; the value is in the collection logistics and the refund timing |
| 4 | Design a reading-list app for someone who saves articles and never reads them | Building better saving; the problem is retrieval and occasion |
| 5 | Design a water-tracking feature | Assuming the user wants tracking; they want the outcome |
| 6 | Improve the process of booking a doctor's appointment by phone | Digitising a call rather than asking what the call is for |
| 7 | Design a way to remember people's names at a conference | Treating it as a database problem rather than a moment-of-recall problem |
| 8 | Design a grocery list for a household of four | Ignoring the multi-user, real-time, at-the-shop context |

### Medium — segment ambiguity, real trade-offs

| # | Prompt | The trap |
| --- | --- | --- |
| 9 | Design a savings product for people with irregular income | Applying a monthly-salary mental model to people who do not have one |
| 10 | Design an onboarding flow for a product whose value takes two weeks to appear | Optimising signup instead of designing the two weeks |
| 11 | Improve the airport security queue experience | Designing signage; the leverage is in expectation-setting and predictability |
| 12 | Design a tool for teachers to give feedback on 120 essays | Ignoring that the constraint is the teacher's time, not the interface |
| 13 | Design a used-goods marketplace for a city with no reliable postal service | Skipping the meet-up safety and trust design |
| 14 | Our activation is 20%. Diagnose and fix it | Redesigning onboarding before defining activation |
| 15 | Design a group-travel planning feature | Designing for the organiser only |
| 16 | Design a medication-adherence aid for an elderly user living alone | Patronising design; ignoring the carer as a second user |
| 17 | Design a way for a restaurant to take orders without waiters | Designing for the diner and forgetting the kitchen's throughput |
| 18 | Improve the second-week retention of a fitness app | Attacking motivation with notifications instead of designing a smaller commitment |

### Hard — hard constraints, multi-sided, or ethically loaded

| # | Prompt | The trap |
| --- | --- | --- |
| 19 | Design a banking app for users who cannot read | Icons-only design that is unusable; ignoring that numeracy and literacy are different |
| 20 | Design a messaging feature that works on a 2G connection with 30-second latency | Retro-fitting an existing chat model; the fix is a different conversational unit |
| 21 | Design the dispute-resolution flow for a two-sided marketplace | Designing for the complainant only; ignoring the appeal and the abuse vector |
| 22 | Design a feature that reduces time-in-app without reducing revenue | Refusing to engage with the business tension; state it and design within it |
| 23 | Design a shared-device experience for a family that includes a child | Privacy, profile switching, and the fact that the child will find every workaround |
| 24 | Design an offline-first field-data-collection tool for surveyors | Sync conflicts, partial submissions, and 8-hour shifts with no charging |
| 25 | Design the consent experience for a product that must collect location continuously | Dark patterns; the hard version is meaningful consent that people still accept |

**Self-marking after each run.** Did you narrow to one segment and defend it in under ninety seconds? Were your three concepts different on a named axis, or the same idea rearranged? Did you name at least one cost for every option, including the one you chose? Did you state a primary metric and one thing you would validate first? Did you finish, or run out of time before the summary? Finishing badly beats not finishing.

## Check yourself

1. Name the four prompt types and the opening move for each.
2. What is the test for whether two concepts are genuinely different?
3. Give the rule for which clarifying questions are worth asking, and the four almost always worth asking.
4. Write, in one paragraph, a defence of a chosen segment that includes both user need and business value.
5. Give the four-step response to a constraint injected mid-way.
6. State the CIRCLES stages and roughly how many of your 45 minutes each should take.

---

<!-- nav -->
[← Previous: App Critique](app-critique.md) · [↑ Interview Prep](../README.md) · [Next: Fundamentals — Rapid-Fire Concept Questions →](fundamentals.md)
