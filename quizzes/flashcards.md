# Flashcards

Compressed recall for every named law, heuristic, principle, method, metric, and criterion in this repo.

## How to use these

**Active recall, not reading.** Cover the answer column, say your answer out loud, *then* uncover and check. Reading a prompt-and-answer pair feels productive and produces almost no retention — the effortful retrieval is the thing that works. If you are not occasionally getting cards wrong, the deck is too easy and you are wasting the session.

**Spaced repetition.** Review a card at **1, 3, 7, 16, and 35 days**. A card you answer correctly moves to the next interval; **a card you fail resets to day 1**, regardless of how far along it was. Expanding intervals are what convert a card from "recognised" to "available under pressure," which is the state you need in an interview.

**The 60-second rule.** Any card you fail becomes a spoken exercise, not a re-read. Set a timer and give a 60-second out-loud answer containing three things: the **statement**, the **mechanism** (why it is true), and **one example** you can point to. Interviews test explanation, not recognition — you will never be asked to pick option (c), you will be asked "why does that happen?" A card you can recite but cannot explain is a card you have not learned.

**These answers are deliberately compressed.** One or two sentences is the memorisation unit, not the full argument. The mechanism, the boundary conditions, and the counter-cases live in the module files; the applied reasoning lives in the module quizzes and the mixed exams. Use the cards to hold the vocabulary in memory and the modules to understand it — neither substitutes for the other.

**When you have ten minutes.** Run the "Cards to master first" list at the end rather than starting at Module 01 again. Deck order is not priority order.

---

## Module 01 — Foundations

| Prompt | Answer |
| --- | --- |
| What does ISO 9241-210 say user experience includes? | A person's perceptions and responses resulting from the anticipated, actual, and remembered use of a system — before, during, and after use. |
| UX versus UI, in one sentence that does not use "look and feel" | UI is the surface handed to engineering; UX is the set of decisions about what should exist, in what order, and why. |
| The four phases of the Double Diamond | Discover, Define, Develop, Deliver — diverge, converge, diverge, converge. |
| What does each diamond of the Double Diamond cover? | The first diamond is the problem space (Discover and Define); the second is the solution space (Develop and Deliver). |
| The most common process failure | Starting at Develop because someone already decided the feature, so the problem diamond was never run. |
| The five stages of Design Thinking | Empathise, Define, Ideate, Prototype, Test — the same skeleton as the Double Diamond with different vocabulary. |
| The Lean UX hypothesis template | "We believe that [building this] for [these people] will achieve [this outcome]. We will know we are right when we see [this signal]." |
| What is dual-track agile? | A discovery track (research, framing, validation) running one to two sprints ahead of a delivery track (build, ship). |
| Persona versus job-to-be-done | A persona describes a person; a JTBD describes a situation and the progress someone wants to make in it. |
| Nielsen's five usability components | Learnability, efficiency, memorability, errors, satisfaction. |
| Which usability component do you optimise for, and how do you decide? | Learnability for occasional tasks, efficiency for daily ones — they trade off, and frequency of use decides. |
| The ISO 9241-11 usability triad | Effectiveness, efficiency, and satisfaction in a specified context of use. |
| SUS — length, range, and benchmark | 10 items scored 0-100; roughly 68 is average and 80+ is good, and it is comparable across products and over time. |
| Utility versus usability versus desirability | Utility is whether it does anything worth doing, usability is whether people can do it, desirability is whether they want it. Useful equals utility plus usability. |
| Morville's UX Honeycomb | Useful, usable, findable, credible, desirable, accessible — with valuable at the centre. |
| Five reasons a usable product still fails | No utility, not findable, not credible, not adoptable because switching cost exceeds the gain, or right solution at the wrong moment. |
| How do you choose prototype fidelity? | Match fidelity to the question — low fidelity for structure and order of steps, high fidelity only when the question is about visual or interaction detail. |
| The rule for choosing an artifact | Ask what decision is blocked right now and produce only the artifact that unblocks it; unrequested artifacts burn credibility. |
| How can you tell a journey map was actually researched? | It has dips in the emotion line. A flat emotion line means it was drawn, not researched. |
| Service blueprint versus journey map | A blueprint extends the journey downward through frontstage, backstage, and support processes, so it locates a failure at the right layer. |
| The Sean Ellis test | "How disappointed would you be if this disappeared?" — a utility and product-market-fit signal rather than a usability one. |

---

## Module 02 — Psychology & Cognition

| Prompt | Answer |
| --- | --- |
| The three models present in any product | The system model (how it actually works), the conceptual model (the story the design tells), and the user's mental model. The designer controls the conceptual model. |
| Gulf of Execution | The distance between what the user wants to do and how they must express it — "I do not know how to do this here." Bridged by discoverable, well-labelled controls. |
| Gulf of Evaluation | The distance between the system's state and the user's ability to perceive and interpret it — "Did that work?" Bridged by feedback and visible status. |
| Where do mental models come from? | Prior products above all, then the physical world, then language, then the design itself. |
| Intrinsic cognitive load | The inherent difficulty of the task itself; you can manage and sequence it but not remove it. |
| Extraneous cognitive load | Load created by how the information is presented — the designer's actual target, and the only kind you can simply delete. |
| Germane cognitive load | The effort that builds a durable mental model; protect it rather than minimising it. |
| The whole of cognitive-load theory in one line | Minimise extraneous, manage intrinsic, protect germane. |
| Realistic working-memory capacity | About four chunks of unrelated information — Miller's "seven plus or minus two" came from a 1956 paper on absolute judgement, not interface design. |
| What is chunking, and why does expertise expand capacity? | Grouping items into meaningful units; a chunk is a unit of meaning, so "BBC" is one chunk to an adult and three letters to a child. |
| Recognition over recall, and its exception | Seeing options beats producing them from memory, so show rather than ask. The exception is expert high-frequency users, for whom recall via shortcuts is faster — so offer both. |
| Name the four categories of pre-attentive attribute | Form (size, shape, orientation, enclosure), colour (hue, intensity), position, and motion. |
| Name something that is NOT a pre-attentive attribute | Semantic meaning — reading and interpreting text requires conscious processing, so no amount of wording makes something pop. |
| The pop-out effect and why four primary buttons kill it | Pop-out depends on the target differing from all distractors on one attribute; when several items share the treatment, search becomes serial and there is no primary. |
| Change blindness | People fail to notice large changes to a scene, especially across an interruption or away from the point of attention — which is why a toast far from the click goes unseen. |
| Inattentional blindness | Focused users miss the obvious; someone hunting for "Checkout" scans straight past a large promotional banner. |
| Banner blindness | Users learn to ignore regions and shapes that look like advertising, so making an important message look like an ad guarantees it is unread. |
| The three scanning patterns | F-pattern on dense unformatted text, Z-pattern or layer-cake on sparse well-headed pages, and spotted scanning when hunting a known item. |
| Satisficing | Herbert Simon's term: people take the first option that seems good enough rather than the optimal one, so the first plausible link wins. |
| Anchoring | The first number seen frames every later judgement, which is why pricing pages show the highest tier or the "was" price first. |
| Framing | The same fact stated as a gain or a loss produces different responses — frame in gains for adoption, in losses for retention. |
| Loss aversion | Losses feel roughly twice as strong as equivalent gains, which is why "you will lose your streak" outperforms "keep your streak." |
| The default effect | People keep the preselected option, making defaults the most powerful design lever available and the most ethically loaded. |
| Serial position effect | First and last items in a sequence are remembered best — it is a memory effect, not a visual-attention one. |
| Availability heuristic | Easily recalled examples feel more probable, so a recent outage dominates perceived reliability far beyond its actual frequency. |
| Decoy effect | An asymmetrically dominated third option shifts choice toward the option that dominates it — the standard mechanism in three-tier pricing. |
| The one-sentence ethical persuasion test | Does this technique help the user reach a goal they already hold, or only a goal the business holds at the user's expense? |
| The designer's own biggest bias risk | Confirmation bias — write research questions that could disprove you, and hunt deliberately for disconfirming cases. |

