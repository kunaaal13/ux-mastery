# Quiz — Module 07: Interaction Design

13 questions. Target: 10/13.

---

### Part A — Recall

**1.** A signifier is:
- a) what an object can do
- b) the perceptible signal that communicates a possible action
- c) a visual style
- d) a constraint on action

**2.** Which component state is most commonly omitted?
- a) hover
- b) focus
- c) disabled
- d) active

**3.** A standard small UI transition should last roughly:
- a) 50 ms
- b) 150–250 ms
- c) 400–600 ms
- d) 1 s

**4.** Elements entering the screen should typically use:
- a) ease-in
- b) ease-out
- c) linear
- d) ease-in-out

**5.** A toggle rather than a checkbox implies:
- a) the option is required
- b) the change takes effect immediately
- c) multiple selections are allowed
- d) the field is read-only

---

### Part B — Short answer

**6.** Name the three distinct empty states and how their content should differ.

**7.** State the rule about gestures in one sentence, and give the two populations excluded when a gesture is the only path.

**8.** Give three distinct reasons placeholders-as-labels is an anti-pattern.

**9.** When is optimistic UI the wrong choice, and what must always accompany it when it is right?

**10.** Give the five-step validation priority order.

---

### Part C — Applied

**11.** A team wants to add a confirmation dialog before every delete. Respond with a recommendation and the conditions under which you would agree.

**12.** You are designing a "save article" feature. List the states you would design and identify the two carrying the most risk.

**13.** A product's checkout has a 32% drop-off on the address step. Give your diagnostic plan and the fixes you would try in priority order, with trade-offs.

---
---

## Solutions

**1. b)** The perceptible signal. An affordance is the relationship between an object's properties and an agent's capabilities; in digital interfaces almost everything we design is a signifier, because pixels afford nothing physically.

**2. b)** Focus. Omitting it makes the product unusable by keyboard, which also breaks screen-reader and switch-device navigation — an accessibility failure, not a polish issue.

**3. b)** 150–250 ms. Larger surfaces (sheets, page transitions) go 250–400 ms; anything over ~400 ms starts to feel sluggish.

**4. b)** Ease-out — fast start, gentle settle, which reads as responsive. Ease-in is for exits; ease-in-out for moves between two on-screen positions.

**5. b)** Immediate effect. A toggle inside a form with a Save button creates ambiguity about whether the change has already applied.

---

**6.** (1) **First-use empty** — the user has never had content: explain the value in one line, show what "filled" looks like, and give one primary action to get started. (2) **User-cleared empty** — the user emptied it themselves (inbox zero, completed all tasks): acknowledge the accomplishment, do not imply an error, and offer the next sensible action. (3) **No-results empty** — a search or filter returned nothing: state what was searched, and offer recovery — relax or clear filters, correct spelling, broaden the query, or browse alternatives. Using the same generic "No data" for all three makes the user suspect a bug in cases 2 and 3.

**7.** Rule: **a gesture may be an accelerator, never the only path to an action.** Excluded populations: keyboard-only users (including many motor-impairment users and power users), and assistive-technology users (screen readers, switch access) for whom the gesture is not exposed. Also affected: new users, since gestures have no signifier and so near-zero discoverability.

**8.** (a) The label disappears on focus/entry, converting recognition into recall exactly when the user needs it, and making review before submission impossible; (b) placeholder styling is typically low-contrast and usually fails WCAG contrast requirements; (c) it breaks programmatic label association, so screen-reader users may get no accessible name — and autofill behaviour is less reliable. A fourth: users frequently mistake pre-filled placeholder text for an already-entered value and skip the field.

**9.** Wrong when failure is likely, consequential, or confusing to reverse — payments, irreversible deletes, legal or financial commitments, or any action whose visible "success" would cause the user to act on false information. When it is right (likes, marking read, reordering), it must be accompanied by a **designed failure path**: the UI reverts visibly, explains what happened in plain language, and offers a retry — never a silent rollback the user discovers later.

