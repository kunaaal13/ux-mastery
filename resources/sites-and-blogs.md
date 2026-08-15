# Sites, Blogs, and Ongoing Sources

Books give you foundations; ongoing sources keep you current and, more importantly, keep you honest. This file lists what is worth reading regularly, what each source is genuinely good at, and what to be sceptical of in each.

Two rules before the list:

1. **Subscribe to fewer things than you want to.** A designer who reads three good sources carefully outperforms one who skims thirty.
2. **Never cite a source you have not checked.** Most design writing is opinion presented as fact. The final section of this file is a method for telling the difference, and it matters more than the list.

---

## Research and evidence-based publications

These are the sources most likely to be based on something other than the author's taste.

| Source | What it is good for | What to be sceptical of |
| --- | --- | --- |
| **Nielsen Norman Group** (nngroup.com) | The largest body of applied usability research published for practitioners: heuristics, eye-tracking studies, article and video summaries, IA and enterprise UX guidance. Strong on evaluation methodology. | Findings from small or narrow samples are often written in universal language ("users do X"). Much of the underlying data sits in paid reports you cannot audit. The house style is prescriptive; it will tell you the answer rather than the trade-off. Some guidance persists in articles long after the underlying context (device, era, population) has changed. |
| **Baymard Institute** (baymard.com) | Very large-scale, methodical e-commerce and checkout usability research, with detailed guideline libraries and benchmark databases of real sites. Unusually explicit about method and sample. | It is e-commerce, and largely Western desktop and mobile web e-commerce. "N% of sites have this issue" framing sells the paid product; a widespread issue is not automatically a costly one. Do not transplant checkout findings into enterprise or productivity software. |
| **MeasuringU** (measuringu.com) | The best free practitioner-level writing on UX statistics: sample size, confidence intervals, SUS and SEQ benchmarks, comparing designs, questionnaire validity. Jeff Sauro and colleagues show their working. | Quantitatively demanding; it will not tell you what to design. Some posts double as marketing for courses and their own instruments. |
| **ACM Digital Library / CHI proceedings** | The primary literature. When you want to know whether a claim has actually been tested, this is where the test lives. | Paywalled unless you have institutional access, though many authors post preprints. Academic findings are often lab-based, use student populations, and do not transfer cleanly to production products. Read the method section, not the abstract. |
| **dscout "People Nerds"** | Thoughtful craft writing on research practice: recruitment, facilitation, synthesis, researcher career questions. | Vendor-published, so expect the occasional nudge toward their platform's way of working. |
| **User Interviews blog and research library** | Practical method guides, templates, and salary/industry survey data for researchers. | Vendor content. Survey data comes from self-selected respondents on their list. |
| **GOV.UK Service Manual and the GDS blog** | Public documentation of how a large government designs, tests, and iterates services, including failures. Unusually evidence-led and unusually honest. | Written for public services with statutory constraints and a legal duty of accessibility. Some guidance is specific to UK government context and should not be copied verbatim. |

## General practitioner publications

