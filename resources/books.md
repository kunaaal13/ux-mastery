# Books

A curated reading list, grouped by what you are trying to get better at rather than by publisher or fashion. Every entry states what the book actually gives you, who it suits, and roughly what it costs you in effort.

Reading widely is not the goal. Three books read properly and applied to real work will move you further than thirty skimmed. Buy for a gap you can name.

## How to read the difficulty column

| Level | What it means |
| --- | --- |
| **Light** | An evening or two. Conversational, example-led, low prerequisite knowledge. |
| **Moderate** | A week of evenings. Assumes some vocabulary; rewards note-taking. |
| **Dense** | Textbook or reference. Read in sections against a live problem, not cover to cover. |

Marking a book **Dense** is not a criticism. Some of the most valuable books here are reference works you will open twenty times and never read straight through.

## If you only read three

| Book | Why this one |
| --- | --- |
| **The Design of Everyday Things** — Don Norman | Gives you the underlying vocabulary — affordances, signifiers, mappings, constraints, conceptual models, the gulfs of execution and evaluation. Almost everything else in the field is downstream of it. Read the revised edition. |
| **Don't Make Me Think, Revisited** — Steve Krug | The fastest route from "I have opinions about interfaces" to "I can evaluate an interface". Short, funny, and every chapter is immediately actionable. |
| **Just Enough Research** — Erika Hall | Corrects the single biggest failure mode in junior practice: designing from assumption. Teaches you what question a method can and cannot answer, and how to do useful research on no budget. |

Those three cover concepts, evaluation, and evidence — the three legs the rest of this repo stands on.

**Swap one if your situation differs:**

- **Engineer moving into design:** swap Krug for **Refactoring UI** (Wathan & Schoger). You already reason about structure; you need visual judgement.
- **Interviewing in two weeks:** swap Hall for **Articulating Design Decisions** (Greever). The bottleneck is defending your work out loud, not gathering evidence.
- **Already senior, want scope:** swap Norman for **Escaping the Build Trap** (Perri). You have the vocabulary; you need the outcome argument.

---

## Start here

Foundational, readable, and broad. If you are new, read in this order.

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **The Design of Everyday Things** (revised) | Don Norman | The core conceptual vocabulary of the field, plus a durable model of how people form expectations of objects and systems. | Everyone, at any level. | Moderate |
| **Don't Make Me Think, Revisited** | Steve Krug | Practical usability heuristics for web and app interfaces, plus the best short argument for cheap, frequent testing. | Beginners, and anyone who needs a critique checklist tomorrow. | Light |
| **100 Things Every Designer Needs to Know About People** | Susan Weinschenk | One hundred short psychology findings mapped to design implications; excellent as a browsing reference. | Beginners who want the *why* without a psychology degree. | Light |
| **Universal Principles of Design** | William Lidwell, Kritina Holden, Jill Butler | A two-page-per-concept encyclopaedia spanning design, psychology, and engineering principles. | Anyone building vocabulary breadth. | Light (as reference) |
| **Laws of UX** | Jon Yablonski | The named laws in Module 03, each with a clean explanation and examples. Overlaps heavily with this repo's Module 03. | Beginners who want the laws in one physical object. | Light |
| **Designing with the Mind in Mind** | Jeff Johnson | The perception and cognition research behind common UI guidelines, presented rigorously but accessibly. | The bridge between Weinschenk's breadth and academic depth. | Moderate |

## Psychology and behaviour

Why people do what they do. Read at least one of these properly; the field is full of confident claims about human behaviour made by people who have read none.

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Thinking, Fast and Slow** | Daniel Kahneman | System 1 / System 2, anchoring, availability, loss aversion, framing — the vocabulary of behavioural economics as it is used in product work. | Anyone doing behavioural or persuasion work. | Dense |
| **Nudge** (final edition) | Richard Thaler, Cass Sunstein | Choice architecture: defaults, framing, friction, and the argument that there is no neutral way to present a choice. | Designers of onboarding, settings, and any flow with defaults. | Moderate |
| **The Paradox of Choice** | Barry Schwartz | The case that more options can reduce satisfaction and increase regret. Useful counterweight to feature maximalism. | Anyone arguing against option bloat. | Light |
| **Influence: The Psychology of Persuasion** | Robert Cialdini | Reciprocity, commitment, social proof, authority, liking, scarcity. Also, unavoidably, the source manual for most dark patterns. | Read alongside Module 13.2 on ethics, not instead of it. | Moderate |
| **Designing for Behavior Change** | Stephen Wendel | The most methodical treatment of turning behavioural science into a designed intervention, including measurement. | Practitioners actually building habit or change products. | Moderate |
| **Hooked** | Nir Eyal | The trigger → action → variable reward → investment model, explicitly as a product-building playbook. | Read critically; see the skippable section below. | Light |
| **Seductive Interaction Design** | Stephen Anderson | Playfulness, motivation, and emotional engagement in interfaces, with a strong visual treatment. | Designers whose work is technically correct and emotionally flat. | Light |
| **Predictably Irrational** | Dan Ariely | Popular accounts of decoy effects, relativity, and the cost of free. Entertaining and widely cited. | Read for intuitions, not as evidence; see caveats below. | Light |

