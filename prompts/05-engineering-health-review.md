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

Treat the current Project Continuation Plan as the authoritative source of truth.

Evaluate the project based on its current implementation rather than theoretical future designs.

Do not recommend redesigns simply because newer technologies exist.

Recommend architectural changes only when there is measurable long-term value.

Think like a Principal Software Architect conducting a formal engineering health review after several months of development.

Whenever implementation details are required to support a recommendation and the relevant files have not been shared, request only the necessary files before making conclusions.

The objective is to determine whether the project remains healthy, maintainable, scalable, and aligned with enterprise engineering practices.

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

# Repository Evolution Review

Review how the repository has evolved since the previous Engineering Health Review.

Summarize:

- Feature branches completed
- Architectural growth
- Repository growth
- Dependency growth
- Documentation growth

Identify whether the project is evolving in a consistent direction or showing signs of architectural drift.

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

# Technology Adoption Review

Review technologies that have been introduced since the last Engineering Health Review.

For each technology determine:

- Is it actively being used?
- Is it providing measurable value?
- Has it increased unnecessary complexity?
- Should it remain part of the project?

Do not recommend removing technologies without strong engineering justification.

# AI Ecosystem Review

Review significant developments in the AI ecosystem since the previous Engineering Health Review.

Recommend adoption only when a technology provides measurable improvements for this project.

For every recommendation include:

- Current limitation addressed
- Expected engineering value
- Migration effort
- Compatibility with existing architecture
- Recommended priority

Do not recommend technologies based solely on popularity or release date.

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

# Repository Governance Review

Review whether repository governance remains appropriate.

Evaluate:

- Branch strategy
- Branch protection rules
- CI/CD workflows
- Pull request templates
- Issue templates
- CODEOWNERS
- Documentation standards

Recommend updates only when they improve long-term maintainability.

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

If no major architectural work is required, explicitly recommend continuing feature development instead of redesigning the platform.

Conclude with:

## Health Review Summary

Include:

- Overall Health Rating
- Highest Priority Improvement
- Architectural Stability
- Technical Debt Trend
- Repository Maturity
- Recommended Next Review (for example, after 5–10 additional feature branches or before the next major release)
```
