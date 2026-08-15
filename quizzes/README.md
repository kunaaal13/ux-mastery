# Quizzes

## In one line

Testing yourself is not how you check that you learned something — it is how you learn it, which is why every module here ends in a quiz and why this folder exists at all.

## How the quiz system is organised

There are two layers.

**Per-module quizzes** live inside each module, at `modules/NN-*/quiz.md`. Each one covers a single module in depth, in three parts: recall, short answer, and applied. Every question has a full worked solution with marking notes, so you can grade yourself honestly rather than generously.

**Cross-module assessments** live in this folder. They exist because knowing a concept inside its own chapter is a much weaker form of knowing than being able to retrieve it when nobody has told you which chapter it is from. Interviews are the second kind. So are real design problems.

| File | What it is | Questions | Target |
| --- | --- | --- | --- |
| [`mixed-exam-1.md`](mixed-exam-1.md) | Foundations exam — Modules 01–06 | 30 | 22 |
| [`mixed-exam-2.md`](mixed-exam-2.md) | Practice exam — Modules 07–13 | 30 | 22 |
| [`final-exam.md`](final-exam.md) | Comprehensive, all 13 modules, applied-weighted | 40 | 34 for interview-ready |
| [`flashcards.md`](flashcards.md) | 200+ recall cards grouped by module | — | — |
| `answer-keys/` | Reserved for any keys kept separately from their quizzes | — | — |

Note that the module quizzes and the mixed exams keep their solutions in the same file, immediately below a horizontal rule. That is deliberate: separating them adds friction that, in practice, means people stop checking. The discipline required of you is simply not to scroll.

## Module quiz index

| # | Module | Questions | Pass target |
| --- | --- | --- | --- |
| 01 | [Foundations](../modules/01-foundations/quiz.md) | 12 | 9 |
| 02 | [Psychology & Cognition](../modules/02-psychology/quiz.md) | 12 | 9 |
| 03 | [UX Laws](../modules/03-ux-laws/quiz.md) | 15 | 11 |
| 04 | [Gestalt Principles](../modules/04-gestalt/quiz.md) | 12 | 9 |
| 05 | [Heuristics & Evaluation](../modules/05-heuristics/quiz.md) | 14 | 10 |
| 06 | [Visual Design](../modules/06-visual-design/quiz.md) | 13 | 10 |
| 07 | [Interaction Design](../modules/07-interaction-design/quiz.md) | 13 | 10 |
| 08 | [Information Architecture](../modules/08-information-architecture/quiz.md) | 12 | 9 |
| 09 | [Research](../modules/09-research/quiz.md) | 14 | 10 |
| 10 | [Accessibility](../modules/10-accessibility/quiz.md) | 12 | 9 |
| 11 | [Design Systems](../modules/11-design-systems/quiz.md) | 10 | 7 |
| 12 | [Metrics & Strategy](../modules/12-metrics-strategy/quiz.md) | 12 | 9 |
| 13 | [Advanced Topics](../modules/13-advanced/quiz.md) | 12 | 9 |
| | **Total** | **163** | **121** |

The pass targets are roughly 72–75% of each quiz. They are not arbitrary: below about 70% you are recognising material rather than retrieving it, and recognition collapses under interview pressure. Above 90% on a first attempt usually means you took the quiz too soon after reading the module, and what you measured was short-term memory rather than learning.

## Retrieval practice: test before you re-read

The single most useful finding in the learning literature for this repo's purposes is that **retrieval outperforms review**. Attempting to recall something — and even failing to recall it — produces more durable learning than re-reading the passage that contains it. Re-reading feels far more productive than it is, because fluency with the text gets mistaken for knowledge of the content.

The practical rules that follow from this:

1. **Take the quiz before you think you are ready.** A quiz taken cold, with several wrong answers, teaches more than a quiz taken after a confident re-read. Aim to be uncomfortable.
2. **Attempt every question before checking any answer.** Checking as you go converts retrieval practice into reading practice.
3. **Write or say your answer out loud before revealing the solution.** A vague sense that you "know this one" is exactly the illusion the method exists to break. If you cannot produce the sentence, you do not have the answer.
4. **Grade against the marking notes, not against your intent.** The solutions in this repo state what separates a strong answer from a weak one, because in an interview the distinction between "named the mechanism" and "gestured at the idea" is the whole score.
5. **Re-read only what you got wrong.** Go back to the specific concept file, not the whole module. Then re-attempt that question a few days later, not immediately — an immediate re-attempt tests your memory of the answer key.
6. **Space it out and mix it up.** Spacing and interleaving both feel worse than blocked massed practice and both produce better retention. The mixed exams exist precisely to force interleaving; that is why they feel harder than the module quizzes covering the same material.

A useful diagnostic while grading: for each miss, label it. Was it a **retrieval failure** (you knew it and could not produce it — that needs flashcards and spacing), a **comprehension failure** (you never understood the mechanism — that needs re-reading the concept file), or an **application failure** (you knew the concept but could not deploy it in the scenario — that needs the exercises in [`../exercises/`](../exercises/), not more reading)? The three have different fixes and conflating them is why revision plateaus.

## Suggested revision schedule

Two schedules, depending on what you are doing.

### Alongside a first pass through the modules

| When | What |
| --- | --- |
| Immediately after finishing a module | Take that module's quiz cold, then read the solutions for everything you missed |
| 2 days later | Re-attempt only the questions you missed, from memory |
| 7 days later | Run the flashcards for that module |
| After Module 06 | Sit `mixed-exam-1.md` |
| After Module 13 | Sit `mixed-exam-2.md` |
| 1 week after finishing everything | Sit `final-exam.md` under exam conditions |

### As interview preparation, from a standing start

| Week | What |
| --- | --- |
| 1 | Flashcards daily, 15 minutes. Module quizzes for 01, 02, 03, 05 |
| 2 | Flashcards daily. Module quizzes for 04, 06, 07, 08. Sit `mixed-exam-1.md` |
| 3 | Flashcards daily. Module quizzes for 09, 10, 11, 12, 13. Sit `mixed-exam-2.md` |
| 4 | Re-run only the weak modules identified by the two exams. Sit `final-exam.md`. Convert every miss into a spoken 60-second answer |

Retake any exam only after at least a week has passed. Retaking it sooner measures how well you remember the solution page, which is not a quantity you have any use for.

### Spacing intervals for the flashcards

The flashcard deck uses expanding intervals of **1, 3, 7, 16, and 35 days**. A card answered correctly moves to the next interval; a card failed resets to day 1. Full mechanics are in [`flashcards.md`](flashcards.md). The important discipline is honesty about failure — a card you "nearly" got is a card you failed.

## A word on what quizzes cannot do

These quizzes test whether you hold the vocabulary and can reason with it under a little pressure. They cannot tell you whether you can run a real study, sit with a stakeholder who disagrees with you, or make a defensible call with incomplete data. That is what [`../exercises/`](../exercises/) and [`../interview-prep/mock-interviews/`](../interview-prep/mock-interviews/) are for.

Treat a strong exam score as a licence to start practising the harder thing, not as evidence that you have finished.

---

<!-- nav -->
[← Previous: Fundamentals — Rapid-Fire Concept Questions](../interview-prep/question-bank/fundamentals.md) · [↑ Contents](../README.md) · [Next: Mixed Exam 1 — Foundations →](mixed-exam-1.md)
