# Prompt 2 — Feature Branch → Master Handoff

## Purpose

Use this prompt after completing a Git feature branch.

It generates a complete engineering handoff that will be copied into the Master conversation.

This document becomes the permanent engineering history for that branch.

## When to Use
```
MASTER
   │
   ├── Create Feature Branch
   │
   ├── Develop Feature
   │
   ├── Testing Complete
   │
   ├── Git Commit(s)
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
Merge Git Branch
```

---

# Prompt
```
Generate a complete engineering handoff document for this Git feature branch.

Assume this document will be copied into the Master Project Continuation Plan and will become the permanent engineering history for this branch.

Do not summarize only the most recent messages.

Review the entire conversation before generating the document.

Do not include implementation code.

Write the document as if another senior engineer will continue development months later without access to this branch.

The document must be complete enough that a completely new ChatGPT conversation can continue development without asking me to explain anything again.

Use the following structure.

# Project

Project name

# Feature Branch

Git branch name

# Branch Objective

Include:

- Original objective
- Final objective
- Scope changes (if any)
- Why the scope changed

# Business Value

Explain:

- Why this feature exists
- What problem it solves
- Portfolio value
- Interview value
- Long-term architectural value

# Features Completed

For every completed feature explain:

- What was implemented
- Why it was implemented
- Files affected
- User-visible impact
- Architectural impact

Do not include code.

# Architecture Changes

Explain:

Before

↓

After

Include architecture diagrams whenever useful.

Highlight:

- new layers
- removed layers
- modified relationships
- dependency changes

# New Components

List every new:

- file
- class
- interface
- provider
- factory
- strategy
- service
- manager
- utility
- helper
- configuration
- design pattern

For each component explain:

- responsibility
- dependencies
- why it was introduced

# Existing Files Modified

For every modified file explain:

- why it changed
- what changed
- architectural impact

Do not include implementation code.

# Configuration Changes

Include:

- configuration updates
- feature flags
- constants
- environment variables
- provider settings
- model settings
- retrieval settings
- evaluation settings
- UI configuration

Explain why each change was required.

# Dependencies

List:

Installed

Updated

Removed

For every dependency explain:

- purpose
- alternatives considered
- long-term maintenance impact

# Problems Encountered

For every important issue include:

- error
- root cause
- investigation
- solution
- final decision

Include architectural problems that were intentionally not solved.

# Design Decisions

List important engineering decisions.

For every decision explain:

- options considered
- chosen solution
- why it was selected
- trade-offs
- rejected alternatives

# Testing Performed

List every validation completed.

Examples:

- CLI
- Streamlit
- API
- Retrieval
- Hybrid Retrieval
- Metadata Filtering
- Parent Retrieval
- Upload
- Evaluation
- Provider Switching
- Reports
- Logging
- Performance
- Regression

For each include:

- what was tested
- result
- remaining concerns

# Performance Impact

If applicable include:

Before

↓

After

Include measurements whenever available.

Examples:

- retrieval latency
- indexing speed
- evaluation speed
- memory usage
- startup time

Explain any regressions.

# Backward Compatibility

Explain:

- what existing functionality remained unchanged
- any migration required
- compatibility risks

# Technical Debt

List intentionally postponed work.

For every item explain:

- why postponed
- impact
- recommended future branch

# Known Limitations

List everything still unfinished.

Be completely honest.

Do not hide limitations.

# Current Architecture

Provide a concise architecture diagram representing the project after this branch.

Show only meaningful components.

# Current Project Status

Completed

In Progress

Deferred

Blocked

Future

# Recommended Next Feature Branches

List the next implementation priorities in order.

For every recommendation include:

- objective
- expected value
- dependencies
- estimated complexity
- whether it is mandatory or optional

Recommend removing work that no longer provides meaningful value.

# Engineering Rules Learned

If this branch established new engineering conventions, document them.

Examples:

- architectural rules
- coding conventions
- dependency rules
- configuration principles
- testing practices
- AI engineering principles

These become permanent project rules.

# Lessons Learned

Summarize:

- what worked well
- what should be avoided
- architectural improvements discovered
- engineering insights gained

# Final Outcome

Provide a concise summary describing exactly what this feature branch accomplished.

The summary should be understandable without reading the rest of the document.

End the document with:

READY TO MERGE INTO MASTER

if the branch is considered complete.

Otherwise end with:

DO NOT MERGE YET

and explain what still needs to be completed.
```
