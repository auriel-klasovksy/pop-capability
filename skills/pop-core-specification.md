POP Core Specification

Purpose

POP is a methodology for communicating software intent.

Its purpose is not to write code.

Its purpose is to create documents that preserve programmer intent while minimizing unnecessary implementation commitment.

Code is considered a derived artifact.

The collection of POP documents is the authoritative expression of the software.

---

Manifest

Intent is written directly as documentation. Implementation is derived from it.

An idea is stable when different people understand it the same way. A specification is stable when different implementations preserve the same meaning.

Editing code without specification is like editing the assembly output of compilation. 

Humans and machines both reason better about complete things.

Instead of complaining about syntax, POP complains about missing ideas and unclear meaning.

Software is a collaboration between the programmer and their compiler.

Programming is the progressive stabilization of intent.

---

Philosophy

Software is not merely implemented.

It is communicated.

Every sentence in a POP document exists to improve shared understanding.

Every unnecessary sentence reduces understanding.

The objective is not completeness.

The objective is clarity.

The objective is not precision for its own sake.

The objective is preserving meaning.

---

Semantic Density

POP values semantic density.

A document should communicate as much understanding as possible with as little ceremony as possible.

Avoid:

- repetition
- defensive wording
- implementation trivia
- unnecessary explanation

Prefer concise writing that communicates complete ideas.

A single sentence may simultaneously express intent, acknowledge a commitment, explain its reason, or reference another source of knowledge.

---

Intent

Intent describes what the software is meant to be.

Intent is sacred.

The implementer should preserve intent, not reinterpret it.

Implementation freedom exists only where intent allows it.

Specific intent is not a weakness.

If the programmer intends exactly two resources, then two resources is the correct specification.

Do not generalize intent merely because a more abstract design is possible.

---

Implementation Commitments

Implementation commitments describe how the software should be implemented rather than what the software should accomplish.

Implementation commitments are allowed.

However, every commitment should have a recorded reason.

POP does not judge the quality of the reason.

The reason may be technical, organizational, personal, temporary, or simply a matter of preference.

The purpose of recording the reason is to preserve understanding rather than justification.

Whenever possible, reasons should naturally communicate the conditions under which the commitment should be reconsidered.

---

Knowledge Ownership

Every important concept should have exactly one authoritative source.

A POP document is responsible only for the knowledge it owns.

When behavior is defined elsewhere, prefer referencing that document over duplicating its contents.

Referencing another POP document is not deferred intent.

It is an explicit acknowledgment that the concept is owned elsewhere.

Documents should strive to be locally complete while remaining globally coherent.

Every idea should have one home.

---

Concept Identity

A concept has an identity independent of the words used to describe it.

A rename changes the preferred name of a concept, not the concept itself.

A concept may evolve over time. Common forms of evolution include:

- rename
- split
- merge
- expansion
- removal
- ownership transfer

When evolving a POP document, reason about concepts rather than words.

A change to a concept may require revisiting every document that depends upon that concept.

Knowledge stability requires preserving concept identity across the entire POP knowledge base.

---

Intent State

Not every idea is equally mature.

POP recognizes four states of knowledge.

Defined

The programmer knows the intended behavior.

The document communicates it directly.

---

Referenced

The behavior is defined by another POP document.

The current document should reference that document rather than duplicate its contents.

Referenced knowledge is considered complete.

---

Deferred

The programmer intentionally leaves a decision for a future stage.

This is acceptable.

The document should explain what has been deferred and, when possible, what should guide the eventual decision.

Deferred intent is not missing intent.

---

Unknown

The programmer has not yet considered an important aspect of the design.

Unknown intent should produce findings.

---

Findings

A finding is an observation requiring programmer attention.

Findings are not errors.

They are opportunities to improve shared understanding.

The programmer may choose to:

- resolve the finding
- reference another POP document
- intentionally defer the decision
- reject the finding

All four are valid outcomes.

POP exists to expose decisions, not make them.

The goal is not the absence of findings.

The goal is the absence of unacknowledged findings.

---

Revision

Revision is a fundamental part of POP.

Writing, auditing and revision form a continuous loop.

Each revision should improve understanding while reducing unnecessary complexity.

Every revision should also attempt to simplify the document without losing meaning.

Prefer deletion over addition.

Prefer simplification over explanation.

The best revision is often the one that removes a sentence rather than rewriting it.

---

Human Collaboration

POP assumes an intelligent programmer.

POP assumes an intelligent implementer.

POP assumes intelligent future readers.

Do not ask questions simply because multiple implementations exist.

Ask questions only when multiple reasonable interpretations would produce meaningfully different software.

When a finding materially affects the resulting software, involve the programmer.

POP should never silently invent product intent.

The purpose of POP is not to answer every question.

The purpose of POP is to discover the questions that still need answering.

---

Success

A successful POP document:

- preserves programmer intent
- communicates complete ideas
- records implementation commitments together with their reasons
- distinguishes defined, referenced, deferred and unknown knowledge
- minimizes unnecessary implementation commitment
- references existing knowledge instead of duplicating it
- remains pleasant to read
- remains easy to modify
- maximizes semantic density

Perfect certainty is not required.

Shared understanding is.