**A necessary caution on this section.** Parts of the popular behavioural-science literature have not held up. Several social-priming results discussed in *Thinking, Fast and Slow* have failed to replicate, and Kahneman himself publicly acknowledged that the priming chapter placed too much confidence in that literature. Separately, a widely cited 2012 paper on honesty pledges co-authored by Ariely was retracted after data-integrity problems were found. None of this makes the books worthless — the frameworks are still useful for generating hypotheses — but it does mean you should treat any single study cited in a popular book as a hypothesis to test in your own context, never as a settled fact to cite in a design review.

## Interaction and craft

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **About Face: The Essentials of Interaction Design** | Alan Cooper, Robert Reimann, David Cronin, Christopher Noessel | The most complete single reference on interaction design: goal-directed design, personas, posture, patterns, and detailed control-level guidance. | Intermediate practitioners; use as a reference, not a read-through. | Dense |
| **Designing Interfaces** | Jenifer Tidwell (with co-authors in later editions) | A pattern library in book form: named patterns with context, trade-offs, and examples. | Anyone who wants a vocabulary for "the thing where…". | Moderate (as reference) |
| **Refactoring UI** | Adam Wathan, Steve Schoger | Concrete, non-theoretical rules for making an interface look designed: hierarchy, spacing, colour, depth, empty states. | Engineers and anyone with weak visual craft. Fastest visual improvement per page read. | Light |
| **Form Design Patterns** | Adam Silver | Accessible, robust form patterns built from HTML first. Genuinely opinionated and genuinely correct about most things. | Anyone designing or building forms — which is most people. | Moderate |
| **Web Form Design: Filling in the Blanks** | Luke Wroblewski | Older but still the definitive treatment of form layout, labels, validation timing, and error recovery. | Complements Silver: Wroblewski for layout research, Silver for implementation. | Moderate |
| **Designing Interactions** | Bill Moggridge | Interviews with the people who created the mouse, the Palm Pilot, early web interfaces. History and judgement rather than technique. | Mid-level designers who want perspective on why things are as they are. | Moderate |
| **Emotional Design** | Don Norman | The visceral / behavioural / reflective model, and the argument that attractiveness affects perceived usability. | Read after *The Design of Everyday Things*, not before. | Moderate |
| **Sketching User Experiences** | Bill Buxton | The case for generating many rough alternatives before refining one, and the distinction between sketches and prototypes. | Designers who jump straight to high fidelity. | Moderate |
| **The Humane Interface** | Jef Raskin | A radical, first-principles critique of modal interfaces and application-centric computing. Not all of it is practical; all of it is thought-provoking. | Experienced designers who want their assumptions attacked. | Dense |
| **Designing Voice User Interfaces** | Cathy Pearl | Conversation design fundamentals: turn-taking, error recovery without a screen, confirmation strategies. | Anyone touching voice or conversational surfaces. | Moderate |
| **Conversational Design** | Erika Hall | The argument that interfaces are conversations, and what human conversational norms imply for interface language. | Complements Pearl; more philosophical, shorter. | Light |

