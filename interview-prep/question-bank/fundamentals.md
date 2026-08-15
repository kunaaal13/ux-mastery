# Fundamentals — Rapid-Fire Concept Questions

## How to use this

Sixty-plus concept checks with model answers, grouped by topic. These are the questions that open rounds, fill gaps between deeper exercises, and get fired at you by a cross-functional interviewer who wants to know whether you actually understand the vocabulary you use.

**Answer length:** two to five sentences. Longer and you sound like you are auditioning; shorter and you sound like a flashcard. The model answers below are at the upper end — trim to taste.

**The trap column matters more than the answer.** Many of these questions are asked precisely because there is a popular wrong answer. Where a trap exists it is flagged. Getting the trap right is worth more than getting the definition right, because the definition is on Wikipedia and the trap is not.

**A rule that applies to every answer on this page:** state the principle, then state what it costs. A principle presented as free reads as junior. Interviewers are listening for the second half.

---

## Process and foundations

### 1. What is UX design?

> "The design of the whole experience of using something to achieve a goal — the flow, the structure, the language, the feedback, and how it fits into what the person was actually trying to do. UI is one part of it. In practice most of my time goes on deciding what should exist and in what order, rather than on how it looks. It's also not only digital: the return process for an online order is UX, and half of it is a cardboard box."

### 2. What's the difference between UX and UI?

> "UI is the surface a person operates — controls, layout, type, colour, states. UX is whether the whole thing works for the goal they came with, including the parts with no interface at all: the email that arrives afterwards, the support call, the wait. You can have flawless UI on a product that solves the wrong problem. You can't have good UX with UI that people can't operate, so they aren't independent — UI is a necessary component of UX, not a separate discipline sitting next to it."

**Trap:** the popular "UI is the saddle, UX is the ride" analogies are fine as a hook but don't answer the follow-up "so which one do you spend more time on and why?" Have that ready.

### 3. Walk me through the double diamond.

> "Diverge to explore the problem, converge to define one problem, diverge to explore solutions, converge to one solution. Discover, define, develop, deliver. Its real value is that it makes explicit that there are two distinct convergences and most teams skip the first one — they diverge on solutions to a problem nobody agreed. Its weakness is that it looks linear on a slide and isn't; in practice you go back through the first diamond when late evidence changes the problem, and a process model that doesn't show that misleads juniors."

### 4. What's design thinking, and what's the criticism of it?

> "Empathise, define, ideate, prototype, test — a way of applying designerly problem-solving to problems that aren't obviously design problems. The fair criticism is that as it scaled it became a workshop format rather than a practice: sticky notes and a two-day sprint, with no real users, no follow-through, and no consequences. It's useful as a shared vocabulary for non-designers and dangerous when it substitutes for actual research and craft."

### 5. Design thinking vs Lean UX vs Agile — how do they relate?

> "They answer different questions. Design thinking is about how you approach an unfamiliar problem. Lean UX is about how you reduce waste — smallest thing that produces a learning, assumptions made explicit as testable hypotheses. Agile is a delivery cadence, not a design method. The friction in most teams is that Agile's cadence is optimised for shipping increments and design needs a discovery horizon that runs ahead of it, which is why dual-track — discovery running a sprint or two ahead of delivery — is the usual reconciliation."

### 6. What is a design sprint?

> "A five-day structured format — map, sketch, decide, prototype, test — for getting from a broad question to tested evidence in a week. It's excellent for breaking a deadlock or de-risking a big bet before committing engineering. It's badly used as a substitute for continuous discovery: five people in a room for five days can produce a strong hypothesis, but you can't sprint your way to knowing your users, and running one every month usually means the team has no research practice."

### 7. When do you skip research?

> "When the cost of being wrong is lower than the cost of finding out, and you can reverse it cheaply. A copy change on a low-traffic page, an internal tool for six people I can walk over to, a decision where the design system has already answered the question. I'd never skip it on a first-in-category problem, on anything irreversible, or where I'm designing for a context I don't share — which is where my intuition is worth the least and feels the most confident."

### 8. What does a designer do that a PM doesn't?