| Source | What it is good for | What to be sceptical of |
| --- | --- | --- |
| **Smashing Magazine** | Long, detailed, well-edited articles spanning UX, front-end, accessibility, and design systems. Their accessibility and CSS coverage is consistently strong. | Article quality is author-dependent. Some UX pieces are opinion pieces with a "best practice" headline and no evidence. |
| **A List Apart** | Essays on web standards, content, and craft with a long editorial pedigree. Slower publishing now, but the archive is valuable. | Much of the archive is old; check dates before applying anything technical. |
| **UX Collective and similar Medium publications** | High volume, occasional gems, useful for spotting what the field is talking about this month. | The dominant format is a confident personal opinion dressed as a rule, frequently with fabricated or unsourced statistics. Treat every claim as unverified. Popularity signals engagement, not correctness. |
| **web.dev (Google)** | Authoritative on web performance, Core Web Vitals, and the measurement that underpins the Doherty-threshold arguments in Module 03. | Google-centric: metrics defined by Google, tooling by Google, and thresholds that occasionally change. Performance advice sometimes assumes a scale you do not have. |
| **MDN Web Docs** | The reference for HTML semantics, ARIA attributes, CSS behaviour, and browser support. Where you check what an element actually does. | It is a technical reference, not a design guide. Its accessibility notes are good but not a substitute for WAI documentation or testing. |
| **Laws of UX** (lawsofux.com) | A clean, well-designed summary of the named laws, useful for revision and for sending to colleagues. | Summaries are necessarily thin; the laws are stated without their limits. Module 03 in this repo deliberately adds the counter-cases that single-card summaries omit. |
| **Growth.Design case studies** | Genuinely engaging illustrated teardowns of real products, referencing psychological principles. | It is persuasion content about persuasion. Principles are asserted, not tested; the analysed company's actual results are unknown to the author. Read it for prompts, not conclusions. |
| **Pattern galleries** (Mobbin, Page Flows, and similar) | Fast reference for how established products handle a specific flow — onboarding, paywalls, empty states, deletion. Excellent for breaking a blank-page block. | A pattern being common is evidence of imitation, not of effectiveness (see Jakob's Law in Module 03, and its counter-case). Large companies ship bad flows too. Nothing in a gallery has been tested for you. |

## Platform and design-system guidelines

Treat these as *normative* for their platform — not because they are always right, but because they define the conventions your users already hold.

| Source | What it is good for | What to be sceptical of |
| --- | --- | --- |
| **Apple Human Interface Guidelines** (developer.apple.com/design) | The definitive statement of Apple platform conventions across iOS, iPadOS, macOS, watchOS, and visionOS: navigation models, controls, gestures, typography, and platform accessibility APIs. | It is a set of platform conventions, not universal usability truth, and it changes with each OS release. It describes what Apple wants, which sometimes serves Apple's business (defaults, App Store rules) rather than your users. Cross-platform products cannot follow it literally without breaking Android expectations. |
| **Material Design** (m3.material.io) | The most thoroughly documented public system: component specifications, motion, adaptive layout, dynamic colour, and a rare public treatment of accessibility inside a system. Strong reference even when you are not building Android. | It is an opinionated brand system, not a neutral baseline, and adopting it wholesale makes your product look like a Google product. Guidance has changed substantially across versions; be sure which version an article refers to. Some components are more elaborate than most products need. |
| **W3C WAI — WCAG, Understanding docs, and Techniques** (w3.org/WAI) | The normative accessibility standard plus the explanatory material. "Understanding WCAG" tells you the intent of a success criterion, and Techniques give sufficient and advisory implementation methods. | The normative text is legal-register and hard to read; the intent is in the Understanding documents, which are informative rather than normative. Conformance is a floor, not a definition of a usable experience for disabled people. |
| **W3C ARIA Authoring Practices Guide (APG)** | Reference patterns for complex widgets — combo boxes, tabs, dialogs, tree views — with expected keyboard behaviour. | The APG documents patterns; it is explicit that they are not guaranteed to be the most usable implementation in every context, and several patterns have been criticised for real-world screen reader behaviour. Test with actual assistive technology rather than assuming the pattern is safe. |
| **GOV.UK Design System** | The best public example of a system where components are justified with published research and usage data, including "when not to use this component". Form components in particular are the most tested in public. | Built for UK public services: low-frequency, high-stakes, wide population, minimal branding. Its restraint is a deliberate response to that context and will read as austere elsewhere. |
| **U.S. Web Design System (USWDS)** | Similar strengths for US federal services; strong accessibility and plain-language orientation. | Same contextual caveat as GOV.UK. |
| **Shopify Polaris, Atlassian Design System, IBM Carbon, Adobe Spectrum, Salesforce Lightning Design System, GitHub Primer** | Excellent references for how mature systems document components, tokens, content guidelines, and contribution processes. Reading three of them side by side teaches you more about documentation structure than any article will. | These are brand systems solving their own product's problems. Copying their token structure or component API without their constraints imports decisions you cannot justify. Their public docs also lag their internal reality. |
| **Microsoft Fluent** | Cross-platform system covering Windows, web, and productivity surfaces; useful for enterprise and data-dense patterns. | Multiple generations of Fluent coexist in documentation and products; check which one you are reading. |
| **EightShapes / Nathan Curtis's writing** | The most useful independent writing on design system practice: token taxonomies, component APIs, team models, and adoption measurement. | Consultancy-authored, so it favours structured, formal system practice that small teams cannot resource. |
| **Brad Frost's blog** | Systems thinking, front-end and design collaboration, and the atomic design vocabulary at source. | Opinion-led, and the atomic taxonomy is a naming convention rather than a validated model. |

## Accessibility references

| Source | What it is good for | What to be sceptical of |
| --- | --- | --- |
| **WebAIM** (webaim.org) | Plainly written explanations of WCAG requirements, the widely used contrast checker, the WAVE evaluation tool, the annual "WebAIM Million" analysis of home page accessibility, and the periodic screen reader user survey — the closest thing to public data on assistive technology usage. | The screen reader survey is self-selected and skews toward engaged, web-literate respondents; treat market-share figures as indicative, not census-grade. Automated results in the Million report only cover detectable errors. |
| **Deque and the axe ecosystem** | axe-core is the de facto open-source rules engine behind many scanners; Deque's writing on ARIA and testing is technically strong. | Commercial vendor. Automated testing detects a minority of accessibility barriers — Deque itself publishes this — so a clean axe report proves very little on its own. |
| **The A11y Project** | A community-maintained checklist and beginner-friendly resources; a good starting point and a good handout. | Community-maintained means variable depth and update cadence. It is a checklist, and checklists encourage compliance thinking. |
| **TPGi** | Detailed accessibility engineering writing, the Colour Contrast Analyser tool, and ARC Toolkit. | Vendor content with a consultancy funnel. |
| **Adrian Roselli's blog** | Rigorous, frequently contrarian testing of components — especially tables, ARIA patterns, and things that "should" work but do not in real assistive technology. Corrects a lot of received wisdom. | Deliberately blunt, and assumes technical fluency. Findings are tied to specific browser and screen reader versions; re-verify before quoting. |
| **Scott O'Hara's blog** | Careful, well-tested writing on accessible component semantics and HTML/ARIA interaction. | Technical; not design-level guidance. |
| **Sara Soueidan's blog** | In-depth articles on accessible front-end implementation, focus indicators, and inclusive component design. | Publishing is infrequent; depth over volume. |
| **Inclusive Components** (inclusive-components.design) | Heydon Pickering's component-by-component reasoning, free online. Pairs with Module 10.3. | Some articles predate current browser and AT behaviour; check the date and re-test. |
| **TetraLogical** | Practical accessibility guidance and clear explainers, often from people involved in the standards work. | Consultancy publication. |

## Newsletters

Newsletters are the lowest-effort way to stay current. Pick at most two.

| Newsletter | What it is good for | What to be sceptical of |
| --- | --- | --- |
| **UX Design Weekly** | A short curated set of links each week, weighted toward craft and case studies. Long-running and consistent. | Curation reflects one editor's taste; heavy on Medium-tier articles. |
| **Smashing Newsletter** | Well-annotated links across UX, accessibility, front-end, and tooling; the annotations often save you the click. | Long. Ties into their conference and book business. |
| **Sidebar** | Five design links a day, minimal commentary. | No filtering for evidence quality; volume adds up quickly. |
| **Dense Discovery** | Broader design, technology, and culture; good for thinking outside product UX. | Only tangentially about interface design. |
| **Nielsen Norman Group's newsletter** | Notification of new articles and videos from the largest applied research body in the field. | Same caveats as their articles; also a course-marketing channel. |

## Communities

Communities are where you get judgement, not information — the thing a search engine cannot give you.

| Community | What it is good for | What to be sceptical of |
| --- | --- | --- |
| **IxDA (Interaction Design Association)** | Local chapters, events, and a long-standing professional network. Good for meeting people who have done the job for a decade. | Activity varies hugely by city. |
| **UXPA** | Professional association with chapters, conferences, and a journal; stronger on research and human factors. | More formal and slower-moving than online communities. |
| **ADPList** | Free mentorship sessions with practitioners, including at senior levels. Genuinely useful for portfolio and interview feedback. | Mentor quality varies enormously and is unverified. Take one opinion as one opinion; get three before you rewrite your portfolio. |
| **Rosenfeld Media community and conferences** | Research, IA, and design-operations depth; the events are unusually substantive. | Paid, and North America-weighted. |
| **Designer Hangout and similar invite Slack groups** | Candid peer discussion, salary comparisons, and job leads. | Closed communities develop consensus positions quickly; groupthink is a real risk. |
| **r/UXDesign and similar forums** | A realistic picture of the job market and of what juniors are actually struggling with. Portfolio feedback is sometimes excellent. | Advice quality is uncontrolled and confidently wrong answers are common. The prevailing mood is pessimistic in ways that may not reflect your market. |

## Podcasts

Best used for judgement, history, and hearing how experienced practitioners reason — not for reference material.

| Podcast | What it is good for | What to be sceptical of |
| --- | --- | --- |
| **99% Invisible** | Design thinking applied to the built world, objects, and systems. Superb for developing an eye for invisible design decisions and for the stories you can use in interviews. | Not about interface design and rarely actionable for your Tuesday. |
| **The Informed Life** (Jorge Arango) | Interviews on information architecture, sense-making, and how people organise knowledge. | Niche and conceptual. |
| **Rosenfeld Review** | Conversations with authors and practitioners in research, IA, and design operations. | Promotes the publisher's books and conferences. |
| **Dollars to Donuts** (Steve Portigal) | Interviews with people who lead user research teams; strong on the organisational reality of research. | Narrow: research leadership specifically. |
| **Awkward Silences** (User Interviews) | Practical research method conversations. | Vendor-produced. |
| **UI Breakfast** (Jane Portman) | UI, UX, and product conversations with a small-product, practical bent. | Skews toward SaaS and founders. |
| **NN/g UX Podcast** | Short episodes on specific UX topics from their research staff. | Effectively an audio version of their articles, with the same caveats. |
| **Design Better** | Longer-form interviews with well-known designers and creative leaders. | Interview format rewards good storytellers; sponsor-influenced. |

---

## How to read design content critically

This is the most important section in the file. The field publishes an enormous amount of confident, unsourced advice, and the ability to tell strong claims from weak ones is a senior-level skill that shows up immediately in interviews and design reviews.

### Why "best practice" articles rarely cite evidence

Four structural reasons, none of them conspiratorial:

1. **Evidence is expensive and articles are free.** A properly powered study costs weeks and money. A blog post costs an afternoon. The economics guarantee that most published advice is reasoning from experience, not measurement.
2. **Publishing incentives reward confidence.** "It depends" does not get shared. Headlines are rewarded for certainty and for numbers, so hedged findings become unhedged rules on the way to the title.
3. **Most real evidence is proprietary.** The organisations running the largest experiments — the ones with the traffic to detect small effects — mostly do not publish, and when they do, they publish wins.
4. **Citation decays into folklore.** A finding gets summarised, then the summary gets cited, then the citation loses the sample size and the context. After three hops a study of 30 desktop users in 2006 has become "research shows users never scroll".

The result is a literature where the *reasoning* is often good and the *evidence* is usually absent. That does not make it worthless — mechanism-based reasoning is genuinely useful — but it does mean you should hold advice as a hypothesis about your context rather than a fact about people.

### Spotting an untested assertion

Warning signs, roughly in order of how often they appear:

| Signal | Example phrasing | What it usually means |
| --- | --- | --- |
| **Universal quantifier with no population** | "Users always…", "Nobody reads…" | Nothing was measured; this is generalised personal experience. |
| **Number with no source** | "Users decide in 50 milliseconds", "It costs 100x more to fix later" | Almost always a laundered citation. Ask which study, which population, which year. |
| **Percentage with no denominator** | "70% of users prefer…" | Preference from an unstated sample, often self-selected, often a survey rather than behaviour. |
| **Mechanism asserted as outcome** | "This reduces cognitive load, so conversion will rise" | A plausible mechanism substituting for a measured result. Load may drop and conversion may not move. |
| **Single-company anecdote as law** | "A large tech company found that a colour change earned $X million" | An unreplicated result from one context, usually stripped of the traffic scale that made it detectable. |
| **Named law applied outside its domain** | "Hick's Law means fewer menu items" | The law is being used as decoration. Check whether the original conditions apply at all (Module 03 covers each law's limits). |
| **Preference reported as performance** | "Participants said the new design was easier" | Self-report and behaviour dissociate routinely; the aesthetic-usability effect specifically suppresses reported problems. |
| **No mention of trade-off** | Advice with no cost and no context in which it fails | Real findings have boundaries. Advice without a boundary has not been tested at its edges. |
| **Undated screenshot advice** | Detailed critique of a product's flow with no date | The flow has probably changed; the critique may be years stale. |
| **Vendor conclusion matching vendor product** | "Studies show teams need a dedicated repository tool" | Not automatically wrong, but the burden of proof rises. |

### How to check a claim in five minutes

A repeatable procedure. Use it before you put a claim in a deck, a critique, or an interview answer.

1. **Find the primary source.** Follow the citation chain to the actual study, not the article that cited the article. If the chain ends at another blog post, the claim is folklore. Stop there and downgrade it to "some practitioners believe".
2. **Check the population and the sample size.** Who was tested, how many, recruited how? Five users in a lab, 300 crowdworkers, and 4 million live sessions justify wildly different sentences. Small qualitative samples can identify problems but cannot support percentages.
3. **Check the date and the platform.** Anything about mobile behaviour, scrolling, ad blindness, or performance tolerance from before roughly 2015 is describing a different device population and a different set of user habits.
4. **Check what was measured.** Was it behaviour (completion, time, errors, revenue) or self-report (preference, satisfaction, recall)? Was it a real task or a hypothetical? Was the outcome the one you care about, or a proxy?
5. **Check the effect size and the uncertainty.** "Statistically significant" without a magnitude tells you nothing about whether it matters. A 0.3% lift with a confidence interval spanning zero is not a design principle. If no interval, sample size, or duration is reported for an A/B result, assume peeking (Module 09.3).
6. **Check who benefits from the conclusion.** Vendor, consultancy, course seller, or the author's own past design decision. Interest does not disprove a claim; it raises the standard of evidence you should require.
7. **Ask whether it transfers.** The most common failure is not that the finding is false but that it was true somewhere else. E-commerce checkout findings do not govern clinical software. Consumer-app onboarding findings do not govern tools used forty hours a week by trained operators.

### Three worked examples

**"The three-click rule."** The claim that users abandon a site if a task takes more than three clicks. There is no credible study supporting it, and practitioner testing — most prominently by usability consultancies in the mid-2000s — found no reliable relationship between click count and either success or satisfaction. What actually predicts success is information scent: whether each click looks like it is heading somewhere useful (Module 08). Users will happily click seven times along a confident path and abandon after two ambiguous ones. **Verdict: discard the rule, keep the underlying concern about clarity.**

**"Five users find 85% of usability problems."** This comes from a real mathematical model by Nielsen and Landauer relating problem discovery to the number of evaluators. The model is legitimate; the slogan is not, because the result depends entirely on the assumed probability that any single user encounters a given problem. That assumption holds reasonably for a homogeneous user group performing the same simple task, and fails for products with distinct user segments, complex flows, or rare-but-severe problems. **Verdict: five users per segment is a good default for iterative formative testing; "85%" is not a number you should ever say out loud.**

**"Carousels do not work."** Here the evidence is unusually good: several organisations have published their own click-through data showing that the overwhelming majority of interactions land on the first slide, with a steep drop-off thereafter. That is a real, replicated pattern for auto-advancing homepage carousels used as navigation. It does not mean every horizontally scrolling component is bad — a manually controlled product-image gallery is a different component solving a different problem. **Verdict: strong evidence, narrow scope. Cite it accurately and say which kind of carousel you mean.**

### The habit to build

For every strong claim you plan to repeat, be able to say three things:

1. Where it came from and how big the sample was.
2. One context where it clearly applies.
3. One context where it clearly does not.

If you can only do the first, you have a citation. If you can do all three, you have judgement — and that is the distinction interviewers are listening for.

---

<!-- nav -->
[← Previous: Books](books.md) · [↑ Contents](../README.md)