---

## Module 03 — UX Laws

| Prompt | Answer |
| --- | --- |
| Fitts's Law, stated | Movement time to a target depends on the distance to it and its size: `MT = a + b·log2(2D/W)`. |
| Why are screen edges and corners the fastest mouse targets? | The pointer is clamped by the screen boundary, so an edge target is effectively infinite along one axis and a corner along two — you can throw the cursor without precision. |
| Why does the corner advantage not transfer to touch? | There is no clamping: a finger can land past the physical edge, the finger occludes the target, and thumb reach dominates instead. |
| The touch equivalent of Fitts's corner insight | The thumb zone — the bottom band of the screen is cheapest to reach, the top corners the most expensive. |
| The Fitts's Law counter-case | It makes destructive actions easy to hit too, so deliberately isolate or shrink them. |
| Steering Law | Time to move through a constrained path depends on the path's length and width — it governs submenu corridors, not point targets. |
| Hick's Law, stated | Decision time grows logarithmically with the number of equally probable options: `RT = a + b·log2(n+1)`. |
| Why does Hick's Law being logarithmic matter? | Because added options have diminishing cost, so cutting the list is a weak lever — grouping, ordering, and defaults beat deletion. |
| The two assumptions Hick's Law makes that real interfaces violate | That the options are equally probable and that the problem is decision time rather than visual search. |
| Miller's Law, and its usual misuse | Working memory holds a small number of chunks (realistically about four). The misuse is "menus should have 7±2 items" — visible items are not memory. |
| Where Miller's Law genuinely applies | Wherever the interface removes information the user still needs: codes carried across steps, headers scrolled out of view, values transcribed between screens. |
| Jakob's Law | Users spend most of their time on other products, so they expect yours to work the same way. |
| The four conditions that justify breaking a convention | The new model is better on something users care about, the task is frequent enough to amortise learning, you can afford a bridge, and you can measure whether the bet worked. |
| Tesler's Law (conservation of complexity) | Complexity is conserved and can only be moved — to the user, the design, or the engineering. The question is always who absorbs it. |
| Postel's Law in interface terms | Be liberal in what you accept and conservative in what you send: accept any phone format, trim whitespace, then echo back your interpretation. |
| The limit of Postel's Law | Do not silently guess genuinely ambiguous input; normalising is fine, inventing is not. |
| The Doherty Threshold | System response under about 400 ms keeps the user in flow and measurably raises productivity (Doherty and Thadhani, IBM, 1982). |
| The three response-time bands | Under 0.1 s feels instantaneous, under 1 s keeps the flow of thought, and up to 10 s holds attention with determinate progress. Past 10 s, let users leave and notify them. |
| Three ways to improve perceived performance | Optimistic UI, skeleton screens, and prefetching during decision time — plus staged progress messaging, which makes occupied time feel shorter. |
| Where optimistic UI fails | When the operation can genuinely fail in a way that matters, because you then have to un-tell the user, which is worse than waiting. |
| Peak-End Rule | An experience is remembered by its most intense moment and its ending, not by its average or its length. |
| Duration neglect | The length of an experience is heavily discounted in memory — which is why fixing the worst moment beats shortening the whole flow. |
| Von Restorff (isolation) effect | The item that differs from its neighbours is noticed and remembered — one primary button, one "Most popular" tier. |
| The precondition Von Restorff needs | A plain background. Three badges means no isolation, so the emphasis budget is spent for zero effect. |
| Zeigarnik Effect | Unfinished tasks stay in mind, which is why progress meters and onboarding checklists pull people back. |
| Goal-Gradient Effect | Motivation increases as the goal gets closer, and endowed progress works — a card stamped twice for free outperforms one starting at zero. |
| The dark side of Goal-Gradient | It feeds sunk-cost reasoning and can trap users inside flows they should abandon. |
| Aesthetic-Usability Effect | Attractive designs are perceived as more usable and their problems are under-reported — so measure behaviour, not satisfaction, when the product is pretty. |
| Parkinson's Law in product terms | Work expands to fill the time available, so real deadlines and timeboxes help — fabricated countdowns are a dark pattern. |
| Occam's Razor as a design tie-breaker | Prefer the solution with the fewest assumptions; it is a tie-breaker between equal designs, not a licence to delete needed capability. |
| Pareto (80/20) in UX | A minority of causes drive most effects, so optimise top tasks and triage by severity times frequency — but the tail holds accessibility and enterprise needs. |
| The three-part test for a legitimate urgency mechanic | Is the constraint real, is it described accurately, and does it survive scrutiny (does the timer reset on reload, does the stock count change randomly)? |
| The five laws to know cold if you have one hour | Fitts, Hick, Jakob, Doherty, Peak-End — motor cost, decision cost, expectation, time perception, and memory. |

---

## Module 04 — Gestalt Principles