> "A lot of the diagnosis overlaps — both of us should be asking what problem this actually is. The distinct contribution is that design makes the thing concrete enough to be argued with. A PM's spec can stay ambiguous for weeks; a flow with states in it can't. Design also owns the parts that only exist at the surface: the sequence, the language, the error path, the accessibility. In practice the healthy split is that the PM owns why and when, I own what and how, and we fight over what in a good way."

### 9. How do you handle a stakeholder who says "just make it pop"?

> "Treat it as a symptom rather than an instruction. I'd ask what they're worried about — usually it's 'people aren't noticing this' or 'this doesn't feel important enough'. Then it's a solvable problem: hierarchy, placement, contrast, or the fact that the thing genuinely isn't important enough to earn the position. Arguing about the word 'pop' goes nowhere; converting it into a goal I can test against does."

---

## UX laws

### 10. State Fitts's law and one non-obvious implication.

> "Time to acquire a target is a function of distance and target size — far and small is slow, near and big is fast. The non-obvious implication is screen edges and corners: they have effectively infinite depth because the pointer stops there, which is why the Mac menu bar at the very top is faster than a menu bar one pixel below the top. On touch, it becomes about thumb reach zones rather than pointer travel, and the practical rule is 44 by 44 points minimum with the primary action in the bottom third on a phone."

**Trap:** interviewers sometimes push "so bigger is always better?" No — a button large enough to be hit accidentally is worse, and destructive actions are a legitimate case for making a target harder to hit.

### 11. Hick's law, and where does it break?

> "Decision time grows roughly logarithmically with the number of equally-likely options. So a menu of twenty flat items is slow to choose from. It breaks in two important ways. First, it assumes the options are undifferentiated and need to be considered — a well-organised list of a hundred products that you scan visually is not twenty decisions, it's one search. Second, categorising to reduce choice count adds a navigation step, so you trade decision time for traversal time. Restructuring into three groups of seven isn't automatically better than one group of twenty-one."

### 12. Miller's law — and what's the trap?

> "Miller's 1956 finding was that short-term memory holds about seven plus or minus two *chunks* of information in a recall task. The trap is applying it to menu length or navigation items. Menus are recognition, not recall — the items are visible, so you aren't holding them in working memory at all. There is no research basis for 'seven items maximum in a navigation bar', and citing it that way is a common interview tell. Where it genuinely applies is anything the user has to carry in their head across steps: a code to retype, a value from a previous screen, a multi-step form with no summary."

### 13. Jakob's law.

> "People spend most of their time on other sites, so they expect yours to work like the ones they already know. Practically it means convention is a resource — putting the cart top-right and the logo top-left costs you nothing and saves the user learning. The cost of ignoring it is that novelty is charged to the user's attention budget, so you should only spend it where the novelty is the value. The counter-case: convention encodes what was possible when it formed, and something has to break it for anything to improve — so the question is whether you have evidence the new thing is better, not whether it's different."

### 14. What is the Doherty threshold?

> "System response under about 400 milliseconds keeps the user in a productive loop; above it, attention drifts and perceived productivity drops sharply. It comes from IBM terminal research in the early eighties. In practice it's why perceived performance work — optimistic UI, skeletons, prefetching, doing the local update before the server confirms — often buys more than actual backend optimisation. The trade-off with optimistic UI is that you have to design the rollback, and a silent failed rollback is worse than a slower honest wait."

### 15. Explain the peak-end rule and give a product use.

> "People judge an experience mostly by its most intense moment and its ending, not by the average or the duration. Product use: the end of a checkout or an onboarding disproportionately sets the memory of the whole thing, so a well-designed confirmation is worth more than shaving a step from the middle. It also means a single bad peak — a data-loss error, a humiliating validation message — outweighs a lot of smooth mediocrity, which is an argument for spending disproportionate effort on failure states."

### 16. Zeigarnik effect and progressive disclosure — how do they relate?

> "Zeigarnik: incomplete tasks stay in memory more strongly than completed ones, which is why progress indicators and partially-filled profiles create pull. Progressive disclosure is showing only what's needed now and deferring the rest. They interact: disclosure reduces load per step, but chopping one task into eight steps also creates eight incompletion states, and if the user abandons at step three you've left them with an unfinished thing rather than a shorter one. The good version shows the whole shape up front and reveals detail on demand."

