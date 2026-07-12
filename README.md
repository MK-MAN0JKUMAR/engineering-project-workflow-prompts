# Engineering Project Workflow Prompts

A reusable collection of enterprise software engineering workflow prompts for managing long-term software projects with ChatGPT.

These prompts help maintain architectural consistency, reduce context loss, and provide a structured development workflow for projects that evolve over months or years.

The workflow is technology-agnostic and can be used for AI platforms, backend systems, automation frameworks, DevOps tools, web applications, and other software engineering projects.

---

# Why This Repository Exists

Long-running ChatGPT conversations eventually become:

- Slow
- Repetitive
- Less accurate
- Inconsistent with earlier architectural decisions

This repository provides a structured workflow that keeps implementation conversations small while preserving the complete engineering history of a project.

The result is a development process that scales with the project instead of degrading over time.

---

# Workflow Overview

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

When the MASTER conversation becomes large:

```text
MASTER

↓

Project Continuation Plan

↓

MASTER v2

↓

Continue Development
```

---

# Repository Structure

```text
engineering-project-workflow-prompts/
│
├── prompts/
│   ├── 01-master-to-feature-branch.md
│   ├── 02-feature-branch-handoff.md
│   ├── 03-master-project-continuation.md
│   ├── 04-architecture-decision-review.md
│   ├── 05-engineering-health-review.md
│   ├── 06-release-readiness-review.md
│   ├── 07-resume-portfolio-interview.md
│   └── 08-engineering-learning-roadmap.md
│
├── examples/
│   ├── workflow-example.md
│   ├── branch-example.md
│   └── project-continuation-example.md
│
├── diagrams/
│   ├── workflow.png
│   └── lifecycle.png
│
├── LICENSE
├── .gitignore
└── README.md
```

---

# Prompt Library

| Prompt | Purpose |
|---------|---------|
| Prompt 1 | Start a new feature branch from the current Master conversation |
| Prompt 2 | Generate a complete engineering handoff after finishing a feature branch |
| Prompt 3 | Replace an oversized Master conversation with a new Project Continuation Plan |
| Prompt 4 | Review major architectural decisions before implementation |
| Prompt 5 | Evaluate engineering health, technical debt, and technology choices |
| Prompt 6 | Verify release readiness before publishing or merging major work |
| Prompt 7 | Translate project work into resume, portfolio, GitHub, and interview material |
| Prompt 8 | Review long-term learning priorities and future project roadmap |

---

# Recommended Workflow

```text
Create MASTER

↓

Create Feature Branch

↓

Prompt 1

↓

Development

↓

Prompt 2

↓

Update MASTER

↓

Repeat
```

Periodically:

```text
Prompt 4
Architecture Review

↓

Prompt 5
Engineering Health Review

↓

Prompt 6
Release Readiness

↓

Prompt 7
Resume & Portfolio Update

↓

Prompt 8
Learning & Roadmap Review
```

When the MASTER conversation becomes too large:

```text
Prompt 3

↓

Generate Project Continuation Plan

↓

Create MASTER v2

↓

Continue Development
```

---

# Benefits

- Structured long-term project management
- Consistent architecture across feature branches
- Reduced ChatGPT context loss
- Focused implementation conversations
- Better documentation of engineering decisions
- Reusable workflow for any software project
- Improved portfolio and interview preparation

---

# Suitable For

This workflow can be applied to projects such as:

- AI Platforms
- LLM Applications
- RAG Systems
- Automation Frameworks
- Playwright Projects
- Backend Services
- DevOps Tooling
- Enterprise Software
- Personal Portfolio Projects
- Open Source Projects

---

# Philosophy

The workflow is built around a few core principles:

- One MASTER conversation acts as the single source of truth.
- One Git feature branch corresponds to one implementation conversation.
- Every completed feature generates a structured engineering handoff.
- Large conversations are periodically replaced with a Project Continuation Plan.
- Architectural decisions are reviewed before implementation.
- Development prioritizes maintainability, scalability, and long-term evolution.

---

# License

This project is licensed under the MIT License.
