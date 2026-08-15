# Quiz — Module 08: Information Architecture

12 questions. Target: 9/12.

---

### Part A — Recall

**1.** The four components of IA are organisation, labelling, navigation, and:
- a) taxonomy
- b) search
- c) content strategy
- d) metadata

**2.** A card sort primarily tells you:
- a) whether users can find things in your structure
- b) how users group and name things
- c) which labels have the best contrast
- d) the optimal number of nav items

**3.** Low directness with high success in a tree test indicates:
- a) the structure is broken
- b) labels are ambiguous but the structure is workable
- c) the tasks were too easy
- d) users used search

**4.** Pogo-sticking is a signal of:
- a) slow load times
- b) weak information scent
- c) too few nav items
- d) poor colour contrast

**5.** The "three-click rule" is:
- a) a validated usability standard
- b) not supported by evidence; scent predicts success better
- c) applicable only to mobile
- d) a WCAG requirement

---

### Part B — Short answer

**6.** Give three ambiguous organisation schemes and a condition under which each fails.

**7.** Explain information scent and the design moves that strengthen it.

**8.** State the difference between card sorting and tree testing in one sentence each.

**9.** Give the evidence-based position on hamburger menus, and where they are acceptable.

---

### Part C — Applied

**10.** A bank's app navigation is "Accounts / Cards / Loans / Insurance." Support contacts are dominated by "how do I change my address" and "how do I dispute a charge." Diagnose and propose a structure, then say how you would validate it.

**11.** You inherit a product with 40 features and a 14-item primary nav that grows every quarter. Give a plan, including what you would measure before and after.

**12.** You have no research budget and two weeks to validate a navigation redesign. Describe exactly what you would run and what you would knowingly not learn.

---
---

## Solutions

**1. b)** Search systems.

**2. b)** How users group and name things — it is generative. Findability in a proposed structure is what tree testing measures.

**3. b)** Users eventually reach the right node but wander to get there, which points at ambiguous or overlapping labels rather than a wrong hierarchy. Fix the labels, then re-test the specific failing tasks.

**4. b)** Weak scent — the link did not accurately predict what was behind it, so users bounce back and try a sibling.

**5. b)** Not evidence-based. Users tolerate more clicks when each one confirms they are getting closer; success tracks scent, not click count.

---

**6.** Any three, with failure conditions:
- **Topical** — fails when items plausibly belong to two subjects, or when users do not share the domain vocabulary that makes the topics meaningful.
- **Task-oriented** — fails when users do not know what the task is called, or when a single task spans many products and the labels get abstract.
- **Audience-based** — fails when users cannot confidently self-identify, or belong to more than one audience (a student who is also an alumnus), so they must guess which section holds their content.
- **Metaphor-driven** — fails when the product outgrows the metaphor and behaviour must diverge from it, which then breaks the mental model it created.

**7.** Information scent is the user's judgement, from a link's label, context, and surroundings, of how likely it is to lead to what they want — from information-foraging theory. Users follow the strongest scent rather than the shortest path. Strengthen it by: using the users' own words; front-loading the meaningful word in the label; adding previews (counts, thumbnails, one-line descriptions); keeping labels consistent across nav, page title, search results, and emails so arrival is confirmable; and making category contents predictable rather than clever. Weak scent shows up as pogo-sticking and high back-button use.

**8.** **Card sorting:** users group and name content items, telling you their mental model and vocabulary — generative, done before you design the structure. **Tree testing:** users perform find-it tasks against a text-only version of your proposed hierarchy, telling you whether your structure and labels actually work — evaluative, done before you design screens.

**9.** Hiding navigation behind a hamburger measurably reduces engagement with the items inside compared with visible tabs, because it removes the signifier and adds a step. Acceptable for **secondary and utility items**, and on small screens for the tail of a navigation whose top 3–5 destinations are already visible in a bar. On desktop, where space exists, hiding primary navigation is rarely justifiable.

**10.** Diagnosis: the navigation is a **product-line taxonomy** (an org-chart IA), while users arrive with **tasks**. Changing an address and disputing a charge cut across every product, so they have no home in the current structure and users default to calling support. High support volume on cross-cutting tasks is the diagnostic signature.
Proposal: keep the product taxonomy for browsing balances and details, and add a **task layer** that is primary for transactional intents — a prominent "Payments and transfers", "Help with a transaction" (dispute, report fraud, query), and "Your details" (address, contact, preferences) — plus contextual entry points, so a dispute can be started directly from the transaction row where the user is already looking, which usually outperforms any menu placement.
Validation: derive the task list from support-ticket topics and search logs; run an open card sort (15–30 customers) to get their words for these tasks; draft two structures; tree test both (30–50 per structure) on tasks like "dispute a charge" and "change your address"; first-click test the designed home screen; after launch, measure support-contact volume for those topics, findability rate, and zero-result search queries. Success metric should be the support-contact reduction, not a satisfaction score.

**11.** Plan:
1. **Content and feature inventory** with usage data per item — traffic, unique users, frequency, and which items support revenue or retention. Expect a long tail with near-zero use.
2. **Baseline measurement before changing anything:** nav item click distribution, task success on 5 top tasks (tree test), search-vs-navigate ratio, zero-result queries, and support-ticket topics.
3. **Choose the primary set from data** — the destinations covering the large majority of sessions, typically 5 or fewer for mobile, plus a small utility group.
4. **Give the tail a home** — grouped section landing pages, strong search with synonyms, and contextual entry points at the moment of relevance.
5. **Institute a rule for growth:** adding a primary nav item requires removing or demoting one, with data. Without a rule the nav re-accretes within a year, which is the actual problem to solve.
6. **Validate** with card sort → tree test → first-click before build.
7. **After launch,** compare against the baseline: task success and directness, nav click distribution, search ratio, zero-result queries, support contacts, and the discoverability of demoted features (make sure you did not silently kill a low-traffic but high-value feature — check revenue and retention impact by segment, not just clicks).

**12.** What I would run:
- **Days 1–2:** free evidence — search logs (especially zero-result and refined queries), support-ticket topic counts, analytics on current nav usage, and session recordings. This costs nothing and often identifies the failing labels outright.
- **Day 3:** a content inventory in a spreadsheet, ranked by traffic.
- **Days 4–5:** an **open card sort** with 15–20 participants recruited from existing users via an in-product prompt or email, run on a free tier tool; supplement with 3 moderated sessions to hear reasoning.
- **Days 6–7:** draft two candidate structures.
- **Days 8–10:** **tree test** both, 25–30 participants each, recruited the same way; measure success and directness on the top 6 tasks.
- **Days 11–12:** fix the weakest labels, re-test only the failing tasks.
- **Day 13:** **first-click test** on a screenshot of the proposed home screen with 5–10 people.
- **Day 14:** write up, with a redirect plan and the post-launch metrics to watch.
What I would knowingly not learn: how the structure performs for users I could not recruit (new users, non-customers, and people with accessibility needs — a real gap, since unmoderated tools under-sample assistive-technology users); how it behaves with real content volume and real personal data; longitudinal effects, including whether existing users' learned paths break (change aversion); and anything about the visual design, since tree tests deliberately exclude it. I would state these limits in the write-up rather than presenting the result as conclusive.

---

<!-- nav -->
[← Previous: 8.3 Validating IA](8.3-validating-ia.md) · [↑ Module 08 — Information Architecture](README.md) · [Next: Module 09 — UX Research →](../09-research/README.md)