### 17. Postel's law in a design context.

> "Be liberal in what you accept and conservative in what you send. In interface terms: accept the phone number with spaces, the card number with dashes, the date typed as '3 Feb' — and normalise it silently rather than rejecting it. It's the difference between an input that serves the database and one that serves the person. The cost is ambiguity: some inputs genuinely can't be disambiguated, like 03/04 as a date, and there you should be explicit rather than guess."

### 18. The aesthetic-usability effect — and its dark side.

> "People perceive attractive interfaces as more usable, and are more tolerant of minor problems in them. That's real and it means visual craft has a functional payoff. The dark side is in evaluation, not in design: attractive prototypes suppress usability feedback in testing, so participants report fewer problems than they actually hit. It's an argument for testing critical flows at lower fidelity, and for weighting observed behaviour above stated satisfaction."

---

## Heuristics and evaluation

### 19. Name Nielsen's ten heuristics.

> "Visibility of system status; match between system and real world; user control and freedom; consistency and standards; error prevention; recognition rather than recall; flexibility and efficiency of use; aesthetic and minimalist design; help users recognise, diagnose and recover from errors; help and documentation. The two most commonly violated in the products I've worked on are the first — no status during slow operations — and the ninth, where errors say what the system experienced rather than what the person should do."

### 20. What's the difference between error prevention and error recovery, and which is better?

> "Prevention stops the error occurring — disabled invalid dates, constrained inputs, confirmation on destructive actions. Recovery makes it cheap to fix — undo, preserved input, a clear route back. Prevention is better where the error is unrecoverable or costly, but over-prevention produces interfaces that block valid-but-unusual cases and treat users as suspects. The most under-used tool is undo, because it lets you skip the confirmation dialog entirely — Gmail's undo send replaced a confirmation nobody read."

### 21. How many evaluators do you need for heuristic evaluation, and why not one?

> "Three to five, working independently. One evaluator finds roughly a third of the problems; the curve climbs steeply to about five and then flattens, so the sixth is poor value. Independence is the part people skip — evaluators who discuss beforehand converge on the same findings and the extra coverage disappears."

### 22. How do you rate severity?

> "Nielsen's 0–4 scale, and severity is a function of three things: frequency, impact when it happens, and persistence — whether the user learns around it once or hits it every time. A rare unrecoverable data-loss bug outranks a constant cosmetic misalignment. I sort reports by severity rather than by screen order, because most stakeholders read one page."

### 23. Heuristic evaluation vs usability testing — when do you use each?

> "Heuristic evaluation is expert inspection, cheap and fast, good for clearing obvious violations before you spend user time on them and for baselining a competitor. Usability testing is observation of real people with real goals. They aren't substitutes: experts systematically over-report cosmetic issues and under-report the problems that only appear when someone brings their own data and their own intent. So evaluation comes before testing, not instead of it."

### 24. What is a cognitive walkthrough?

> "A structured inspection focused on learnability for first-time users. For each step you ask four questions: will they try to achieve the right effect, will they notice the action is available, will they connect that action with the effect they want, and will they see progress after doing it. Any 'no' is a finding, and the number tells you the fix type — goal, visibility, labelling, or feedback. The first three map to Norman's gulf of execution and the fourth to the gulf of evaluation."

### 25. What are affordances and signifiers?

> "An affordance is a relationship between an object's properties and what a person can do with it — a door can be pushed whether or not you know it. A signifier is the perceivable cue that communicates it — the flat plate that says push. Norman's later correction matters here: in screens we almost never create affordances, we create signifiers, and 'this button has no affordance' usually means 'this button doesn't look like a button'. The design failure in flat interfaces was removing signifiers, not affordances."

---

## Research

### 26. What's the difference between qualitative and quantitative research?

