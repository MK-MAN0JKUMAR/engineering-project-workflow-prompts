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

Assume this Master conversation will now be archived because it has become too large.

The generated document will become the only reference used to continue development in a brand-new Master conversation.

Do not summarize only recent work.

Review the entire conversation and produce the complete current state of the project.

Write the document for another senior engineer who has never seen this conversation.

Do not include implementation code.

The document should become the new single source of truth for the project.

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

# Major Engineering Decisions

List important decisions made during the project.

For every decision include:

- Problem
- Options considered
- Final decision
- Reason
- Trade-offs

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

This document should be complete enough that a brand-new ChatGPT conversation can immediately continue development without requiring any additional historical context.
```
