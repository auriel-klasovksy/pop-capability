POP Working Agreement

This agreement defines how the programmer and the implementer collaborate.

It complements the POP Core Specification and the POP Pipeline.

Those documents define POP.

This document defines how we work together while using it.

---

Session Initialization

At the beginning of every session:

1. Read the POP Core Specification.
2. Read the POP Pipeline.
3. Read every relevant POP document for the requested work.

These documents are the project's authoritative source of intent.

Assume nothing that is not expressed by them.

---

Source of Truth

Treat POP documents exactly as you would treat source code in a traditional software project.

They are the project's authoritative source.

Implementation is a compiled artifact derived from them.

Code may be inspected to understand the current implementation.

Code must never become the authoritative description of the software.

When POP and implementation disagree, POP is correct.

---

Default Behaviour

Assume every request is a request to evolve software intent.

The default response is therefore:

- evolve the relevant POP documents
- preserve knowledge stability
- run the POP pipeline
- wait for implementation to be requested

Do not implement software unless explicitly instructed.

---

Software Evolution

Treat changes as semantic operations rather than textual edits.

Before modifying a POP document, determine whether the request represents:

- a new concept
- a renamed concept
- a refined concept
- a split
- a merge
- a removal
- a transfer of ownership

Preserve concept identity.

When concepts evolve, determine whether dependent POP documents should evolve as well.

Treat this exactly as updating dependent source files after changing a shared interface.

---

Programmer Collaboration

Resolve findings autonomously whenever programmer intent can be preserved confidently.

When a finding represents a genuine product decision, involve the programmer.

Ask the smallest possible question that resolves the uncertainty.

Do not ask implementation questions unless implementation itself has become part of the intended software.

---

Knowledge Stability

The POP knowledge base should remain internally consistent.

When a concept evolves:

- preserve its identity
- update dependent references where necessary
- avoid duplicated knowledge
- preserve document ownership

Treat inconsistencies between POP documents as seriously as inconsistencies between source files.

---

Document Classification

Only documents that explicitly declare themselves as POP artifacts participate in the POP methodology.

Example:

Type: POP Intent

All other artifacts remain authoritative within their own domain.

POP should integrate with them rather than replace them.

---

Implementation

Implementation follows accepted POP documents.

The implementation should treat those documents as its sole source of software intent.

Direct code edits are appropriate for:

- experimentation
- debugging
- investigation
- temporary fixes

Such edits become permanent only after the corresponding POP documents have evolved.

If a lasting software change is not reflected in the POP knowledge base, it does not exist.

---

Trigger Phrases

The following phrases modify the default workflow.

Implement

Begin implementation using the current POP knowledge base as the authoritative source.

---

Rebuild

Discard assumptions derived from the existing implementation.

Reimplement the software entirely from the current POP knowledge base.

Do not preserve behaviour that is not captured by the POP documents.

---

Do It

Choose whether to implement incrementally or rebuild from the POP knowledge base.

Briefly explain the decision before proceeding.

---

Philosophy

Our objective is not to maintain code.

Our objective is to maintain understanding.

Software evolves by changing intent.

Implementation follows.

Treat POP documents with the same discipline traditionally reserved for source code.

Treat implementation with the same freedom traditionally reserved for compiled artifacts.