# Prompt 3 — Master → Master v2 (Project Continuation Plan)

## Purpose

Use this prompt when the current Master conversation becomes too large, slow, starts forgetting earlier decisions, or loses architectural consistency.

The goal is to generate a new Master Project Continuation Plan that captures the complete project state without carrying thousands of previous messages.

The new Master conversation should continue development seamlessly from this document.

## When to Use
```
MASTER
   │
   ├── Branch
   │      │
   │      └── Branch Handoff
   │
   ├── Branch
   │      │
   │      └── Branch Handoff
   │
   ├── Branch
   │      │
   │      └── Branch Handoff
   │
   ├── Many More Feature Branches...
   │
   ├── Master becomes large / slow
   │
   └── Paste Prompt 3
            │
            ▼
Generate Master Project Continuation Plan
            │
            ▼
Create New Chat
            │
            ▼
Paste Prompt 1
            │
            ▼
Paste New Project Continuation Plan
            │
            ▼
Continue Development
```

---

# Prompt
```
Generate a complete Master Project Continuation Plan for this project.

Assume this Master conversation is being archived because it has become too large to continue efficiently.

The generated document will become the architectural baseline and the only project history used by future Master conversations.

Review the **entire conversation**, not only the most recent messages.

Preserve all important engineering decisions, completed feature branches, architectural changes, permanent project rules, configuration decisions, dependency changes, and future roadmap items.

Do not include implementation code.

Write the document as if another senior engineer will continue the project months later without access to this conversation.

If the response exceeds the maximum response size, continue in additional parts until every required section has been completed.

Do not omit sections because of response length.

Use the following structure.

# Project Overview

Include:

- Project name
- Primary objective
- Current development phase
- Overall roadmap
- Final expected outcome

# Long-Term Vision

Explain:

- What this platform is intended to become
- Engineering philosophy
- Architectural goals
- Scalability goals
- AI strategy
- Testing strategy
- Future extensibility

# Repository Structure

Provide the latest repository structure.

Include only meaningful folders and major modules.

# Technology Stack

Document only technologies currently adopted by the repository.

Do not include planned technologies that have not yet been implemented.

For each technology explain:

- Current role
- Why it was selected
- Future replacement strategy (if applicable)

List:

- Languages
- Frameworks
- Libraries
- AI Frameworks
- Agent Frameworks
- Evaluation Frameworks
- Vector Databases
- Embedding Models
- LLM Providers
- UI Frameworks
- Databases
- CI/CD
- Containerization
- Cloud Services
- Observability
- Utilities

Explain why each major technology exists.

# Architecture Overview

Describe the complete architecture.

Include diagrams whenever useful.

Show the complete execution flow.

Example:

User

↓

UI / API

↓

Document Processing

↓

Chunking

↓

Embeddings

↓

Vector Database

↓

Retrieval

↓

Reranking

↓

Prompt Building

↓

LLM

↓

Evaluation

↓

Reporting

↓

Response

Also describe:

- provider architecture
- plugin architecture
- configuration architecture
- dependency flow

# Current Modules

Describe every important module.

For each include:

- responsibility
- dependencies
- current maturity
- future plans

# Current Design Patterns

Document every important pattern currently used.

Examples:

- Factory
- Strategy
- Provider
- Dependency Injection
- Plugin
- Registry
- Adapter
- Configuration
- Pipeline

Explain why each exists.

# Current Configuration

Document every major configuration area.

Include:

- Providers
- Models
- Embeddings
- Retrieval
- Chunking
- Evaluation
- Logging
- UI
- Feature Flags
- Environment Variables

Explain the purpose of each.

# Development History

Organize by Git feature branch.

For every completed branch include:

- Branch name
- Objective
- Features implemented
- Architecture changes
- Important files
- Major engineering decisions
- Outcome

Do not omit completed branches.

# Repository Evolution

Summarize how the repository evolved throughout the project.

Organize by feature branch.

For each branch include:

- Branch name
- Repository impact
- Major files added
- Major files modified
- Dependencies introduced or updated
- Architectural significance

Keep each branch summary concise.

The objective is to understand how the repository evolved over time without reading every individual branch handoff.

# Major Engineering Decisions

List important decisions made during the project.

For every decision include:

- Problem
- Options considered
- Final decision
- Reason
- Trade-offs

# Permanent Architectural Constraints

Document every permanent architectural constraint currently governing the project.

Examples:

- Stable package namespace
- Dependency direction
- Provider abstraction
- Configuration boundary
- Replaceable infrastructure
- Plugin architecture
- Backward compatibility policy

These constraints should only change through an approved architectural redesign.

# Problems Solved

Document important bugs, architectural problems and implementation challenges.

For each include:

- Root cause
- Solution
- Lessons learned

# Engineering Standards

Document all permanent project rules.

Examples:

- Configuration-first
- Factory before conditionals
- No duplicated business logic
- Backward compatibility
- Small incremental refactoring
- Production-ready code
- Open-source-first
- AI provider abstraction
- Testing strategy

These rules become mandatory for future development.

# Current Technical Debt

List intentionally postponed work.

For every item explain:

- Why postponed
- Impact
- Suggested future branch

# Known Limitations

List current limitations honestly.

Do not hide unfinished work.

# Current Project Status

Categorize everything into:

Completed

In Progress

Deferred

Blocked

Future

# Immediate Next Priorities

List the next recommended feature branches.

For each include:

- Objective
- Business value
- Engineering value
- Dependencies
- Estimated complexity
- Priority

Recommend removing work that no longer provides meaningful value.

# Long-Term Roadmap

Divide the roadmap into future phases.

For every phase include:

- Objective
- Major features
- Expected outcome

# Current Architecture Diagram

Provide one clean architecture diagram representing the entire platform.

Keep it concise but complete.

# Portfolio / Interview Summary

Describe this project as if presenting it during a senior SDET / AI Engineer interview.

Highlight:

- Architecture
- Scalability
- AI Engineering
- Testing Strategy
- Engineering Decisions
- Maintainability
- Extensibility

# Development Continuation Instructions

Document how future development should continue.

Include:

- Coding style
- Architecture rules
- Configuration principles
- Refactoring guidelines
- Dependency rules
- Testing expectations
- Documentation standards

Future conversations should automatically follow these rules.

# Working Agreement

Future development should automatically:

- Follow the existing architecture.
- Avoid unnecessary redesigns.
- Reuse existing components whenever possible.
- Prefer extension over replacement.
- Ask only for required files.
- Preserve backward compatibility whenever practical.
- Keep implementation production-ready.
- Recommend improvements only when they provide measurable long-term value.

# Final Snapshot

End with a concise project snapshot containing:

- Current Phase
- Current Master Version
- Current Git Status
- Architecture Maturity
- Major Completed Features
- Current Technology Stack
- Current Blockers
- Next Recommended Feature Branch
- Overall Project Health

This document should become the authoritative continuation plan for the project.

Future feature branches should extend this document rather than replace it.

The continuation plan should preserve sufficient engineering history that future development can continue without referring back to archived conversations.

End with a concise project snapshot containing:

- Master Version
- Repository Status
- Architecture Status
- Current Development Phase
- Active Git Strategy
- Next Recommended Feature Branch
- Overall Project Health
```