| Prompt | Answer |
| --- | --- |
| Law of Prägnanz | The eye resolves ambiguity toward the simplest, most stable interpretation available; every other Gestalt principle is a specific case of it. |
| Proximity | Elements close together are perceived as a group regardless of their similarity — spacing beats colour, borders, and labels for communicating structure. |
| Similarity | Elements sharing colour, shape, size, orientation, or texture are perceived as related; it is the mechanism underneath consistency. |
| The cardinal sin of similarity | Two things that look identical but behave differently — if behaviour differs, appearance must differ. |
| Closure | The mind completes incomplete shapes, which is why a card cut off at the viewport edge reads as "there is more this way." |
| Continuity (good continuation) | The eye follows the smoothest path, so a shared alignment edge binds a list together and a ragged edge breaks the group. |
| Common region | Elements inside a shared boundary are perceived as a group, and this overrides proximity — a card drawn around the wrong elements beats correct spacing. |
| Common fate | Elements moving in the same direction are perceived as related; items animating in together read as one set. |
| Figure and ground | The eye separates a scene into subject and background; ambiguous figure/ground (is this panel on top of or behind the content?) is a bug, not a style. |
| Symmetry and order | Symmetrical elements read as a coherent, stable whole, which is why pricing tables and side-by-side comparisons rely on it. |
| Uniform connectedness | Elements joined by a visible link — a line, a shared container edge, a connector — are the most strongly grouped of all. |
| The grouping-strength ordering, and why it matters | Uniform connectedness, then common region, then proximity, then similarity. When cues conflict in a real layout, the stronger one wins and tells you which to fix. |
| The form-label spacing rule | A label must sit closer to its own field than to any other element; equidistant labels make users associate them with the wrong input. |
| The most common spacing bug and its effect | Between-group spacing equal to or smaller than within-group spacing, which makes proximity stop encoding structure and reads as "cluttered." |
| The squint test, and four ways to run it | Deliberately degrade your view so you see only what pre-attentive perception delivers: physically squint, blur a screenshot, zoom to 25%, or convert to greyscale. |
| What the squint test is judging | Whether the intended things group, whether there is a clear first stop for the eye, whether the primary action survives, and whether figure separates from ground. |
| Why does a peeking card beat pagination dots? | Closure — the mind completes the cut-off card into a whole object that continues past the viewport, so it implies both more content and its direction, with no legend. |
| The Gestalt diagnosis of "this screen feels cluttered" | Uniform spacing (no proximity signal), ragged alignment (no continuity), and equal visual weight everywhere (no figure/ground). |

---

## Module 05 — Heuristics & Evaluation

| Prompt | Answer |
| --- | --- |
| Nielsen heuristic 1 | Visibility of system status — keep users informed about what is going on through timely, appropriate feedback. |
| Nielsen heuristic 2 | Match between system and the real world — speak the users' language and follow real-world conventions and ordering. |
| Nielsen heuristic 3 | User control and freedom — users act by mistake and need a clearly marked emergency exit. |
| Nielsen heuristic 4 | Consistency and standards — internal consistency within your product and external consistency with the platform and category. |
| Nielsen heuristic 5 | Error prevention — a careful design that prevents the problem beats even a good error message. |
| Nielsen heuristic 6 | Recognition rather than recall — make objects, actions, and options visible so nothing must be remembered. |
| Nielsen heuristic 7 | Flexibility and efficiency of use — accelerators unseen by the novice that speed up the expert. |
| Nielsen heuristic 8 | Aesthetic and minimalist design — every irrelevant unit of information competes with the relevant ones and diminishes their visibility. |
| Nielsen heuristic 9 | Help users recognise, diagnose, and recover from errors — plain language, precise problem, constructive solution. |
| Nielsen heuristic 10 | Help and documentation — ideally unnecessary, but when needed it should be task-focused, concrete, and findable at the point of doubt. |
| Which Nielsen heuristic is misunderstood, and how? | Number 8 — it is about competition for attention, not visual sparseness, so a dense professional tool can satisfy it if everything present is relevant. |
| Slip versus mistake (Norman) | A slip is the right intention executed wrongly (a mis-tap); a mistake is a wrong intention from a faulty mental model. |
| How to prevent slips versus mistakes | Slips: constraints, larger targets, forgiving input, undo. Mistakes: clearer conceptual models, better labels, and confirmations that carry real context. |
| The four parts of a good error message | What happened in the user's terms, why, how to fix it, and a way out. |
| Why is undo usually better than a confirmation dialog? | A confirmation taxes every user to protect against a rare mistake and gets clicked through reflexively; undo costs nothing on the happy path and actually works. |
| When is a confirmation justified over undo? | When the action is genuinely irreversible, has a wide blast radius, or is high cost — and then the confirmation must be informative, not "Are you sure?" |
| Shneiderman's eight golden rules — the three that add most beyond Nielsen | Seek universal usability, offer *proportional* feedback, and design dialogues to yield closure. |
| Tognazzini's distinctive principles worth naming | Anticipation, latency reduction, explorable interfaces, and protect users' work — never lose data, ever. |
| Nielsen's severity scale | 0 not a problem, 1 cosmetic, 2 minor, 3 major, 4 catastrophe — must fix before release. |
| The three factors that determine severity | Frequency, impact (how hard it is to overcome), and persistence (a one-off learnable annoyance versus a repeated obstacle). |
| How many evaluators does a heuristic evaluation need, and why not one? | Three to five working independently. One evaluator finds roughly a third of problems; the curve rises steeply to about five, then flattens. |
| The two things heuristic evaluation fundamentally cannot tell you | Whether anyone wants the thing, and how real users with real goals and real data will actually behave. |
| The four cognitive-walkthrough questions | Will the user try the right effect, notice the correct action, associate that action with the effect, and see progress after doing it? |
| How the walkthrough questions map to Norman's gulfs | Questions 1 to 3 are the Gulf of Execution; question 4 is the Gulf of Evaluation. |
| The five parts a reported finding must contain | Where, what was observed, which heuristic, the consequence, the severity, and the fix — sorted by severity, never by screen order. |
| The three-part shape of a good critique | Heuristic, observed consequence, fix — that is the difference between a trained critique and an opinion. |
| The most common evaluator mistakes | Personal preference dressed as a heuristic, redesigning instead of diagnosing, ignoring constraints, reviewing only the happy path, and omitting severity ratings. |

---

## Module 06 — Visual Design