> "Qual tells you why and what to build; quant tells you how much and whether it worked. Five interviews will tell you the mechanism behind a drop-off; they will never tell you what percentage of users hit it. Analytics will tell you 62% drop at step two and never tell you why. Most bad research decisions are using one to answer the other's question — sizing a problem from six interviews, or trying to diagnose a funnel from the funnel."

### 27. Why five users?

> "Nielsen and Landauer's model: with roughly a 31% per-user problem-detection rate, five users surface about 85% of the findable usability problems in a homogeneous group, and additional users mostly re-find the same ones. The important qualifiers get dropped: it's per user *segment*, so two distinct segments means ten; it applies to usability problems, not to preference, sizing, or prevalence; and it assumes an iterative loop where you fix and retest. Five users to validate a business decision is a misuse of the number."

**Trap:** if the interviewer says "so five users is enough research?", the answer is no — five users is enough for one round of one segment on usability, and nothing else.

### 28. What's the difference between generative and evaluative research?

> "Generative research is about discovering the problem space — interviews, diary studies, contextual inquiry — and it happens before you know what you're building. Evaluative research tests something that exists — usability testing, A/B tests, surveys about a shipped feature. Teams over-invest in evaluative because it's easier to schedule and it makes existing work feel validated. The expensive failures come from skipping generative and evaluating your way to a locally-optimal version of the wrong thing."

### 29. What makes a leading question, and rewrite one.

> "A question that carries its answer. 'How easy was it to find the settings?' presumes it was easy and offers a scale of easy. Better: 'Tell me about what just happened' or 'What were you expecting when you tapped that?' Similarly, 'Would you use this?' is worthless because everyone says yes to be polite — replace with 'When was the last time you had this problem, and what did you do?' Past behaviour is evidence; predicted behaviour is conversation."

### 30. What is contextual inquiry?

> "Observing people doing the real task in the real place, with a master–apprentice framing: they work, you ask about what you see. It's the highest-yield method for finding things nobody thinks to mention — the second tool open on the other monitor, the paper note beside the keyboard, the workaround so routine it's invisible to them. The cost is that it's slow and hard to schedule, and the data is unstructured. It's the method I reach for when I suspect the stated workflow and the real workflow have diverged."

### 31. How do you recruit for a study when you have no budget and no user list?

> "In order of preference: existing customers via a support or in-product intercept; sales and support staff as proxies for what they hear, clearly labelled as second-hand; a screener posted where the segment actually is rather than a general panel; and a general panel last, because panel professionals are a distinct population. I'd also say the honest thing: if I can only get five badly-screened people, I'll report it as five badly-screened people and weight the findings accordingly rather than laundering them into confidence."

### 32. What's the difference between a moderated and an unmoderated test?

> "Moderated means you're there and can probe — best for exploratory work, complex flows, and anything where the interesting data is the reasoning. Unmoderated is cheaper, faster, and scales, but you only get what the task prompted for, so it's better for comparative or benchmark work on a well-understood flow. The failure mode of unmoderated is writing a task that accidentally tells the participant where to look."

### 33. Someone says "users don't know what they want" — respond.

> "Half right, and it's usually used to dismiss research entirely. People are unreliable at predicting their own future behaviour and at specifying solutions — that's real, and it's why I don't ask 'would you use this'. They are extremely reliable about their current problems, their workarounds, and what happened last time. So you don't ask users to design; you ask them what they did and you watch them do it. The Ford quote about faster horses is usually deployed to justify skipping the part where you find out people want to get somewhere quickly."

### 34. What is survivorship bias in product analytics?

> "Your analytics only contain the people who got far enough to be measured. If 40% of signups never complete onboarding, every behavioural insight from your active-user data is drawn from the 60% for whom the product already works. It's the main reason funnel data alone tells you where people leave and never why, and it's an argument for talking to churned and non-converting users specifically, who are also the hardest group to recruit."

### 35. How do you synthesise interview data without cherry-picking?

> "Tag at the observation level before interpreting — actual quotes and observed actions, not conclusions. Then cluster bottom-up and count how many participants support each theme, keeping participant counts rather than mention counts so one talkative person can't create a theme. Then explicitly look for disconfirming evidence for the theme I like most, because that's the one I'll be least critical of. And I write the themes that contradict my going-in hypothesis first."