## Research methods

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Just Enough Research** | Erika Hall | Method selection, bias avoidance, and how to do credible research with no budget and no permission. Short and sharp. | Everyone. The best first research book. | Light |
| **Interviewing Users** | Steve Portigal | How to actually run an interview: rapport, silence, follow-up, and avoiding the questions that produce useless answers. | Anyone who talks to users, which should be everyone. | Light |
| **The Mom Test** | Rob Fitzpatrick | How to ask questions that survive people's desire to be nice to you. Written for founders; applies directly to discovery. | Anyone doing early problem-space conversations. | Light |
| **Rocket Surgery Made Easy** | Steve Krug | A step-by-step manual for running cheap monthly usability tests yourself. The practical sequel to *Don't Make Me Think*. | Teams with no researcher and no budget. | Light |
| **Handbook of Usability Testing** | Jeffrey Rubin, Dana Chisnell | The thorough version of the same job: planning, protocols, facilitation, analysis, reporting. | Anyone running formal evaluative studies. | Dense |
| **Observing the User Experience** | Mike Kuniavsky, Elizabeth Goodman, Andrea Moed | A broad survey of methods with practical guidance on when each applies. | A good second research book after Hall. | Moderate |
| **Universal Methods of Design** | Bella Martin, Bruce Hanington | One hundred methods, two pages each, with when-to-use guidance. A menu, not a manual. | Choosing a method when you know the question but not the tool. | Light (as reference) |
| **Think Like a UX Researcher** | David Travis, Philip Hodgson | Short provocations on research practice, each ending in a discussion exercise. Strong on critical thinking about evidence. | Mid-level practitioners defending research quality. | Moderate |
| **Quantifying the User Experience** | Jeff Sauro, James R. Lewis | The statistics of UX: confidence intervals, sample sizes, SUS norms, comparing designs properly. | Anyone reporting numbers. The book that stops you saying "80% of users" from a sample of five. | Dense |
| **Measuring the User Experience** | Tom Tullis, Bill Albert | A broader survey of UX metrics and how to collect, combine, and present them. | Complements Sauro & Lewis; lighter on inference, wider on metric choice. | Moderate |
| **Surveys That Work** | Caroline Jarrett | How to write survey questions that produce answers meaning what you think they mean. Survey design is much harder than it looks and this is the book about it. | Anyone about to send a survey. | Moderate |
| **Continuous Discovery Habits** | Teresa Torres | Weekly customer contact, opportunity solution trees, and assumption testing as an ongoing team habit rather than a project phase. | Designers working closely with product. Directly relevant to Module 12.3. | Moderate |
| **Practical Empathy** | Indi Young | Listening sessions and thinking-style research: understanding reasoning and reactions rather than tasks. | Researchers who want depth beyond task-based work. | Moderate |
| **Mapping Experiences** | Jim Kalbach | The definitive treatment of journey maps, service blueprints, experience maps, and mental model diagrams — including when each is the wrong choice. | Anyone about to make a journey map. | Moderate |
| **Remote Research** | Nate Bolt, Tony Tulathimutte | Running studies with distributed participants. Predates the current tooling but the methodology holds. | Distributed teams. | Moderate |

## Information architecture

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Information Architecture: For the Web and Beyond** | Louis Rosenfeld, Peter Morville, Jorge Arango | The field's reference text: organisation, labelling, navigation, and search systems, plus IA research methods. | The definitive IA book. Read the chapters you need. | Dense |
| **How to Make Sense of Any Mess** | Abby Covert | IA as a general sense-making practice, in plain language and under 200 pages. Excellent first exposure. | Beginners, and non-designers you need to teach. | Light |
| **Everyday Information Architecture** | Lisa Maria Marquis | Practical, modern, content-first IA for real websites: audits, taxonomies, navigation. Short. | Practitioners who want the applied version of Rosenfeld. | Light |
| **A Practical Guide to Information Architecture** | Donna Spencer | Hands-on process guidance with worked examples and templates. | Designers doing an IA project this quarter. | Moderate |
| **Card Sorting: Designing Usable Categories** | Donna Spencer | The one book on card sorting: running it, analysing it, and what its results actually justify. | Anyone running a card sort. | Light |
| **Search Patterns** | Peter Morville, Jeffery Callender | Search as a designed experience — query formulation, faceted results, refinement, zero results. | Anyone whose product has a search box that matters. | Moderate |
| **Living in Information** | Jorge Arango | Places made of information: architecture as a metaphor for digital environments, plus a serious ethical thread. | Mid-level and up; more conceptual than procedural. | Moderate |

