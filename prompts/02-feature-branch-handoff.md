# Prompt 2 — Feature Branch → Master Handoff

## Purpose

Use this prompt after completing a Git feature branch.

Generate an engineering handoff document that will be copied into the Master Project Continuation Plan.

This document becomes the permanent engineering history for the completed feature branch.

The objective is **not** to create exhaustive documentation.

The objective is to preserve every important engineering decision, repository change, architectural update, dependency change, validation result, and future recommendation so that a completely new ChatGPT conversation (or another senior engineer) can continue development without requiring additional explanation.

---

# When to Use

```text
MASTER
   │
   ├── Create Feature Branch
   │
   ├── Develop Feature
   │
   ├── Validation Complete
   │
   ├── Git Commit(s)
   │
   ├── Pull Request
   │
   ├── Merge Branch
   │
   └── Paste Prompt 2
            │
            ▼
Generate Engineering Handoff
            │
            ▼
Paste into MASTER
            │
            ▼
Continue Next Feature Branch
```

---

# Instructions

```prompt
Review the **entire conversation**, not only the most recent messages.

Treat every engineering decision made during the feature branch as part of the project history.

Do not include implementation code.

Do not omit important changes simply because they are small.

If the response exceeds the maximum response size, continue in additional parts until every required section has been completed.

Do not shorten the response by skipping sections.

Prefer concise engineering summaries instead of long explanations.

Use:

- bullet points
- tables
- grouped information
- short engineering explanations

Avoid repeating information.

Explain only files that were created, modified, or removed.

---

# Output Structure

# Project

- Project name

---

# Feature Branch

Include:

- Git branch name
- Branch status
- Merge status

---

# Branch Objective

Include:

- Original objective
- Final objective
- Scope changes
- Why the scope changed

---

# Business Value

Briefly explain:

- Why this feature exists
- Problem it solves
- Portfolio value
- Interview value
- Long-term architectural value

---

# Features Completed

For every completed feature include:

- Feature name
- Purpose
- Files affected
- Architectural impact

Group related work together when appropriate.

Do not include implementation code.

---

# Files Added

List every newly created file.

For each file include:

| File | Responsibility | Why Added |

Keep explanations to one or two sentences.

---

# Files Modified

List every modified file.

For each file include:

| File | What Changed | Why Changed |

Do not include implementation code.

---

# Files Removed

If applicable, include:

| File | Reason Removed |

---

# Dependencies

## Installed

For every newly installed dependency include:

- Package
- Purpose
- Why it was selected
- Long-term project value

---

## Updated

For every updated dependency include:

- Package
- Previous version
- New version
- Reason for update
- Impact on the project

---

## Removed

For every removed dependency include:

- Package
- Reason removed
- Replacement (if applicable)

---

# Configuration Changes

List all configuration changes made during the branch.

Examples include:

- pyproject.toml
- GitHub Actions
- pre-commit
- environment variables
- tooling
- CI/CD
- build configuration
- linting
- formatting
- testing configuration

Explain each change in one or two sentences.

---

# Architecture Changes

Explain:

Before

↓

After

Include a simple architecture diagram whenever useful.

Highlight:

- new modules
- removed modules
- dependency changes
- architectural relationships
- permanent architectural decisions introduced by this branch

---

# Engineering Decisions

List every important engineering decision.

For each decision include:

- Decision
- Reason
- Alternatives considered
- Long-term impact

---

# Problems Encountered

For every important issue include:

- Problem
- Root cause
- Investigation
- Resolution
- Final decision

Include architectural issues that were intentionally deferred.

---

# Validation Performed

List every validation completed.

Examples:

- Ruff
- Black
- MyPy
- Pytest
- Coverage
- GitHub Actions
- API testing
- UI testing
- Manual verification
- Performance validation

For each include:

- Purpose
- Result

---

# Backward Compatibility

Explain:

- Existing functionality preserved
- Breaking changes (if any)
- Migration required (if any)

---

# Technical Debt

List intentionally postponed work.

For every item include:

- Description
- Why postponed
- Recommended future feature branch

---

# Known Limitations

List everything that remains unfinished.

Be honest.

Do not hide limitations.

---

# Permanent Engineering Rules

Document any new project-wide engineering conventions established during this branch.

Examples:

- Architecture rules
- Dependency policy
- Git workflow
- Testing policy
- Configuration principles
- Documentation standards
- Coding conventions
- AI engineering principles

These become permanent project rules.

---

# Current Project Status

Summarize the current repository status.

Include:

- Completed
- In Progress
- Deferred
- Future

---

# Recommended Next Feature Branches

Recommend future branches in priority order.

For each include:

- Branch name
- Objective
- Dependencies
- Estimated complexity
- Mandatory or Optional

---

# Lessons Learned

Summarize:

- What worked well
- What should be avoided
- Architectural improvements discovered
- Engineering insights gained

---

# Final Outcome

Provide a concise summary describing exactly what this feature branch accomplished.

The summary should be understandable without reading the rest of the document.

---

End the document with one of the following:


READY TO MERGE INTO MASTER

or 

DO NOT MERGE YET


If the branch is not complete, clearly explain what remains before it should be merged into the Master Project Continuation Plan.
```