---

## Accessibility

### 36. What are the four POUR principles?

> "Perceivable, Operable, Understandable, Robust. Perceivable — the content is available to at least one sense that works for the user. Operable — every function is reachable by keyboard and by assistive tech, not just by pointer. Understandable — behaviour is predictable and language is clear. Robust — it works with current and future assistive technology, which in practice means valid semantic markup and correct ARIA rather than clever DOM."

### 37. What contrast ratios do you need to remember?

> "4.5:1 for normal body text, 3:1 for large text — 18.66px bold or 24px regular — and 3:1 for meaningful non-text elements like icons, form borders, and focus indicators. That's AA. AAA is 7:1 and 4.5:1 respectively, and is a reasonable target for long-form reading but often not practical across a whole brand palette. Placeholder text and disabled states are the two things designers most consistently get wrong."

### 38. Is meeting WCAG AA the same as being accessible?

> "No, and this is the most useful thing to know about WCAG. It's an automatable floor, and roughly a third of real barriers are things it can't check — an ARIA-perfect flow that requires forty tabs to reach the primary action, a form that's technically labelled and semantically incoherent, a modal that traps focus correctly and announces nothing useful. Compliance is necessary and it is not sufficient. The only way to know is to test with assistive tech users."

### 39. What's the difference between a disability and an impairment, in design terms?

> "The useful framing is the social model: the impairment is in the person, the disability is created by the environment. A step is what disables a wheelchair user, not the wheelchair. In product terms that reframes accessibility from accommodating a minority to removing barriers we built. It also brings in situational and temporary limitations — one arm holding a baby, bright sunlight, a slow connection, a broken wrist — which is why curb-cut effects are so common."

### 40. Explain focus management and why it matters.

> "Keyboard focus is where the user's attention and input go, and for someone who can't see the screen it *is* their position in the interface. It matters most at transitions: opening a modal should move focus into it and trap it there, closing it should return focus to the trigger, a route change should move focus to the new heading, and inserting content should announce or receive focus appropriately. Getting this wrong is invisible in a screenshot and completely breaks the product for keyboard and screen reader users, which is why it survives so many design reviews."

### 41. What is a skip link and why is it still needed?

> "A link, usually the first focusable element, that jumps past repeated navigation straight to the main content. It's needed because a keyboard user otherwise tabs through the same thirty header links on every page. Landmark regions help screen reader users navigate but do nothing for a sighted keyboard user, so the skip link isn't redundant. It should become visible on focus — a permanently hidden skip link is a common failed implementation."

### 42. How do you handle colour as the only carrier of meaning?

> "Never carry meaning in colour alone. Add a second channel: an icon, a text label, a pattern, position, or weight. Roughly 8% of men and 0.5% of women have some colour vision deficiency, and beyond that colour fails in sunlight, in greyscale printing, and under a night-mode filter. Practically: a red/green status dot becomes a red cross and a green tick with a text label, and a chart gets direct labels rather than a colour legend."

### 43. Is accessible design more expensive?

> "Retrofitting it is expensive. Designing it in costs very little — semantic structure, contrast in the palette, focus states in the components, keyboard operation in the interaction spec. The cost lands in custom components: a bespoke combobox that must handle keyboard, ARIA, and screen reader announcement correctly is genuinely more expensive than a native select, which is a good argument for using native elements and for solving it once in the design system rather than per feature (Module 11)."

---

## Visual design

### 44. Does visual design matter, or is it decoration?

> "It's a functional layer, and treating it as taste is the fastest way to lose the argument for it. Hierarchy tells people what to read first; grouping tells them what belongs together; contrast tells them what's actionable; consistency lets them transfer learning between screens. And the aesthetic-usability effect means perceived quality changes tolerance for friction. Where it becomes decoration is when it's applied after the structure is fixed rather than as part of deciding the structure."

**Trap:** this question is often asked by a PM or engineer expecting a defensive answer. Answering functionally rather than defensively is the whole point.

### 45. How do you establish hierarchy?

