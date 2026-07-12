# Prompt 5 — Engineering Health & Technology Review

## Purpose

Use this prompt periodically to evaluate the long-term health of the project.

### Recommended frequency:

- Every 3–6 months
- After completing approximately 5–10 feature branches
- Before a major release
- Before a large architectural expansion
Whenever the AI ecosystem has changed significantly

The goal is not to redesign the project.

The goal is to identify improvements that genuinely increase the project's long-term quality while avoiding unnecessary complexity.

## When to Use
```
MASTER
    │
    ├── Feature Branch
    ├── Feature Branch
    ├── Feature Branch
    ├── Feature Branch
    ├── Feature Branch
    │
    └── Paste Prompt 5
             │
             ▼
Engineering Health Review
             │
             ▼
Improvement Roadmap
             │
             ▼
Prioritize Future Branches
```

---

# Prompt
```
Perform a complete Engineering Health & Technology Review of this project.

Assume this project is intended to remain production-quality and evolve continuously for many years.

The current Project Continuation Plan is the single source of truth.

Do not recommend redesigns simply because newer technologies exist.

Only recommend changes that provide meaningful long-term engineering value.

Think like a Principal Software Architect reviewing the platform after several months of development.

The objective is to determine whether the project is still healthy, maintainable, and aligned with current engineering best practices.

Use the following structure.

# Executive Summary

Provide an overall assessment of the project.

Rate:

- Architecture
- Maintainability
- Scalability
- AI Engineering
- Testing Strategy
- Code Organization
- Documentation
- Portfolio Value

Give an overall health score from 1–10.

# Architecture Health

Review:

- module organization
- dependency graph
- abstraction quality
- coupling
- cohesion
- extensibility

Identify unnecessary complexity.

Highlight opportunities to simplify.

# Code Quality

Review:

- duplicated logic
- inconsistent patterns
- naming consistency
- configuration management
- readability
- maintainability

Identify areas needing refactoring.

# Technical Debt

Categorize:

High

Medium

Low

For every item explain:

- why it exists
- impact
- recommended branch
- urgency

# Performance Review

Review:

- indexing
- retrieval
- reranking
- inference
- evaluation
- reporting
- startup time
- runtime memory

Identify bottlenecks.

Estimate future scaling concerns.

# Dependency Review

Review every major dependency.

For each dependency explain:

- still appropriate?
- actively maintained?
- production ready?
- should be replaced?
- migration risk

Do not recommend replacing dependencies without strong engineering justification.

# AI Ecosystem Review

Review whether newer technologies provide meaningful value.

Examples:

- LangChain
- LangGraph
- MCP
- OpenAI Agents SDK
- DSPy
- CrewAI
- Haystack
- LlamaIndex
- AutoGen
- new evaluation frameworks
- new rerankers
- new vector databases

For every recommendation explain:

- why
- expected value
- migration effort
- urgency

Do not recommend adoption simply because the technology is newer.

# Security Review

Evaluate:

- secrets management
- API keys
- configuration
- dependency security
- prompt injection protection
- retrieval safety
- evaluation safety

Recommend improvements.

# Testing Review

Review:

- unit tests
- integration tests
- evaluation coverage
- regression testing
- UI testing
- API testing
- AI evaluation coverage

Identify missing testing areas.

# Documentation Review

Evaluate:

- README
- architecture documentation
- setup guides
- ADRs
- diagrams
- developer onboarding

Recommend improvements.

# Portfolio Review

Review the project from the perspective of:

- Senior SDET interview
- AI Test Engineer interview
- Principal SDET interview
- Open-source portfolio

Identify strengths.

Identify missing enterprise capabilities.

# Future Readiness

Determine whether the architecture can easily support:

- additional providers
- additional models
- agent workflows
- multimodal AI
- voice
- vision
- new evaluation frameworks
- new retrieval techniques
- distributed deployment

Estimate readiness.

# Engineering Scorecard

Provide scores (1–10) for:

Architecture

Maintainability

Scalability

Performance

Testing

Documentation

AI Engineering

Security

Configuration

Developer Experience

Portfolio Value

Overall Project Health

# Improvement Roadmap

Categorize recommendations into:

Immediate

Next Quarter

Future

Optional

For every recommendation include:

- expected value
- implementation complexity
- interview value
- portfolio value
- business value

Prioritize only meaningful improvements.

# Final Recommendation

Conclude with one of the following:

Excellent

Healthy

Needs Improvement

Major Refactoring Required

Explain why.

If no major architectural work is needed, explicitly recommend continuing feature development instead of redesigning the platform.
```