| Prompt | Answer |
| --- | --- |
| The six tools of visual hierarchy, strongest first | Size, weight and contrast, colour, space, position, and style or treatment. |
| The most underused hierarchy tool | Space — isolation makes an element read as important even at modest size. |
| The rule of relativity in hierarchy | Emphasis is relational, never absolute: adding emphasis to more elements subtracts it from all of them. |
| The practical ceiling on hierarchy levels | Three levels is usually enough and four is the maximum; beyond that the differences stop being perceptible. |
| The emphasis budget for one view | One primary action, zero to two secondary actions, everything else at text level, and one focal content element. |
| The cheaper alternative to enlarging your primary element | Demote everything around it — lowering the noise floor beats raising the signal. |
| Body text size guidance | About 16 px on web (the browser default) and never below 14 px for sustained reading; 16-17 pt on mobile. |
| Measure (line length) target | 45 to 75 characters per line, with about 66 as the classic target — long measures cause line-tracking errors on the return sweep. |
| Line height guidance | Roughly 1.4 to 1.6 times for body text, tighter (1.1 to 1.25) for large headlines; wider measures need more leading. |
| What a modular type scale is, and why use one | Each step multiplied by a fixed ratio (often 1.2 or 1.25 from a 16 px base), so sizes are decidable rather than arbitrary. Five to seven steps is plenty. |
| When two type sizes read as a mistake | When they are within about 2 px of each other — that reads as an inconsistency rather than a hierarchy. |
| Why is all-caps poor for longer text? | It removes word-shape cues, which slows reading; it is acceptable only for short labels. |
| When do you need tabular figures? | Any time numbers sit in a column — prices, times, statistics — so digits align vertically. |
| Which part of the colour palette matters most, and why? | The neutral ramp of 8 to 12 steps, because most of the interface is neutral and it determines how everything else reads. |
| Primitive versus semantic tokens | Primitives are raw values like `blue-600`; semantic tokens are role-based like `color-text-primary`. Components should consume semantic tokens only. |
| OKLCH or LCH versus HSL | HSL is easy to reason about but perceptually uneven; OKLCH and LCH are perceptually uniform, so equal lightness values genuinely look equally light. |
| How is a contrast ratio computed? | From relative luminance, not from your perception of darkness — always measure it, never eyeball it. |
| The two contrast numbers to know | 4.5:1 for normal text and 3:1 for large text, with 3:1 also required for UI component boundaries and meaningful graphics. |
| The unbreakable colour rule | Never encode meaning with colour alone; pair it with an icon, a label, a pattern, or a position. |
| How common is colour-vision deficiency? | Around 8% of men have some form of it, which alone makes colour-only encoding unacceptable. |
| Five rules for dark mode | Avoid pure black backgrounds and pure white text, desaturate saturated hues, express elevation by lightness rather than shadow, and re-check every contrast ratio. |
| The accent trap | Using the brand colour for headers, links, icons, active states, and backgrounds at once destroys its ability to mark the primary action. |
| Grid anatomy | Columns, gutters, margins, and rows or baseline grid — plus the breakpoints at which the layout reconfigures. |
| Why 12 columns on the web? | It divides evenly by 2, 3, 4, and 6, so most layout ratios are expressible. |
| The spacing scale to use | A 4- or 8-point scale (4, 8, 12, 16, 24, 32, 48, 64); half-steps exist for optical corrections inside components, not for layout. |
| The three responsive strategies, and the risky one | Reflow, reveal/hide, and restructure. Reveal/hide is dangerous because hiding content on mobile assumes mobile users want less — hide chrome, not content. |
| Why should breakpoints be content-driven? | Set them where the layout stops working — where measure exceeds about 75 characters or a column gets too narrow — because device sizes change and content constraints do not. |
| What degrades first when you increase density? | Touch and click target size, contrast, and grouping — protect those three explicitly. |

---

## Module 07 — Interaction Design

| Prompt | Answer |
| --- | --- |
| Affordance versus signifier | An affordance is what an object can do; a signifier is the perceptible signal that tells the user it can. Interfaces fail on signifiers far more often. |
| Why is almost everything in a digital interface a signifier? | Pixels afford nothing physically — a button looks clickable only because we have learned a visual convention. |
| Natural mapping | A control layout spatially analogous to what it controls — Norman's stove with knobs arranged like the burners, or a layer panel ordered to match visual stacking. |
| Norman's four kinds of constraint | Physical, cultural, semantic, and logical. |
| The rule about gestures | A gesture may be an accelerator, never the only path to an action — gestures have no signifier and exclude keyboard and assistive-technology users. |
| Why are hover-only controls a problem, and for whom? | They are invisible on touch and unreachable by keyboard, so they exclude touch users, keyboard users, and assistive-technology users entirely. |
| The problem with a disabled button | With no explanation it is a dead end — the user cannot tell what to change. Prefer an enabled control that explains the blocker, or adjacent text stating the requirement. |
| Name the state matrix | Empty first-use, empty user-cleared, empty no-results, loading, partial/streaming, populated, overflowing, recoverable error, unrecoverable error, offline, success, and permission-denied. |
| The interactive component states | Default, hover, focus, active/pressed, selected, disabled, loading, error, read-only. |
| Which component state is skipped most, and what breaks? | Focus — skipping it makes the product keyboard-unusable and fails WCAG 2.4.7. |
| The three distinct empty states | First-use (teach and invite), user-cleared (confirm nothing is broken), and no-results (relax filters, fix spelling, offer alternatives). |
| What a good first-use empty state does | Explains the value in one line, shows what filled looks like, and offers one primary action to get out of it. |
| The acknowledgement rule | Every tap gets a visible response within 100 ms even when the result takes seconds. |
| Proportional feedback | Frequent minor actions get subtle feedback; rare major actions get substantial, unmissable confirmation. |
| Feedback and locus of attention | Put feedback near where the user is looking — a toast in the opposite corner from the click is routinely missed through change blindness. |
| Choosing the feedback carrier | Inline for validation and per-item results, toast for transient success with undo, banner for ongoing conditions, modal only when a decision blocks continuing, full page for unrecoverable errors. |
| When is a modal justified? | Only when the user must decide before continuing and the decision cannot be deferred — modals block, break keyboard and screen-reader flow, and train dismissal reflexes. |
| Optimistic versus pessimistic updates | Optimistic for high-success low-cost actions like likes and marking read; pessimistic where failure matters and reversal is confusing, such as payments and deletes. |
| The typical motion duration bands | Up to 100 ms for micro feedback, 150-250 ms for standard transitions, 250-400 ms for large sheets and page changes; beyond 400 ms is rarely justified. |
| Which easing for entering versus leaving elements? | Ease-out for entering (fast start, gentle settle) and ease-in for leaving; ease-in-out for moves between two on-screen positions. |
| The four parts of a microinteraction (Saffer) | Trigger, rules, feedback, and loops and modes — the last is skipped most and matters most over months. |
| What should the reduced-motion variant do? | Keep the information and remove the movement — a cross-fade or an instant state change, never simply no feedback. |
| Why placeholders as labels are an anti-pattern | The label disappears exactly when it is needed, it typically fails contrast, and it breaks screen-reader association and pre-submit review. |
| The five-step validation priority | Prevent, accept liberally, validate at the right moment (on blur, not per keystroke, never only on submit), explain adjacent and specific, and recover without clearing the form. |
| Toggle versus checkbox | A toggle implies the change takes effect immediately; a checkbox implies it applies when the form is submitted. |
| The biggest cheap win for mobile form completion | Autofill and autocomplete attributes plus correct keyboard types — free, and the single largest completion improvement available. |
| Form structure rules | One column, labels above fields, meaningful sections with between-group spacing clearly larger than within-group, and field length that signals expected input. |
| The trade-off of putting the easiest questions first | It exploits goal-gradient and raises completion, but front-loading trivial fields can degrade data quality and delay the questions that would disqualify a user early. |

