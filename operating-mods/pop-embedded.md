POP Operating Profile: Embedded

This profile embeds POP into an existing software project.

POP does not replace the project's existing workflows.

It becomes another authoritative source of knowledge alongside them.

---

Purpose

POP owns only the software intent that has been explicitly transferred into POP documents.

Everything else continues to be owned by the existing project.

The purpose of this profile is to allow POP to improve communication incrementally without requiring the project to be rewritten.

---

Ownership

Treat every POP document exactly as you would treat source code.

However, only concepts explicitly owned by POP belong to POP.

Everything else remains owned by the existing project.

Do not attempt to migrate concepts into POP unless requested.

Respect ownership boundaries.

---

Source of Truth

Determine the authoritative source before making changes.

Examples:

- POP documents own software intent.
- Existing code may own implementation.
- Architecture documents may own system topology.
- API specifications may own interfaces.
- Balance spreadsheets may own numerical tuning.

Always modify the artifact that owns the requested knowledge.

---

Evolution

When a requested change affects POP-owned concepts:

1. Evolve the POP documents.
2. Preserve knowledge stability.
3. Run the POP pipeline.
4. Reflect the accepted intent into the implementation.

When a requested change affects knowledge owned elsewhere:

Respect that artifact instead.

Do not duplicate knowledge inside POP.

---

Shared Concepts

Some concepts may be referenced by both POP and non-POP artifacts.

Treat POP as authoritative only for the intent it explicitly owns.

Never overwrite knowledge owned by another artifact.

When inconsistencies arise, surface them rather than guessing which artifact should win.

---

Implementation

Implementation may be modified directly when implementation itself is the authoritative artifact.

When implementation changes software intent owned by POP, evolve the corresponding POP documents first.

If implementation diverges from POP-owned intent, surface the inconsistency.

Do not silently resolve it.

---

Collaboration

Assume POP adoption is incremental.

Do not encourage unnecessary migration.

Only recommend moving knowledge into POP when doing so improves communication or establishes clearer ownership.

POP should be a good citizen within the project's existing ecosystem.

Its goal is collaboration, not replacement.

---

Philosophy

POP earns ownership.

It does not demand it.

Every concept should have one authoritative home.

That home does not have to be POP.