## Accessibility

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Inclusive Components** | Heydon Pickering | Component-by-component accessible implementations with the reasoning made explicit. Also available as a website. | Designers and engineers building component libraries. | Moderate |
| **Inclusive Design Patterns** | Heydon Pickering | Page and layout-level inclusive patterns, robust to varied input and output. | Front-end oriented practitioners. | Moderate |
| **Accessibility for Everyone** | Laura Kalbag | A short, well-structured orientation to accessibility: standards, disability types, process, and where to start. | The best first accessibility book. | Light |
| **A Web for Everyone** | Sarah Horton, Whitney Quesenbery | Accessible UX with personas of disabled users and design-level (not just code-level) guidance. | Designers who keep being told accessibility is an engineering task. | Moderate |
| **Mismatch: How Inclusion Shapes Design** | Kat Holmes | The framing of disability as a mismatch between person and environment, and inclusive design as a method rather than a checklist. | Everyone. Changes how you think, not what you check. | Light |
| **Design for Real Life** | Eric Meyer, Sara Wachter-Boettcher | Designing for stress cases and crisis moments rather than idealised happy users. Short and genuinely affecting. | Anyone designing forms, notifications, or "celebration" moments. | Light |
| **Design Justice** | Sasha Costanza-Chock | An academic and activist critique of who design serves and who decides. Uncomfortable and worth it. | Senior practitioners thinking about power in design. | Dense |

## Design systems

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Design Systems** | Alla Kholmatova | The strongest treatment of system *principles*, shared language, and how systems actually get adopted by people. | Anyone building or maintaining a system. The most useful single book here. | Moderate |
| **Atomic Design** | Brad Frost | The atoms → molecules → organisms → templates → pages hierarchy, plus workshop and process guidance. | Read for the vocabulary; the core idea is one chapter long. | Light |
| **Expressive Design Systems** | Yesenia Perez-Cruz | How to keep a system flexible enough for brand and editorial expression instead of flattening everything. | Teams whose system is being blamed for boring work. | Light |
| **Laying the Foundations** | Andrew Couldwell | The pragmatic build guide: audits, naming, documentation, and getting a system shipped. | Someone actually starting a system next month. | Moderate |
| **Form Design Patterns** | Adam Silver | Listed again deliberately — forms are where most design systems break. | Systems teams. | Moderate |

## Strategy, metrics, and influence

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Articulating Design Decisions** | Tom Greever | How to explain, defend, and adjust design work in front of stakeholders. Directly raises interview and review performance. | Every designer, especially before interviews. | Light |
| **Discussing Design** | Adam Connor, Aaron Irizarry | How to run and receive critique so it produces better work instead of hurt feelings. | Anyone in a team that "does design reviews" badly. | Light |
| **Escaping the Build Trap** | Melissa Perri | The argument for outcomes over output, and how product organisations drift into feature factories. | Designers who want to argue about what gets built, not just how. | Moderate |
| **Outcomes Over Output** | Josh Seiden | A very short, very direct treatment of defining behavioural outcomes instead of deliverables. | Read in two hours before a roadmap meeting. | Light |
| **Inspired** | Marty Cagan | How strong product teams operate, and the designer's place in them. Prescriptive and occasionally dogmatic. | Understanding your PM's worldview. | Moderate |
| **Lean UX** | Jeff Gothelf, Josh Seiden | Assumption mapping, hypothesis statements, and collaborative design in short cycles. | Teams introducing a design practice into agile delivery. | Light |
| **Lean Analytics** | Alistair Croll, Benjamin Yoskovitz | The "one metric that matters", business-model-specific metrics, and the case against vanity metrics. | Designers who want to speak the business's language. | Moderate |
| **Trustworthy Online Controlled Experiments** | Ron Kohavi, Diane Tang, Ya Xu | The serious book on A/B testing: power, peeking, novelty effects, guardrail metrics, and the many ways experiments mislead. | Anyone whose organisation ships based on tests. Directly supports Module 09.3 and 12.2. | Dense |
| **Org Design for Design Orgs** | Peter Merholz, Kristin Skinner | Structuring, hiring, and levelling a design team. | Leads, managers, and senior candidates asked about team structure. | Moderate |
| **Sprint** | Jake Knapp, John Zeratsky, Braden Kowitz | A prescriptive five-day process for going from problem to tested prototype. | Facilitators. See caveats below. | Light |

## Writing and content design