> "Six tools, in rough order of strength: size, weight, colour and contrast, position, spacing, and enclosure. The discipline is using the fewest of them that works — if size alone establishes the order, adding colour and a box makes it noisier, not clearer. And hierarchy is relative, so a page where everything is emphasised has no hierarchy at all. The test I use is squinting: if the same three things stand out as the ones that should, it works."

### 46. What is a type scale and why use one?

> "A limited, ratio-derived set of sizes — a common one is a 1.25 or 1.333 ratio giving something like 12/14/16/20/25/31 — instead of arbitrary values. Two reasons: adjacent steps are distinguishable so hierarchy actually reads, and constraint removes a per-screen decision that produces drift across a team. The trade-off is that a strict ratio scale sometimes produces sizes you don't want, so most production scales are ratio-derived and then hand-tuned, especially at the small end."

### 47. What's a good line length and why?

> "Roughly 45–75 characters for body text, 66 as the classic target. Too long and the eye loses the line on the return sweep; too short and you break the rhythm with too many returns and increase hyphenation. On mobile you're usually forced narrower and it's fine, because the alternative is a smaller type size. The practical implication is that a full-width paragraph on a 1440px desktop layout is a readability bug, not a layout choice."

### 48. How do you use whitespace?

> "As a grouping tool first and a luxury signal second. The rule that does the most work is that the space inside a group must be smaller than the space around it — a label 4px from its input and 24px from the next field reads correctly; the same values reversed makes the label appear to belong to the field above. Most 'cluttered' interfaces don't need less content, they need the proximity relationships fixed (Module 04)."

### 49. Is a 60-30-10 colour rule real?

> "It's a workable heuristic borrowed from interior design — roughly 60% dominant neutral, 30% secondary, 10% accent — and it's useful mainly as a reminder that accent colour is scarce by definition. It isn't a law and it doesn't survive contact with a real design system, which needs semantic roles: surface, on-surface, primary, on-primary, error, warning, success, plus states for each. I'd rather talk about roles and contrast than about ratios."

### 50. What does a grid actually buy you?

> "Alignment without per-element decisions, and a shared vocabulary between design and engineering so 'span 4' means something to both. A 12-column grid is popular because 12 divides into halves, thirds, quarters, and sixths. What it doesn't buy you is hierarchy — a perfectly aligned page can still be unreadable. And rigid grid adherence can force content into columns it doesn't want; the grid is a default to depart from deliberately, not a constraint to obey."

---

## Information architecture

### 51. What is information architecture?

> "The structural design of shared information environments — how content is organised, labelled, and made findable. It's the layer that decides what's a category, what it's called, what belongs in it, and how you get from any point to any other. It's mostly invisible when it's right, which is why it's under-invested in; you notice it as 'I can't find anything' rather than as an IA problem."

### 52. Card sorting vs tree testing — what's the difference?

> "Card sorting is generative: participants group and label content, and it tells you how they think the space divides. Tree testing is evaluative: participants are given a task and navigate a text-only version of your structure, and it tells you whether your labels and hierarchy work without visual design bailing them out. The mistake is running only card sorting and treating the resulting clusters as a finished IA — a card sort output is input, not a navigation menu."

### 53. Open vs closed card sort?

> "Open: participants make and name their own groups, which surfaces their vocabulary and their mental model. Closed: you supply the categories and they file the items, which tests whether categories you've committed to are comprehensible. Open first when you're deciding structure, closed when you're validating one. Hybrid — supplied categories plus the ability to create new ones — is often the most informative in practice."

### 54. How do you handle content that belongs in two places?

> "First check whether the duplication is a symptom of the wrong top-level axis — if lots of items are ambiguous, you've probably organised by an attribute users don't think in. If it's genuinely polyhierarchical, cross-linking beats duplication: one canonical location, referenced from the other. Faceted classification is the proper answer for large content sets, where you let people filter by several dimensions rather than forcing one tree. Duplicated pages create maintenance drift and split your analytics."

### 55. Breadth vs depth in navigation?

