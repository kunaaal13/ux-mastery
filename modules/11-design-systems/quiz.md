# Quiz — Module 11: Design Systems

10 questions. Target: 7/10.

---

### Part A — Recall

**1.** Components should consume which tier of tokens?
- a) primitive
- b) semantic
- c) raw hex values
- d) component-level only

**2.** Atomic Design's levels are atoms, molecules, organisms, templates, and:
- a) systems
- b) patterns
- c) pages
- d) layouts

**3.** The best measure of a design system's success is:
- a) number of components
- b) adoption across product surfaces
- c) documentation page count
- d) Figma library file size

**4.** A component with twenty boolean props usually indicates:
- a) good flexibility
- b) a need for composition instead of configuration
- c) correct abstraction
- d) proper token usage

---

### Part B — Short answer

**5.** Name the five layers of a design system, and say which is most often neglected and why that matters.

**6.** Explain why semantic tokens make dark mode and theming tractable.

**7.** Give the test for whether something belongs in the system, and the cost of promoting too early.

**8.** Name four reasons design systems die.

---

### Part C — Applied

**9.** A product team says the system's table component does not support what they need and they are going to build their own. Respond, including what you would do in the next two weeks.

**10.** You are the first designer hired to build a design system at a 60-person company with four product teams and no system today. Describe your first 90 days, including what you would build first and how you would measure progress.

---
---

## Solutions

**1. b)** Semantic (role-based) tokens. Primitives sit behind them; components referencing primitives directly defeat theming and make misuse invisible in review.

**2. c)** Pages.

**3. b)** Adoption. Component count measures activity, not value — a large library nobody uses has made consistency worse, because it added a maintenance cost with no return.

**4. b)** Composition over configuration. A long prop list usually means several distinct components are hiding inside one, and each new flag multiplies the states nobody tests.

---

**5.** **Foundations/tokens**, **components**, **patterns**, **guidelines**, and **tooling/infrastructure**. The most neglected is **patterns** — the compositions that solve recurring problems like forms, empty states, error handling, filtering, and page templates. It matters because consistency at the pattern level is what users actually perceive: two teams can use identical components and still produce two completely different form experiences. Patterns are also where most accessibility and content decisions live.

**6.** Semantic tokens name a colour by **role** (`color-text-primary`, `color-surface-raised`, `color-border-danger`) rather than by value. Components reference roles, so switching to dark mode, a high-contrast mode, or a white-label brand is a remapping of role→value in one place, rather than an edit at every use site. It also makes misuse reviewable — a `danger` token on a neutral border is visibly wrong in a diff, while a hex value is not — and it keeps contrast decisions centralised, so an accessibility fix applies everywhere at once.

**7.** Test: **repetition plus stability** — used in three or more places, with behaviour that has settled. Cost of promoting too early: every consumer inherits churn. Each change to a system component forces coordination, migration, and re-testing across teams; if the pattern is still evolving weekly, that churn is paid repeatedly by everyone, and repeated breakage teaches teams that the system is unreliable, which suppresses adoption far longer than the component saves time.

**8.** Any four: built without consumers so it does not fit real needs; too slow to respond, so teams ship around it and never return; no owner, so it rots and becomes untrustworthy; too rigid with no escape hatch, so teams fork silently; documentation that lists props rather than guiding decisions; measuring component count instead of adoption; and breaking changes shipped without migration paths, which makes upgrading expensive enough that teams pin an old version forever.

**9.** Response and plan:
- **Do not say no.** A team about to fork is telling me the system has a gap, and if I refuse, I lose visibility permanently and they will build their own for everything after this too.
- **Week 1 — understand the actual need.** Sit with them and look at the real use case: what does the table have to do that ours does not — column resizing, virtualisation for large datasets, row grouping, inline editing, sticky columns, bulk selection? Distinguish a genuine capability gap from a discoverability gap; if our component can already do it, the failure is my documentation, and I fix that immediately because other teams will hit the same wall.
- **If it is a real gap — agree a plan in the open.** Either (a) I extend the system component on a committed timeline they can plan around, or (b) they build it in their product, using our tokens and our accessibility spec, with an agreed intent to promote it once it has proven itself in two or three places. Option (b) is usually right: it is faster for them and lower risk for everyone else.
- **Constraints I would hold firm on:** tokens, accessibility semantics (keyboard operation, name/role/state, focus management), and content/interaction conventions. Those are the parts that hurt users when they diverge; visual specifics matter less.
- **Week 2 — write it down.** Log the gap publicly in the system backlog with the team named, so other teams can find it and pile on if they need it too. Add a documented escape-hatch procedure if none exists, so the next team forks *visibly* rather than silently.
- **Follow up:** revisit in a month and promote if it has stabilised; if two other teams have hit the same need, prioritise it above whatever was next.

**10.** First 90 days:
- **Days 1–20 — audit and listen, build nothing.**
  - Interface inventory: screenshot every surface across the four products and catalogue the variation — how many button styles, input styles, type sizes, greys, spacing values, and modal patterns exist. The count is the argument; teams are usually shocked by it.
  - Interview all four teams plus engineering leads: what do they rebuild most often, what slows them down, where do bugs and accessibility defects cluster.
  - Check what already exists in code — there is usually a partial component library nobody documented.
  - Deliverable: an audit with the variation counts, the top pain points, and a proposal with a scope I can actually deliver.
- **Days 20–50 — foundations and the highest-pain components.**
  - **Tokens first** — colour (with accessible contrast verified in both themes), type scale, spacing scale, radius, elevation, motion. This is the highest-leverage layer and unblocks everything else.
  - Then the 6–10 components teams rebuild most: button, input with label/error, select, checkbox/radio, modal, toast/inline message, table or list row, card. Each with all states, accessibility spec, and content guidance.
  - Ship them into **one** product team's real work as the pilot, so the first version is validated by production use rather than by my own taste.
- **Days 50–90 — patterns, documentation, and process.**
  - Document the patterns that cause the most inconsistency: form layout and validation, empty states, error handling, loading, and page templates.
  - Set up governance: how to propose, how to contribute, how breaking changes are announced, and a documented escape hatch. Start office hours.
  - Establish design–code parity: one token source generated into both, matching names, versioned releases with a changelog.
- **Measure:** baseline the variation counts from the audit, then track adoption (share of surfaces and design files using library components), detached-instance rate, one-off components created outside the system, time-to-first-screen for a new hire, support-request turnaround, and accessibility defects found in audit. Report against the baseline monthly.
- **What I would explicitly not do:** try to cover every component in 90 days, mandate adoption, or measure success by component count. The goal at 90 days is that one team's work is measurably faster and the other three want in.

---

<!-- nav -->
[← Previous: 11.2 Governance & Adoption](11.2-governance-and-adoption.md) · [↑ Module 11 — Design Systems](README.md) · [Next: Module 12 — Metrics & Strategy →](../12-metrics-strategy/README.md)