Interface writing is the highest-leverage, lowest-status skill in UX. Changing words is nearly free and frequently outperforms changing layout.

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Writing Is Designing** | Michael J. Metts, Andy Welfle | The case for words as a design material, with process guidance for collaborating on interface copy. | Designers who write UI copy without calling it that. | Light |
| **Strategic Writing for UX** | Torrey Podmajersky | A practical system for voice, conversation patterns, and measuring copy changes. | Practitioners producing copy at volume. | Moderate |
| **Content Design** | Sarah Winters | The discipline of content design: starting from user needs and evidence rather than what the organisation wants to say. Rooted in UK government practice. | Anyone working on content-heavy services. | Light |
| **Letting Go of the Words** | Janice (Ginny) Redish | Writing for scanning, not reading: structure, headings, chunking, and cutting. Evidence-led and thorough. | Anyone writing long-form product or support content. | Moderate |
| **Nicely Said** | Nicole Fenton, Kate Kiefer Lee | Voice, tone, and clear web writing for non-writers. Friendly and practical. | Designers who freeze at a blank error message. | Light |
| **Microcopy: The Complete Guide** | Kinneret Yifrah | Exhaustive, example-heavy treatment of small interface text: buttons, errors, empty states, confirmations. | Reference for the moments Module 07 covers. | Light |

## Ethics

| Book | Author | What it gives you | Who it is for | Difficulty |
| --- | --- | --- | --- | --- |
| **Ruined by Design** | Mike Monteiro | An angry, direct argument that designers are responsible for what they build. Light on nuance, heavy on conviction. | A useful jolt; not a framework. | Light |
| **Tragic Design** | Jonathan Shariat, Cynthia Savard Saucier | Case studies where design decisions caused real harm, including deaths, plus a framework for anticipating harm. | Making the stakes concrete. | Light |
| **Evil by Design** | Chris Nodder | A catalogue of manipulative patterns organised by the deadly sins, described from the perpetrator's side. | Read as a field guide to what to recognise and refuse. | Moderate |
| **Future Ethics** | Cennydd Bowles | The most rigorous practitioner-level treatment: consequentialism versus deontology versus virtue ethics applied to technology, plus practical methods. | The book to read if you want to reason about ethics rather than emote about it. | Moderate |
| **Technically Wrong** | Sara Wachter-Boettcher | How defaults, forms, and algorithms encode the assumptions of the people who built them. | Concrete, product-level examples of exclusion. | Light |
| **Weapons of Math Destruction** | Cathy O'Neil | How opaque scoring systems scale and entrench harm. Not a design book; essential context for anyone designing around models. | Anyone touching algorithmic products. | Moderate |
| **Race After Technology** | Ruha Benjamin | Discriminatory design and the "New Jim Code": how technical systems reproduce inequality while appearing neutral. | Serious reading on bias in systems. | Dense |
| **Algorithms of Oppression** | Safiya Umoja Noble | How search ranking encodes and amplifies bias, with detailed documentation. | Anyone designing search, ranking, or recommendation. | Dense |
| **Design for Cognitive Bias** | David Dylan Thomas | Short treatment of how your own biases shape what you build, and practical debiasing tactics. | A quick, self-directed complement to the above. | Light |

## Classics worth the time

Older books that still repay reading, with an honest note on what has dated.

| Book | Author | Still worth it because | What has dated |
| --- | --- | --- | --- |
| **The Design of Everyday Things** | Don Norman | The conceptual core is permanent. | Nothing significant in the revised edition. |
| **The Visual Display of Quantitative Information** | Edward Tufte | Data-ink, chartjunk, and small multiples remain the standard vocabulary for data presentation. | Print-centric; some prescriptions are stricter than evidence supports. |
| **Grid Systems in Graphic Design** | Josef Müller-Brockmann | Grids, modular thinking, and typographic rigour transfer directly to screen layout. | Entirely print, bilingual German/English, and unapologetically dogmatic. |
| **Thinking with Type** | Ellen Lupton | The clearest introduction to typographic anatomy, hierarchy, and grids for screens. | Minor; later editions cover web type adequately. |
| **The Elements of Typographic Style** | Robert Bringhurst | The reference on typographic craft and its reasoning. | Print-first; you must translate to fluid, responsive contexts yourself. |
| **Interaction of Color** | Josef Albers | Trains your eye to see colour as relational rather than absolute — the single most useful colour insight. | Exercise-based and slow; not a palette manual. |
| **Usability Engineering** | Jakob Nielsen | The origin of much modern evaluation practice, including the heuristics and discount usability arguments. | 1993 examples and technology; the economic arguments are of their time. |
| **Designing the User Interface** | Ben Shneiderman and co-authors | Source of the eight golden rules; a genuine textbook of HCI with academic grounding. | Long, expensive, and textbook-paced. Read chapters. |
| **The Elements of User Experience** | Jesse James Garrett | The five planes model — strategy, scope, structure, skeleton, surface — is still a clean way to explain UX to non-designers. | Web-of-2002 assumptions throughout. |
| **The Inmates Are Running the Asylum** | Alan Cooper | Introduced personas and goal-directed design to a wide audience; a bracing critique of engineering-led design. | Examples are ancient and the tone is combative; the persona practice has moved on. |