> "Broad-and-shallow generally beats narrow-and-deep for findability — fewer decisions to reach an item, and the choices at each level are more discriminable. The classic rule of thumb is not more than three levels for most consumer sites. But breadth has a real cost in scanning time and in the header space it consumes, and mobile can't display it, so the honest answer is that the right shape depends on whether users arrive by browse or by search. If most arrival is via search or deep links, hierarchy matters less than labelling and filtering."

### 56. What makes a good label?

> "The user's word, not the organisation's. Specific enough to be distinguishable from its siblings — 'Resources' next to 'Information' is two useless labels. Front-loaded so it's scannable, since people read the first two words of a link. And tested: labelling is the single highest-return thing to tree-test, because a good structure with bad labels tests as a bad structure. 'Solutions' is the canonical failure — it's on half the B2B sites in the world and it means nothing."

---

## Design systems

### 57. What is a design system, as opposed to a component library?

> "A component library is the code and the Figma file. A design system is that plus the decisions around it: the principles, the tokens, the usage guidance, the contribution model, the versioning, and the people who maintain it. The distinction matters because most 'we have a design system' failures are libraries with no governance — components exist, nobody knows which to use, three variants of the button ship, and it drifts within two quarters."

### 58. What are design tokens?

> "Named values for design decisions — colour, spacing, radius, type — that both design and code consume from one source. The useful structure is three tiers: primitive (blue-600), semantic (color-action-primary), and component-level (button-background-primary). The value of the semantic tier is that a theme change or a brand change touches one layer rather than every component, and that a token name carries intent so you can tell whether a use is correct."

### 59. When should a pattern become a component?

> "Rule of three is the usual heuristic: when the same pattern is needed in three genuinely different contexts, it's earned. Before that you're generalising from one case and you'll build the wrong abstraction, which is more expensive than duplication. The other test is whether the variants share behaviour or only appearance — things that look alike but behave differently should stay separate, because merging them produces a component with nine boolean props that nobody can use correctly."

### 60. How do you stop a design system from being ignored?

> "Make the right thing the easy thing. That means adoption friction is a design problem: good defaults, discoverable naming, a search that works, and installation that takes minutes. Then measure adoption rather than assume it — percentage of surfaces on system components, number of detached instances, count of one-off colours in the codebase. And treat the system as a product with users: office hours, a contribution path that isn't humiliating, and a rule that if three teams have built the same escape hatch, the system is wrong rather than the teams."

### 61. What's the trade-off of a design system?

> "It buys consistency, speed on the 80% case, and accessibility solved once. It costs flexibility, a maintenance burden, and a real risk of homogenising products that should feel different. It also slows the first three projects to speed up the next thirty, which is a hard sell to whoever is running project two. The failure mode nobody plans for is a system so rigid that teams route around it, which gives you the maintenance cost and none of the consistency."

---

## Metrics and strategy

### 62. What's the difference between a leading and a lagging indicator?

> "Lagging measures the outcome you care about but reports too late to steer — revenue, quarterly retention, churn. Leading measures something earlier in the causal chain that predicts it — activation completion in week one, sessions in the first fortnight. You need both: leading for steering, lagging for truth. The failure is optimising a leading indicator that turns out not to be causally linked, which is how teams end up celebrating a number that moves while the business doesn't."

### 63. Explain HEART.

> "Google's framework: Happiness, Engagement, Adoption, Retention, Task success — chosen per project, not all five at once. For each you define goals, signals, and metrics, which is the part that does the work, because it forces you from a fuzzy goal to a specific observable. The most common misuse is treating it as a dashboard template rather than a selection exercise; a search feature might legitimately only care about task success and adoption."

### 64. What are HEART's blind spots?

> "It's user-centred by design, so it has no cost side — nothing about support load, engineering maintenance, or business viability, all of which are legitimate reasons a design succeeds or fails. It also treats engagement as good, which is only true for products where more usage means more value. For a tax-filing tool or a bank fraud flow, falling engagement is the goal, and a team that instruments HEART without thinking will optimise the wrong direction."

### 65. Is more engagement always good?

> "No, and this is a question worth being sharp on. Engagement is a proxy for value only when using the product more means getting more value. For a support centre, a settings page, or a password reset, higher engagement means something is broken upstream. And even where more is better, time-on-task can rise because people are confused. The honest metric is whether the user achieved the thing they came for, at what cost in effort — which usually needs a task-success metric alongside the engagement one."

