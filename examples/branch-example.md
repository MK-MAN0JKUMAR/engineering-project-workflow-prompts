# Branch Workflow Example

This document demonstrates the recommended workflow for developing long-running software projects using the Engineering Project Workflow Prompts.

---

# Example Project

```
Enterprise AI Testing Platform
```

---

# Current Master

```
Master v1
```

Contains:

- Overall architecture
- Completed feature branches
- Project roadmap
- Engineering decisions
- Current project status

Master is the single source of truth.

---

# Step 1 — Create a Feature Branch

Git Branch

```bash
git checkout -b feature/hybrid-retrieval
```

Open a new ChatGPT conversation.

Paste:

```
Prompt 1 – Master → Feature Branch
```

Then paste:

```
Latest Master Project Continuation Plan
```

Development begins.

---

# Step 2 — Implement Feature

During development:

```
Review Architecture

↓

Request Required Files

↓

Implement Changes

↓

Test

↓

Review

↓

Repeat
```

Example:

```
feature/hybrid-retrieval

✓ BM25 Retriever

✓ FAISS Retriever

✓ Reciprocal Rank Fusion

✓ Retriever Factory

✓ Metadata Filtering

✓ Tests

✓ Documentation
```

---

# Step 3 — Complete Feature

After implementation:

```
Run Tests

↓

Verify Architecture

↓

Verify Backward Compatibility

↓

Finalize Feature
```

Example:

```bash
git add .
git commit -m "feat: implement hybrid retrieval using BM25 and FAISS"
```

---

# Step 4 — Generate Branch Handoff

Paste:

```
Prompt 2 – Feature Branch → Master Handoff
```

ChatGPT generates:

```
Engineering Handoff Document
```

Includes:

- Features completed
- Files modified
- Architecture changes
- Decisions
- Problems solved
- Testing
- Remaining work

---

# Step 5 — Update Master

Return to the Master conversation.

Paste:

```
Branch Handoff
```

Master now knows:

```
Hybrid Retrieval

↓

Current Architecture Updated

↓

Roadmap Updated
```

Feature branch conversation can now be archived.

---

# Step 6 — Start Next Feature

Create another Git branch.

Example:

```bash
git checkout -b feature/parent-document-retrieval
```

Create a new ChatGPT conversation.

Paste:

```
Prompt 1
```

Paste:

```
Latest Master Project Continuation Plan
```

Continue development.

---

# Master Lifecycle

```
Master
    │
    ├── feature/hybrid-retrieval
    │         │
    │         └── Prompt 2
    │
    ├── feature/parent-document-retrieval
    │         │
    │         └── Prompt 2
    │
    ├── feature/langgraph-support
    │         │
    │         └── Prompt 2
    │
    ├── feature/mcp-support
    │         │
    │         └── Prompt 2
    │
    └── Continue...
```

---

# When Master Becomes Large

Eventually:

```
Master
```

becomes:

- Slow
- Starts forgetting earlier decisions
- Gives inconsistent recommendations
- Becomes difficult to maintain

At this point:

Paste:

```
Prompt 3 – Master Project Continuation Plan
```

Generate:

```
Master Project Continuation Plan
```

Create a brand-new Master conversation.

Paste:

```
Prompt 1
```

Then paste:

```
New Master Project Continuation Plan
```

Development continues without losing project history.

---

# Complete Lifecycle

```
Master v1
      │
      ├── Feature Branch
      │       │
      │       └── Prompt 2
      │
      ├── Feature Branch
      │       │
      │       └── Prompt 2
      │
      ├── Feature Branch
      │       │
      │       └── Prompt 2
      │
      ├── Feature Branch
      │       │
      │       └── Prompt 2
      │
      └── Master grows large
              │
              ▼
       Prompt 3
              │
              ▼
          Master v2
              │
              ▼
     Continue Development
```

---

# Workflow Summary

| Step | Action | Prompt |
|------|--------|--------|
| 1 | Create Git feature branch | Prompt 1 |
| 2 | Develop feature | Prompt 1 |
| 3 | Complete implementation | — |
| 4 | Generate engineering handoff | Prompt 2 |
| 5 | Update Master | Prompt 2 Output |
| 6 | Start next feature branch | Prompt 1 |
| 7 | Replace Master when it becomes large | Prompt 3 |

---

# Benefits

- Small, focused implementation chats
- Master remains the single source of truth
- Minimal context growth
- Consistent architecture decisions
- Easy recovery if a branch goes wrong
- Long-term maintainability for multi-year projects
- Suitable for enterprise-scale AI and software engineering projects
