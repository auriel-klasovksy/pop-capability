# Setting Up a POP Project in Claude

This guide walks you through creating a Claude Project configured for POP. It assumes you have read the POP documentation and understand the methodology.

---

## Why a Project

Claude Projects give you a persistent workspace where uploaded files are available in every conversation. This makes them the natural home for POP — your skills and working agreement load automatically at the start of every session without you having to paste them in.

---

## Step 1 — Create a Project

Open Claude and create a new Project. Give it a name that reflects your software, not the methodology — you will likely have one Project per software initiative.

---

## Step 2 — Upload the POP Files

From the POP GitHub repository, upload the following to your Project's file library:

- All files from the `skills/` folder
- The POP Native operating mode from the `operating-mods/` folder

These files become part of every conversation in the Project. Claude reads them automatically at the start of each session.

---

## Step 3 — Add Your POP Documents

If you are starting a new project, you have no POP documents yet — skip this step and create them in your first session.

If you are embedding POP into an existing project, upload any POP intent documents you have already written. Remember to declare each one on its first line:

```
Type: POP Intent
```

Only files with this declaration participate in the POP methodology.

---

## Step 4 — Configure the Project Instructions

In your Project's system prompt or instructions field, add the following:

```
This project uses the POP methodology. Follow the POP Working Agreement 
uploaded to this project. At the start of every session, read the POP 
Core Specification and POP Methodology before doing anything else.
```

This ensures Claude initialises correctly even if the conversation starts abruptly.

---

## Step 5 — Start Your First Session

Begin with a clear statement of what you want to build or evolve. You do not need to invoke the pipeline manually — Claude will run it as part of the default behaviour defined in the working agreement.

A good opening for a new project:

> I want to start a new POP project. Here is what I am building: [description]

A good opening for an existing session:

> Continue from the POP documents in this project. I want to evolve [area of intent].

---

## What to Expect

Claude will evolve your intent documents, run the pipeline, surface findings, and wait for you to request implementation. If you want to proceed to code, say **Implement**. If you want a full rewrite from the documents, say **Rebuild**. If you want Claude to choose, say **Do it**.

Your POP documents accumulate in the Project over time and become the authoritative description of your software. Treat them accordingly.

---

## Tips

**Keep documents short.** POP documents are most useful when they are pleasant to read. Resist the temptation to make them exhaustive.

**Name documents clearly.** Use names that reflect what the document owns, not what it describes — `feed-view`, `mechanics`, `animations` rather than `frontend-spec`, `game-design-document`.

**One concept, one home.** If you find yourself writing the same idea in two documents, one of them should reference the other instead.

**Use the working agreement.** If Claude starts drifting toward implementation before you asked for it, point back to the agreement. It is there to govern the collaboration, not just to read once.