---

## Module 08 — Information Architecture

| Prompt | Answer |
| --- | --- |
| The four components of IA (Rosenfeld and Morville) | Organisation systems, labelling systems, navigation systems, and search systems. |
| The most common kind of IA failure | A labelling failure wearing a navigation costume. |
| Exact organisation schemes | Alphabetical, chronological, and geographical — objective and unambiguous, good when the user already knows the name, date, or place. |
| Ambiguous organisation schemes | Topical, task-oriented, audience-based, and metaphor-driven — subjective, harder, and far more useful. |
| When does audience-based organisation work? | Only when users can confidently self-identify and belong to exactly one group. |
| Breadth versus depth | Broad and shallow generally beats narrow and deep, because every extra level is a decision point at which users can go wrong and recovery is expensive. |
| Information scent | Users follow whichever link smells most like what they want, judging by label, context, and surroundings — strong scent beats short paths. |
| Why is the three-click rule not useful? | Evidence does not support it; scent predicts success, and users tolerate more clicks when each one confirms they are getting warmer. |
| Pogo-sticking | Clicking into a page, bouncing back, and clicking a sibling — a direct signal of weak or misleading scent, usually a labelling or preview problem. |
| The three least informative common navigation labels | "Solutions", "Resources", and "More". |
| Labelling rules worth memorising | Use the users' words, be specific over clever, keep items at one level grammatically parallel, and front-load the meaningful word. |
| Polyhierarchy | Letting an item appear in more than one category when users' models genuinely disagree — cross-listing is cheap and matches how people look. |
| Content inventory, and why it is first | Enumerate every page with owner, traffic, last update, and purpose. It usually reveals that most content has near-zero traffic, changing the problem from organising to retiring. |
| Content model | The definition of content *types* with their attributes and relationships — what makes an IA scale, and the part engineers most need from you. |
| Open versus closed card sort | Open: participants create and name their own categories, used to design a new structure. Closed: categories are fixed, used to validate an existing one. |
| Card sort practicalities | 15 to 30 participants and 30 to 60 items; run it unmoderated for scale plus a few moderated sessions, because the reasoning is often the real finding. |
| What a card sort does NOT tell you | Whether people can find things in your structure — that is a tree test's question. |
| Tree testing | Participants do a task in a text-only hierarchy with no visual design and no search, which isolates the structure. Typically 30 to 50 participants per structure. |
| Tree test metrics beyond success rate | Directness (did they get there without backtracking), time, and first click. High success with low directness means the label is ambiguous even though the structure works. |
| Why is the first click so predictive? | Users who start down the wrong branch often never recover, so a correct first click strongly predicts eventual task success. |
| The six navigation types | Global/primary, local/secondary, contextual/inline, utility, supplemental, and wayfinding — wayfinding is the most neglected. |
| The evidence-based position on hamburger menus | Hiding navigation reduces engagement with the items inside it, so put your top three to five destinations in a visible bar and use the menu for the tail. |
| Which seeking behaviour is search bad at? | Exploratory seeking — you cannot search for a vocabulary you do not yet have, so browse must exist alongside it. |
| Two states that must be preserved on return from a detail view | Scroll position and active filters; losing them is among the most infuriating common defects in feeds and catalogues. |
| Free, continuous sources of IA evidence | Search logs (especially zero-result and high-refinement queries), support-ticket topics, and analytics on the search-versus-navigate ratio. |
| What must ship with an IA restructure? | Redirects, plus post-launch monitoring of findability, search-versus-navigate ratio, and zero-result queries. |

---

## Module 09 — Research

