# Workflow Example

This document demonstrates the recommended workflow for using the Engineering Project Workflow Prompts repository.

The objective is to keep long-running software projects organized, maintain architectural consistency, and prevent ChatGPT conversations from becoming too large or losing context.

---

# Overall Workflow

```text
MASTER

↓

Feature Branch

↓

Development

↓

Branch Handoff

↓

Update MASTER

↓

Repeat
```

After several completed branches:

```text
MASTER

↓

Branch

↓

Branch Handoff

↓

Update MASTER

↓

Branch

↓

Branch Handoff

↓

Again Update MASTER

↓

Branch

↓

Branch Handoff

↓

MASTER becomes large

↓

Generate Master Project Continuation Plan

↓

MASTER v2

↓

Continue Development
```

---

# Step 1 — Create the Master Conversation

Create one conversation that becomes the project's long-term reference.

The Master conversation stores:

- Architecture
- Roadmap
- Engineering decisions
- Development history
- Current project status

It should **not** contain detailed implementation discussions for every feature.

---

# Step 2 — Create a Feature Branch

Whenever you begin a new Git feature branch:

Example:

```text
feature/hybrid-retrieval
```

Create a new ChatGPT conversation.

Use:

```
Prompt 1 – Master → Feature Branch
```

Then paste:

- the latest Project Continuation Plan
- the feature objective

Development happens entirely inside this conversation.

---

# Step 3 — Complete the Feature

During development:

- implement the feature
- fix bugs
- review architecture
- test functionality
- complete the branch

Avoid updating the Master conversation during implementation.

---

# Step 4 — Generate Branch Handoff

After the feature is complete:

Use:

```
Prompt 2 – Feature Branch → Master Handoff
```

This generates a complete engineering summary including:

- completed work
- architecture changes
- modified files
- dependencies
- testing
- lessons learned
- recommended next work

---

# Step 5 — Update the Master Conversation

Return to the Master conversation.

Paste the generated Branch Handoff.

The Master conversation now understands:

- what changed
- why it changed
- the latest architecture
- the current project status

The implementation conversation can now be archived.

---

# Step 6 — Repeat

Create another Git feature branch.

Example:

```text
feature/reranking

↓

Prompt 1

↓

Development

↓

Prompt 2

↓

Update MASTER
```

Repeat this workflow for every feature.

---

# Step 7 — Replace the Master Conversation

Over time the Master conversation becomes large.

Typical indicators include:

- slower responses
- repeated recommendations
- forgotten architectural decisions
- inconsistent implementation guidance

At this point use:

```
Prompt 3 – Master Project Continuation Plan
```

Generate a complete continuation document.

Create a brand-new Master conversation.

Paste:

- Prompt 1
- the generated Project Continuation Plan

Development continues without losing project history.

---

# Architecture Reviews

Before introducing significant architectural changes use:

```
Prompt 4 – Architecture Decision Review
```

Examples include:

- new frameworks
- new databases
- new design patterns
- repository restructuring
- AI agent frameworks
- vector databases

This prevents unnecessary redesigns.

---

# Engineering Reviews

Every few months perform:

```
Prompt 5 – Engineering Health & Technology Review
```

This evaluates:

- architecture quality
- technical debt
- maintainability
- dependencies
- future improvements

---

# Release Reviews

Before:

- GitHub Release
- Portfolio Update
- Major Merge
- Interview Demo

Run:

```
Prompt 6 – Release Readiness Review
```

This ensures the project is suitable for public release.

---

# Career Updates

Whenever significant features have been completed use:

```
Prompt 7 – Resume, Portfolio & Interview Translation
```

This converts engineering work into:

- Resume achievements
- LinkedIn content
- GitHub descriptions
- Interview stories

---

# Learning Reviews

Every few months run:

```
Prompt 8 – Engineering Learning & Roadmap Review
```

This keeps:

- learning priorities
- technology choices
- future roadmap

aligned with industry trends and project goals.

---

# Complete Lifecycle

```text
Create MASTER

↓

Prompt 1

↓

Feature Development

↓

Prompt 2

↓

Update MASTER

↓

Repeat

↓

Prompt 5 (periodically)

↓

Prompt 6 (before releases)

↓

Prompt 7 (career updates)

↓

Prompt 8 (learning review)

↓

MASTER becomes large

↓

Prompt 3

↓

MASTER v2

↓

Continue Development
```

---

# Benefits

Following this workflow provides:

- Small focused implementation conversations
- Stable long-term architecture
- Consistent engineering decisions
- Better ChatGPT context management
- Easier onboarding into existing projects
- Production-oriented development process
- Reusable workflow for any software project