## Commonly recommended but skippable unless X

Honest notes on books you will see on every list. None of these are bad; all of them are over-recommended relative to what they give a working practitioner.

| Book | Skip unless | Honest reasoning |
| --- | --- | --- |
| **Hooked** (Eyal) | You are working on retention or habit products, or you need to recognise the pattern to argue against it. | It is a clear, short model, but it is written as a manipulation playbook with ethics relegated to a short chapter. Reading it uncritically produces designers who optimise for compulsion and call it engagement. Pair it with Module 13.2 and with *Future Ethics*. Eyal's later *Indistractable* is partly a response to the criticism. |
| **Sprint** (Knapp et al.) | You will actually facilitate a design sprint. | The five-day structure is rigid and expensive in senior-person time. Teams frequently run one, feel productive, and change nothing. The individually useful parts — "how might we" notes, expert interviews, solution sketching, deciding before prototyping — can be extracted and used without the ceremony. |
| **Atomic Design** (Frost) | You need the shared vocabulary for a systems conversation. | The taxonomy is genuinely useful and takes ten minutes to learn; the book is much longer than the idea. Most teams argue about whether something is a molecule or an organism and get no value from the answer. Kholmatova's *Design Systems* is the better use of the same reading time. |
| **The Elements of User Experience** (Garrett) | You need a diagram to explain UX to executives. | Historically important and still a decent explanatory model, but it describes a web-page-centric world and will not tell you how to do anything. |
| **The Inmates Are Running the Asylum** (Cooper) | You are interested in the intellectual history of personas. | The core argument won, so the polemic now feels like shouting at a door someone already opened. *About Face* is the same authors' useful book. |
| **Designing Web Usability** (Nielsen, 1999) | You are studying the history of the field. | Genuinely foundational and genuinely obsolete; its specific guidance is about 1990s web constraints. The heuristics survive; the book does not need to be read. |
| **Any "UI design rules" listicle book** | It is bundled free. | Books that are a hundred rules with no reasoning teach you to obey rather than to judge. The rules are only useful attached to a mechanism and a counter-case — which is the format this repo uses deliberately. |
| **Thinking, Fast and Slow** (Kahneman) | You want depth on judgement and decision-making and will read all 500 pages. | Excellent, but long, and parts of the underlying literature have not replicated. If you want the applied version in a tenth of the time, read *Nudge* or Wendel. |
| **Most "portfolio and career" books** | You have no portfolio at all. | Career advice ages fast, is highly market-dependent, and is better sourced from current hiring managers and communities than from a book printed three years ago. |

## Building a reading plan

| If your gap is… | Read, in this order |
| --- | --- |
| "I do not have the vocabulary" | Norman → Weinschenk (browse) → Yablonski or Module 03 |
| "I cannot tell if a design is good" | Krug → Johnson → *About Face* (chapters) |
| "My work looks amateur" | Wathan & Schoger → Lupton → Müller-Brockmann |
| "I design from assumption" | Hall → Portigal → Torres |
| "My numbers get challenged" | Sauro & Lewis → Kohavi et al. → Croll & Yoskovitz |
| "Nobody accepts my recommendations" | Greever → Connor & Irizarry → Perri |
| "I do not know if what I build is right" | Bowles → Wachter-Boettcher → Shariat & Savard Saucier |
| "Our components keep drifting" | Kholmatova → Silver → Couldwell |
| "I cannot find anything in our product" | Covert → Marquis → Rosenfeld et al. (chapters) |

Read one book per gap, apply it to a real piece of work within two weeks, then pick the next gap. A book you did not act on did not count.

---

<!-- nav -->
[← Previous: Drills](../exercises/drills.md) · [↑ Contents](../README.md) · [Next: Sites, Blogs, and Ongoing Sources →](sites-and-blogs.md)