| Prompt | Answer |
| --- | --- |
| The three axes for classifying research methods | Qualitative versus quantitative, attitudinal versus behavioural, and generative versus evaluative. |
| The single most important fact about attitudinal data | People misreport their behaviour, cannot predict their future behaviour, and rationalise the past — weight behaviour over self-report whenever both exist. |
| What "five users find 85% of problems" does and does not claim | It applies to usability problems in one homogeneous group across iterative rounds. It does not tell you what to build, does not cover multiple segments, and licenses no claims about proportions. |
| Interview sample size | Run to saturation, when new sessions stop producing new themes — usually 5 to 12 per segment. |
| Usability test sample size | 5 to 8 participants per segment, iterating between rounds; two rounds of five beat one round of ten. |
| The core interview rule | Ask about the past, not the future: "tell me about the last time you…" beats "would you use…" |
| Why avoid hypotheticals in interviews? | "Would you pay for this?" reliably overestimates willingness; predictions of future behaviour are unreliable at any sample size. |
| The highest-value B2B interview question | "Show me how you handle that today" — workarounds like spreadsheets, sticky notes, and chat threads are where the real findings are. |
| Contextual inquiry | Interviewing in the environment while watching real work, in a master-apprentice relationship — the highest-yield generative method for professional tools. |
| Diary study | Participants log behaviour over days or weeks, capturing what people actually do over time rather than what they recall in a session. |
| Think-aloud protocol, and its caveat | Asking participants to narrate reveals expectation gaps, but it slows people down, so never use it when you are measuring time. |
| Moderating rules | Say nothing while they struggle, bounce questions back, never defend the design, and record behaviour over commentary. |
| Moderated versus unmoderated testing | Moderated gives depth and probing for complex or early designs; unmoderated gives scale and speed for validating known flows and benchmarks. |
| The rule for a good task | Give a realistic scenario with a defined end state, phrased in the user's words rather than the interface's labels. |
| How to write a screener | Screen on behaviour ("how many times did you do X last month"), never on self-described attitudes, and hide the desired answer. |
| Non-response bias | People who answer surveys differ systematically from those who do not — usually the very happy and the very angry. |
| Four survey-writing rules | One idea per question, no leading language, balanced scales with a labelled midpoint, and pilot it before fielding. |
| SUS, SEQ, CSAT, CES, NPS in one line each | SUS: 10 items, 0-100, ~68 average. SEQ: one 7-point post-task item, cheap and sensitive. CSAT: transactional satisfaction. CES: perceived effort. NPS: crude and a poor diagnostic. |
| What a retention curve tells you | A curve that flattens indicates a group that keeps returning, a product-market-fit signal; a curve declining to zero means no durable value. |
| The three inputs to an A/B test sample size | Baseline rate, minimum detectable effect, and desired power — calculate before launch and pre-commit to duration. |
| Peeking | Stopping a test when the result looks good, which massively inflates false positives. Run at least one full weekly cycle. |
| Novelty and primacy effects | A change may win temporarily because it is new, or lose temporarily because it is unfamiliar — both distort short tests. |
| Multiple comparisons | Testing twenty metrics guarantees a "significant" one by chance, so pre-declare one primary metric plus guardrails. |
| Statistical significance versus importance | With enough traffic a 0.1% lift is significant and may be worthless — state effect size and confidence interval, not just the p-value. |
| When not to A/B test | Low traffic, long-horizon effects like brand and trust, high-risk irreversible changes, and cases where the variants are different products rather than different designs. |
| Triangulation | Strong conclusions come from two or more independent method types pointing the same way — analytics for where, interviews for why. |
| What to do when qual and quant disagree | Treat the disagreement as the finding, not an error to resolve away: check the quant's validity, then use the qual for mechanism and the quant for magnitude. |
| The five levels from note to action | Observation, pattern, insight, recommendation, decision. Most reports stop at pattern; the insight is the unit of value. |
| Affinity mapping versus rainbow spreadsheet | Affinity mapping clusters observations with the team, which creates belief; a rainbow spreadsheet puts participants in columns and findings in rows, making frequency instantly visible. |
| Three guards against confirmation bias in synthesis | Write down what you expect before synthesising, have two people cluster independently, and count participants per theme rather than quoting the most vivid one. |
| Why "6 of 8" rather than "75%"? | A percentage from a sample of eight implies precision the study cannot support and invites the reader to generalise. |
| The cheapest way to make findings stick | Get stakeholders to observe the sessions — a PM who watched two users fail needs no persuading. |
| The research repository, and why | A findable store of past findings; research nobody can locate gets re-run at full cost. |

---

## Module 10 — Accessibility

| Prompt | Answer |
| --- | --- |
| The social model of disability | Disability arises from barriers in the environment, not from the person — so an inaccessible interface is a design defect, not a user limitation. |
| The interaction or mismatch model | Disability is a mismatch between a person's capabilities and the design, which is the most useful framing for designers because it makes the design the variable. |
| Permanent, temporary, situational | One arm, a broken arm, holding a baby — all three benefit from one-handed operability, which is the fastest way to widen a sceptical stakeholder's sense of the affected population. |
| POUR | Perceivable, Operable, Understandable, Robust — the four WCAG principles and the structure for any accessibility answer. |
| The structure of WCAG | 4 principles, 13 guidelines, testable success criteria, and non-normative techniques. |
| WCAG versions and what they added | 2.0 (2008), 2.1 (2018, mobile, low-vision, cognitive), 2.2 (2023, focus appearance, target size, dragging alternatives, accessible authentication, consistent help). |
| The conformance levels and the practical target | A is the minimum, AA is the practical industry and legal target, AAA is enhanced and selectively adopted. "WCAG compliant" almost always means 2.1 or 2.2 AA. |
| 1.1.1 Non-text Content (A) | Text alternatives for images; decorative images get an empty alt so screen readers skip them, informative ones describe the information rather than the picture. |
| 1.3.1 Info and Relationships (A) | Structure conveyed visually must exist in the markup — headings, lists, table headers, and label associations. |
| 1.4.1 Use of Color (A) | Colour is never the only means of conveying information. |
| 1.4.3 Contrast (Minimum) (AA) | 4.5:1 for normal text and 3:1 for large text. |
| 1.4.4 Resize Text (AA) | Content remains usable at 200% zoom with no loss of content or function. |
| 1.4.10 Reflow (AA) | No two-dimensional scrolling at a width equivalent to 320 CSS px. |
| 1.4.11 Non-text Contrast (AA) | 3:1 for UI component boundaries and meaningful graphics. |
| 2.1.1 Keyboard and 2.1.2 No Keyboard Trap (A) | All functionality must be available from a keyboard, and focus must always be able to leave a component. |
| 2.4.3 Focus Order (A) | Focus order must preserve meaning and match the visual reading order. |
| 2.4.7 Focus Visible (AA) | A visible focus indicator is required; removing outlines without a replacement is one of the most common and most damaging failures. |
| 2.4.11 Focus Not Obscured (AA, 2.2) | Sticky headers and footers must not hide the element that currently has focus. |
| 2.5.3 Label in Name (A) | The accessible name must contain the visible label text — voice-control users speak what they see. |
| 2.5.7 Dragging Movements (AA, 2.2) | Any drag action needs a single-pointer alternative, such as tap-to-select then tap-to-place. |
| 2.5.8 Target Size (Minimum) (AA, 2.2) | 24 by 24 CSS px minimum, with spacing and inline-text exceptions; 44 by 44 pt is the better practical touch target. |
| 3.3.1 and 3.3.2 (A) | Errors must be identified in text, and every input must have a visible label or instruction. |
| 3.3.7 Redundant Entry (A, 2.2) | Do not make users re-enter information they already provided in the same process. |
| 3.3.8 Accessible Authentication (AA, 2.2) | No cognitive function test without an alternative — which is why paste must work in OTP and password fields. |
| 4.1.2 Name, Role, Value (A) | Every custom control must expose what it is, what it does, and its current state. |
| 4.1.3 Status Messages (AA) | Status updates must be announced without moving focus, via live regions. |
| The first rule of ARIA | Do not use ARIA if a native HTML element will do the job — bad ARIA is worse than none. |
| EN 301 549 and VPAT | EN 301 549 is the European standard incorporating WCAG plus hardware and non-web software; a VPAT or Accessibility Conformance Report is the document enterprise procurement asks for. |
| The screen readers to know | VoiceOver (macOS and iOS), NVDA and JAWS (Windows), TalkBack (Android) — users navigate by headings, landmarks, links, and controls, not by layout. |
| Why does screen magnification make focus management critical? | Magnifier users see a small portion at high zoom, so anything far from the point of focus is effectively invisible. |
| The fastest and most revealing accessibility test | A keyboard-only pass: unplug the mouse and complete the primary flow. If you cannot finish, neither can a whole population. |
| What automated tools catch, and what they cannot judge | Roughly a third of issues at best; they can never judge whether alt text is meaningful or whether focus order makes sense. |
| Focus management for a dialog | Focus moves into the dialog on open, is trapped inside while it is open, and returns to the trigger on close. |
| The accessibility failures that block populations entirely | Keyboard traps, missing focus indicators, and custom controls with no name, role, or state. |
| Five things a designer must specify in handoff | Semantics (button versus link), accessible name, role and state, focus behaviour, and what gets announced on asynchronous change — plus alt text or an explicit decorative marking. |
| Why is leading with the legal argument weak? | It produces minimum compliance, which is the worst outcome — technically conformant and still unusable. Lead with the ethical and human case, close with legal exposure. |