### 66. How do you measure the impact of a design change?

> "Decide the metric and instrument it before shipping, or you'll be reconstructing a baseline afterwards from data that doesn't exist. Then pick a comparison you can defend: an A/B test if traffic supports it, a staged rollout with a holdout if not, or a before-and-after with the confounders named if neither. And define the guardrail metrics as well as the target — a change that improves conversion while raising refunds hasn't worked (Module 12)."

### 67. What's a north star metric, and what goes wrong with them?

> "A single metric that represents the core value the product delivers, used to align teams — nights booked, weekly active teams, minutes of content consumed. What goes wrong is Goodhart's law: once it's a target it stops being a good measure. Teams optimise the metric rather than the value, usually by gaming the definition. The mitigation is to pair it with counter-metrics that get worse when you cheat, and to revisit whether it still represents value at least annually."

### 68. How do you justify UX work to someone who wants to see ROI?

> "Convert design outcomes into their units. Reduced support contacts times cost per contact. Reduced time-on-task times fully-loaded hourly cost times uses per year, for internal tools. Conversion delta times traffic times average order value. Reduced rework from catching a problem in research rather than after build. I'd also be honest that some of it doesn't convert cleanly — accessibility and trust are mostly risk reduction, and the honest frame there is expected cost avoided rather than revenue gained."

### 69. What is a SUS score and what does the number mean?

> "System Usability Scale: ten standard questions, alternating positive and negative, producing a 0–100 score. It's a percentile-style benchmark, not a percentage — 68 is roughly average, above 80 is good, below 50 signals a real problem. Its value is comparability across products and over time from a small sample. Its limitation is that it's a single global attitude number, so it tells you something moved and nothing about what to fix."

### 70. What would make you reverse a design decision after launch?

> "A guardrail metric moving the wrong way, a spike in support contacts pointing at the change, or qualitative evidence that the mechanism I assumed isn't the one operating. The important part is that I decide the reversal condition before launch, not after — otherwise every ambiguous result gets rationalised into a win. I'd also say what I wouldn't reverse for: internal opinion, a loud minority in a feedback channel, or a flat metric in the first week, because most changes have a learning dip."

---

## Quick trap reference

| Question | Popular wrong answer | What to say instead |
| --- | --- | --- |
| Miller's law | "Max seven menu items" | Applies to recall, not to visible lists |
| Five users | "Five users is enough research" | Enough for one round, one segment, usability only |
| Fitts's law | "Make buttons as big as possible" | Size is one term; edges are free; destructive actions may deserve friction |
| Hick's law | "Fewer options is always better" | Adding a level trades decision time for traversal time |
| Fewer clicks | "Three-click rule" | Never had evidence; certainty per click beats click count |
| Visual design | "It's subjective" | Hierarchy, grouping, and contrast are functional |
| WCAG AA | "AA means accessible" | An automatable floor; a third of barriers aren't checkable |
| Engagement | "More engagement is good" | Only when more use means more value |
| Personas | "Every project needs personas" | Only when they change a decision someone would otherwise get wrong |
| Card sorting | "The clusters are the IA" | Card sort output is input; validate with tree testing |
| Design system | "We have a component library" | Library plus governance, or it drifts |
| A/B testing | "Just test it" | Needs traffic, a guardrail, and a pre-registered decision rule |

## Check yourself

1. Give the correct scope of Miller's law and the two places it genuinely applies.
2. Explain why "fewer options is always better" is wrong, using Hick's law properly.
3. What are the three qualifiers that get dropped from "five users"?
4. Why is WCAG AA compliance necessary but not sufficient?
5. Name a product where rising engagement is a failure signal, and say why.
6. Give the three-tier token structure and explain what the middle tier buys you.
7. What's the difference between a design system and a component library, and which failure does the distinction predict?

---

<!-- nav -->
[← Previous: Design Challenge](design-challenge.md) · [↑ Interview Prep](../README.md) · [Next: Quizzes →](../../quizzes/README.md)