**10.** (1) **Prevent** — constraints, structured pickers, masks, defaults, disabling impossible combinations. (2) **Accept liberally** — strip spaces and dashes, trim whitespace, accept multiple formats, normalise and echo back the interpretation. (3) **Validate at the right moment** — on blur, not on every keystroke, and never only on submit. (4) **Explain** — adjacent, specific, in the user's words, saying what is wrong and what would be right; show constraints before entry. (5) **Recover** — preserve all input, move focus to the first error, summarise with links, never clear the form.

**11.** Recommendation: **default to undo, not confirmation.** Reasoning to give:
- A dialog taxes every user on every delete to protect against a rare mistake, and repetition trains reflexive dismissal — after which it protects nobody. Measured behaviour on high-frequency confirmations shows users click through without reading.
- Undo costs nothing on the happy path and actually recovers the error, which is the goal.
Conditions under which I would agree to confirmation:
- The action is genuinely **irreversible** (no soft-delete possible, data leaves the system).
- The **blast radius is wide** (deleting a shared workspace, removing other people's access, sending to thousands of recipients).
- The cost is **high and asymmetric** (financial, legal, or destroys others' work).
And even then, make the confirmation **informative** — state exactly what will happen and at what scale ("Permanently delete 1,240 records; this cannot be undone"), and require a deliberate action proportionate to the risk (typing the name for the most destructive cases). Where possible, offer both: soft-delete with a recovery window *and* a confirmation only for permanent purge.

**12.** States for "save article":
- **Default** (not saved), **hover**, **focus**, **pressed**, **saved/selected** — the toggle must read unambiguously in both states without relying on colour alone.
- **In-flight/loading** — brief, since this should be optimistic.
- **Error** — the save failed (offline, auth expired, quota).
- **Offline** — action queued or refused, and clearly communicated.
- **Unauthenticated** — the user is not signed in; what happens to the intent after login matters.
- **Limit reached** — quota or plan cap.
- The saved *list* has its own states: first-use empty, user-cleared empty, loading, populated, overflowing (very long titles), and error.
Two highest-risk: (1) **the offline/error state after an optimistic save** — the user believes the article is saved, closes the tab, and loses it; this is a "protect users' work" failure and the most damaging outcome. (2) **the unauthenticated state** — if the intent is discarded after sign-in, the user has to find the article again, which is the point where most people abandon. Both need explicit design: queue the save and reconcile, and preserve intent across authentication.

**13.** Diagnostic plan:
1. **Segment the drop-off** — by device, country, new vs returning, and whether autofill fired. A 32% drop concentrated on mobile points to keyboard/target/autofill issues; concentrated in one country points to address-format mismatch.
2. **Field-level instrumentation** — time per field, error events per field, correction counts, and the last field touched before abandonment. This usually identifies the culprit within a day.
3. **Session recordings and rage-click detection** on that step.
4. **5 usability sessions** on the real form with real addresses, including one non-standard address.
Fixes in priority order with trade-offs:
- **Enable address autofill and correct `autocomplete` attributes** — largest cheap win; trade-off: none material, but requires correct field naming.
- **Add address lookup/autocomplete by postcode or search** — big reduction in typing and errors; trade-offs: cost of a third-party service, and it must always allow manual entry for addresses the database lacks (a failure here excludes real users entirely).
- **Fix validation** — accept liberally (spaces, case, punctuation in postcodes), validate on blur, preserve input, and make messages specific. Trade-off: none.
- **Support international address formats** — do not force a US/UK shape (state as a required dropdown, fixed postcode pattern) on users elsewhere; this is a common cause of geographically clustered abandonment. Trade-off: more layout complexity.
- **Reduce required fields** — is a phone number genuinely needed at this step? Trade-off: operations may want it for delivery contact; negotiate with a reason rather than deleting unilaterally.
- **Reorder or defer** — collect address after payment method selection only if the flow allows; trade-off: shipping cost depends on address, so deferring may hide the total, which harms trust more than it helps completion.
Close with: ship one change at a time behind an experiment, watch step-completion and downstream order-error rate together — a change that raises completion but increases failed deliveries is a net loss.

---

<!-- nav -->
[← Previous: 7.4 Forms & Inputs](7.4-forms-and-inputs.md) · [↑ Module 07 — Interaction Design](README.md) · [Next: Module 08 — Information Architecture →](../08-information-architecture/README.md)