---

## Module 11 — Design Systems

| Prompt | Answer |
| --- | --- |
| The five layers of a design system | Foundations and tokens, components, patterns, guidelines, and tooling and infrastructure. |
| The three tiers of tokens | Primitive (raw values), semantic (role-based), and optional component tokens. Components should consume semantic tokens, never primitives. |
| Why do semantic tokens matter? | They decouple decisions from usage, so dark mode, high-contrast mode, and white-label brands become remappings rather than rewrites — and misuse becomes visible in review. |
| The layer most systems neglect | Patterns — the compositions like forms, empty states, and error handling, which is where a system creates the most consistency. |
| Atomic Design | Atoms, molecules, organisms, templates, pages — useful as a mental model for composition, unhelpful as a literal folder structure. |
| What makes a component good | Right level of abstraction, complete states, accessible by default, composable rather than configurable, documented with "when not to use", and content guidance included. |
| Composable rather than configurable | Twenty boolean props is a smell; slots and composition scale better than flags. |
| Why is "accessible by default" the biggest multiplier? | The consumer should not need to know ARIA to use the component correctly, so one correct implementation fixes the same defect across every product surface. |
| The test for what belongs in the system | Repetition plus stability — used in three or more places with settled behaviour. Promoting something early creates churn for every consumer. |
| The four governance models | Centralised, federated, open or community, and hybrid — hybrid (core owns foundations, product teams contribute components) is the most common working answer. |
| The three things any governance model must make explicit | Who decides, how something gets in, and how a breaking change is communicated. |
| The contribution loop | Propose a use case (not a component), check for an existing solution, prototype in the product, promote once proven, and deprecate with a migration path. |
| What a contribution proposal should describe | The use case — "we need a way to show inline status on a row" — not the component, "we need a Chip." |
| The rule for breaking changes | Semantic versioning with a human changelog, lead time, a migration guide, and ideally a codemod. A breaking change without a codemod costs every consuming team and they remember. |
| Design system adoption metrics | Percentage of product surfaces on system components, detached-instance rate in design files, time-to-first-screen, count of one-off components, and support-request volume. |
| The metric that is not a success metric | Component count — activity mistaken for value. |
| Why design systems die | Built without consumers, too slow to change, no owner, rigid with no escape hatch, documentation that describes rather than guides, and measurement by component count. |
| The escape hatch | A sanctioned, documented way to build something the system does not cover and propose it back — without one, teams fork silently and drift becomes invisible. |
| The one-line answer on adoption | Systems are adopted because using them is easier than not, never because they were mandated. |

---

## Module 12 — Metrics & Strategy

| Prompt | Answer |
| --- | --- |
| The five HEART dimensions | Happiness, Engagement, Adoption, Retention, Task success — and you choose one or two, not all five. |
| The most misused HEART dimension | Engagement — for a tax-filing tool, more time in the product is a failure signal, not a success one. |
| The GSM chain | Goals to Signals to Metrics: what are we trying to achieve in user terms, what observable behaviour would show progress, and how do we count it. |
| Why does GSM matter? | Going straight to metrics produces numbers nobody can interpret; running GSM out loud is a complete senior answer to "how would you measure success?" |
| Time on task, and its caveat | Directional only — interpret it alongside success rate, because faster failure is not an improvement. |
| The three questions before adopting any metric | Would a change in it change what we do, what would make it improve for a bad reason, and who is excluded from it? |
| Who is invisible in every product metric? | People who never arrived, and anyone whose events did not fire — including users who could not sign up at all. |
| Counter-metrics, with examples | Every primary metric needs a guardrail that catches the cheap way to move it: conversion paired with refund rate, engagement with satisfaction, speed with error rate. |
| Vanity versus actionable metrics | Vanity metrics only go up and cannot inform a decision (total registered users, page views); actionable ones are rates, cohorts, per-user values, and funnel step conversion. |
| AARRR (pirate metrics) | Acquisition, Activation, Retention, Revenue, Referral. |
| Which AARRR stage is design's highest leverage? | Activation — reaching first value — and defining it precisely is often the most valuable analytical work a designer does. |
| How should activation be defined? | As the moment a user first experiences core value ("sent a first message", "completed a first transfer"), not "finished the tour." |
| N-day versus rolling versus bracket retention | Three different definitions producing very different numbers; pick one, state it, and stay consistent. |
| Resurrection | Dormant users returning — often cheaper to win back than new acquisition. |
| Voluntary versus involuntary churn | Voluntary means they chose to leave; involuntary means a payment failed. Involuntary churn is a design and operations problem with a surprisingly large payoff. |
| A north-star metric | The one number that best represents delivered user value, chosen so that moving it means the product genuinely got better rather than busier. |
| The three causes of activation drop-off | People who cannot (usability or technical failures), people who will not (value unclear or the ask is too early), and people who should not (wrong users acquired). |
| RICE | Reach times Impact times Confidence divided by Effort — the Confidence term is the honest part. |
| Kano's three categories | Basic (no satisfaction when present, severe dissatisfaction when absent), performance (scales linearly), and delight (disproportionate satisfaction, not missed if absent). |
| How do Kano attributes migrate? | Delight decays into performance and then into basic — fingerprint unlock was delight, then performance, now basic. |
| Four trade-off axes to name out loud | Speed versus flexibility, simplicity versus capability, consistency versus optimisation, and novice versus expert. |
| What every design proposal should include besides the recommendation | The cheap version that fits this sprint, so the answer can be "yes, partly" instead of "not now." |
| Design debt | Shortcuts that compound — inconsistent patterns, unaddressed findings, accessibility gaps, unsupported states. Untracked, it is invisible to planning and never funded. |
| The two things not tradeable against a deadline | Accessibility blockers and data loss. |
| How to say no professionally | Say no to a solution, never to a need: get the outcome behind the request, then make the trade-off visible and let the person with the priority mandate choose. |

