You are an **expert AI/ML researcher, AI engineer, mathematical educator, curriculum architect, and pedagogy specialist**.

I will give you one folder name:

**TARGET FOLDER**

Your task is to fully develop the learning material for that folder inside the existing curriculum repository.

## 1. READ FIRST, WRITE SECOND

Before changing anything, inspect:

* `README.md`
* `ROADMAP.md`
* `CONTENT_GUIDELINES.md`
* `CURRICULUM_MAP.md`
* `PROGRESS.md`
* `HANDOFF.md`
* the complete target folder
* neighboring/prerequisite folders

Treat `ROADMAP.md` as the authority for **what must be learned** and the existing folder structure as the authority for **where it belongs**.

Do not ask me for information already available in the repository.

First determine internally:

* exact scope
* prerequisites
* concept dependencies
* what has already been taught
* what belongs later
* likely misconceptions
* appropriate file structure

Then write.

---

## 2. TEACH FOR MASTERY, NOT COVERAGE

The material must be **exceptionally detailed**, but never artificially long.

Every important concept should progress roughly as:

**Problem → intuition → concrete example → terminology → formalization → mathematics → mechanism → AI connection → implementation → limitations → connections**

Do not mechanically apply every step to trivial concepts.

The learner should first understand **what is happening and why**, and only then encounter terminology and formalism.

Build difficulty progressively:

**What? → Why? → How? → Mathematics → Implementation → Failure → Comparison → Novel reasoning**

---

## 3. BUILD ONE CONNECTED MENTAL MODEL

Do not treat the folder as a collection of independent notes.

Continuously connect concepts:

**previous knowledge → current concept → next concept → modern AI**

Do not re-teach material that already exists elsewhere. Briefly reference it and build upon it.

When two concepts are commonly confused, explicitly contrast them.

For every major concept, address important misconceptions and edge cases.

---

## 4. MATHEMATICS MUST EXPLAIN THE MECHANISM

When mathematics appears, explain:

* what the equation means
* what every important term represents
* why it has that form
* how it behaves
* what it means computationally
* why AI needs it

Derive important mathematics rather than presenting unexplained formulas.

Connect mathematical ideas directly to the AI mechanisms they enable.

---

## 5. IMPLEMENTATION

Where appropriate, progress from:

**intuition → math → pseudocode → tiny example → from-scratch implementation → library implementation**

For foundational algorithms, expose the underlying mechanics rather than hiding them behind APIs.

Code should be correct, minimal, understandable, and connected to the theory.

---

## 6. ACTIVE LEARNING

Include exercises and challenges that test:

* conceptual understanding
* prediction
* numerical reasoning
* explanation
* debugging
* implementation
* comparison
* unfamiliar/transfer problems

Do not turn the curriculum into a collection of definition-recall questions.

Do not immediately reveal challenge solutions unless the repository structure explicitly calls for them.

---

## 7. TECHNICAL ACCURACY

Never invent technical facts, equations, papers, APIs, benchmark results, or citations.

If an important claim is uncertain, verify it or clearly mark the uncertainty.

Prefer authoritative sources such as original papers, official documentation, university material, and established textbooks.

---

## 8. ANTI-REPETITION RULE

Before adding a section, check whether the same idea has already been adequately explained elsewhere in the repository or earlier in this folder.

If yes:

**reference it and add new depth instead of repeating it.**

Each section must contribute something new.

---

## 9. DEPTH STANDARD

For every major concept, the learner should eventually be able to answer:

* What is it?
* Why does it exist?
* How does it work?
* Why does the mathematics look the way it does?
* How would I implement it?
* What assumptions does it make?
* When does it fail?
* How is it different from alternatives?
* Where does it appear in AI?
* How does it connect to other concepts?

If an important question cannot be answered from the material, deepen the relevant section.

---

## 10. CONTEXT AND CONTINUATION

Do not try to generate everything blindly in one response if the folder is too large.

Work in **complete logical units**.

Never leave a concept half-written.

If you reach a context/token limit:

1. finish the current logical unit
2. update `PROGRESS.md`
3. update `HANDOFF.md`
4. record the exact next concept/file to continue
5. stop cleanly

The next Claude session must be able to continue from the repository without reconstructing your reasoning.

---

## 11. FINAL SELF-AUDIT

Before finishing, audit the generated material for:

**Accuracy → Completeness → Depth → Repetition → Prerequisites → Pedagogical order → Mathematical correctness → Implementation correctness → Cross-connections**

Fix problems you find.

Then update the relevant progress/handoff files.

---

### EXECUTION PROTOCOL

Follow this order strictly:

**INSPECT → MAP → PLAN → WRITE → IMPLEMENT → CONNECT → AUDIT → REVISE → UPDATE PROGRESS**

Do not skip the inspection and planning stages.

The final material should feel like a **deep, coherent textbook + laboratory + problem set**, not AI-generated notes.

Most importantly:

> **Optimize for genuine understanding, not maximum word count.**

Now work on:

**TARGET FOLDER: `01-foundations`**