---

## Module 13 — Advanced Topics

| Prompt | Answer |
| --- | --- |
| The Fogg Behaviour Model | B = MAP — behaviour occurs when Motivation, Ability, and a Prompt converge at the same moment. No prompt, no behaviour. |
| Which element of B=MAP does design move most reliably? | Ability — make the action smaller, faster, cheaper, and less scary. Then the prompt; motivation last. |
| Tiny habits | Shrink the behaviour until motivation is irrelevant — floss one tooth, write one sentence, add one item, read one card. |
| The Hook Model (Eyal) | Trigger, Action, Variable Reward, Investment — looping, with triggers moving from external to internal. |
| Why does variable reward outperform fixed reward? | Unpredictability sustains engagement far better than a predictable payoff; it is the mechanism behind feeds and pull-to-refresh, and the most abusable part of the model. |
| What does Investment do in the Hook Model? | The user puts in content, connections, or reputation, which raises the value of returning and raises switching cost. |
| The habit loop (Duhigg) | Cue, routine, reward — the same skeleton as the Hook Model in behavioural-science vocabulary. |
| Why do streaks work, and where do they go wrong? | They combine loss aversion and the goal-gradient effect, and they become anxiety machines without repair, pauses, or freezes — the goal is the habit, not the number. |
| The three-question ethical test | Whose goal does this serve, would the user be comfortable if I explained exactly how it works, and is the reverse as easy as the forward? |
| Name six dark patterns | Roach motel, hidden costs or drip pricing, confirmshaming, forced continuity, preselection, false urgency — also misdirection, trick questions, nagging, obstruction, disguised ads. |
| Roach motel | Easy to get in, hard to get out — subscribe in one click, cancel by phone. |
| Confirmshaming | A guilt-laden decline option, such as "No thanks, I hate saving money." |
| Regulation touching deceptive design | EU: GDPR consent requirements plus the Digital Services Act's explicit prohibition. US: FTC action on negative-option billing. India: the CCPA's 2023 dark-pattern guidelines. |
| The four ethical lenses beyond the three questions | The regret test, the vulnerable-user test, the scale test, and the publication test. |
| The first thing to establish when asked to build a scarcity mechanic | Whether the mechanism is factually accurate — is the stock really low? An inaccurate claim is a legal problem, and that framing ends most conversations quickly. |
| Internationalisation versus localisation versus transcreation | i18n builds the capacity to adapt (externalised strings, RTL support, flexible layout); l10n adapts to a specific locale; transcreation rewrites for cultural resonance. |
| The text expansion figure | German and Finnish run about 30% longer than English, so fixed-width buttons and containers break. |
| What mirrors in RTL languages | Layout, navigation direction, icon direction, and progress — Arabic, Hebrew, Urdu, and Persian all read right to left. |
| Why is "First name / Last name" a problematic pattern? | It fails for mononyms, patronymics, multiple surnames, and differing name orders; a single full-name field is usually correct. |
| The correct and incorrect use of Hofstede's dimensions | Correct: a prompt for questions to test locally. Incorrect: a description of the individual in front of you — national averages say nothing about a person. |
| Why design for the low end first? | A product that works on a three-year-old mid-range Android on a slow connection works everywhere; the reverse is not true. |
| The two assumptions of classical UI that generative systems break | That the system is deterministic, and that its capabilities are visible in a finite set of controls. |
| Calibrated trust | The goal is accurate trust, not maximum trust — over-trust produces unchecked errors and under-trust produces abandonment. |
| The critical axis for AI automation authority | Reversibility. Act directly where undo is trivial; suggest and confirm as the blast radius grows, and always preview before an external side effect. |
| Why is streaming output a real improvement, not a trick? | Generation is slow relative to the Doherty threshold, and streaming converts a wait into visible progress — but a stop control is mandatory. |
| The dominant AI failure mode, and its design consequence | A fluent, confident, wrong answer — so the design work moves into verification, provenance, cheap correction, and a deterministic escape hatch. |
| Four heuristics for an AI interface | Set capability expectations before first use, expose uncertainty and provenance, make correction cheaper than restarting, and preview or confirm anything irreversible. |
| The layers of a service blueprint | Physical evidence, user actions, frontstage actions, backstage actions, and support processes — separated by the lines of interaction, visibility, and internal interaction. |
| What is a service blueprint for? | Locating a failure at the right layer — a "confusing status page" is often a backstage problem where two systems cannot reconcile, and no interface work fixes that. |
| The most common channel-seam failures | Information collected in one channel is unavailable in the next, state diverges between channels, tone diverges, and the recovery channel is the worst-designed one. |
| Four second-order questions before shipping | Who else is affected, what behaviour does this incentivise, what happens at scale, and what does this make impossible later? |
| Why are internal tools high-leverage? | High frequency, high expertise, and enormous aggregate time cost — and the impact is easy to compute as time saved times loaded cost times headcount. |
| The highest leverage points in systems terms | Rules, goals, and information flows rather than surface parameters — in product terms, what gets measured and what is default beats what colour the button is. |

---

## Cards to master first

These carry the most interview weight: they are the ones that get asked directly, the ones that anchor a whole module, or the ones where a wrong answer is a visible tell.

- The four phases of the Double Diamond, and what each diamond covers
- Nielsen's five usability components, and which to optimise for
- Gulf of Execution and Gulf of Evaluation
- Realistic working-memory capacity (and why "7±2" is wrong for menus)
- Name the four categories of pre-attentive attribute
- Fitts's Law, stated
- Hick's Law, and why its logarithmic form matters
- Miller's Law, and its usual misuse
- Tesler's Law (conservation of complexity)
- The Doherty Threshold and the three response-time bands
- Peak-End Rule
- The grouping-strength ordering, and why it matters
- The form-label spacing rule
- Nielsen heuristics 1, 5, 6, and 9 by name and statement
- The three factors that determine severity
- The two contrast numbers to know
- Name the state matrix
- Open versus closed card sort, and tree testing
- What "five users find 85% of problems" does and does not claim
- POUR, and the conformance levels with the practical target
- The three questions before adopting any metric
- The five HEART dimensions and the most misused one
- The three-question ethical test
- The Fogg Behaviour Model, and which element design moves most reliably

If you can give each of these a 60-second spoken answer with a mechanism and an example, you can hold a competent conversation across every module in this repo.

---

<!-- nav -->
[← Previous: Final Exam — All 13 Modules](final-exam.md) · [↑ Quizzes](README.md) · [Next: Drills →](../exercises/drills.md)
