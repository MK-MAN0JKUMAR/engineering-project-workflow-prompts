# Prompt 4 — Architecture Decision Review

## Purpose

Use this prompt before introducing a significant architectural change.

## Examples include:

- New framework
- New design pattern
- Major refactoring
- New AI framework
- New database
- New vector database
- New agent framework
- New provider
- New retrieval strategy
- New evaluation framework
- Large dependency
- Repository restructuring

The goal is to determine whether the proposed change is genuinely beneficial before implementing it.

## When to Use
```
MASTER
    │
    ├── Feature Branch
    │
    ├── New Architectural Idea
    │
    └── Paste Prompt 4
             │
             ▼
Architecture Decision Review
             │
             ▼
Decision

Accept
Reject
Postpone
Architecture Branch
```

---

# Prompt
```
We are considering a significant architectural change to the project.

Treat the current Project Continuation Plan as the authoritative source of truth.

Before recommending any implementation, first verify whether the proposed change can be achieved by extending the existing architecture.

Do not recommend a redesign simply because a new technology or pattern exists.

Challenge the proposal objectively.

Assume you are part of an Enterprise Architecture Review Board responsible for maintaining this platform for the next 5–10 years.

Prioritize long-term maintainability, architectural consistency, and production readiness over novelty.

If the proposal requires information from existing project files that has not been shared in the current conversation, request only the required files before making a recommendation.

Do not make architectural assumptions without reviewing the relevant implementation.

Review the proposal using the following framework.

# Proposed Change

Summarize the proposed architectural change.

Clearly define:

- what changes
- why it is being considered
- expected outcome

# Current Architecture

Describe how the project currently solves this problem.

Identify existing components that are already involved.

# Existing Implementation Review

Identify the existing implementation related to this proposal.

Determine:

- Which modules already solve part of this problem.
- Which files would likely change.
- Whether the existing implementation can be extended instead of replaced.
- Whether duplicate functionality would be introduced.

Recommend the smallest architectural change capable of solving the problem.

# Problem Analysis

Determine whether a real problem exists.

Explain:

- current limitation
- impact
- frequency
- severity

Avoid solving theoretical problems.

# Alternative Solutions

Identify simpler alternatives.

Examples:

- configuration changes
- extending existing components
- improving current abstractions
- plugin approach
- adapter pattern
- strategy pattern

Compare each option.

# Scope Classification

Determine whether this proposal belongs in:

- Current feature branch
- New feature branch
- Dedicated architecture branch
- Future roadmap
- Should not be implemented

Explain why.

# Architecture Impact

Explain how the proposal affects:

- modularity
- maintainability
- scalability
- observability
- performance
- testing
- deployment
- dependency graph
- developer experience

Include diagrams if useful.

# AI Engineering Impact

Explain how the proposal affects:

- provider abstraction
- model abstraction
- retrieval pipeline
- evaluation pipeline
- prompts
- agent workflows
- future AI frameworks

# Dependency Review

List any new dependencies.

For each dependency explain:

- purpose
- maturity
- maintenance risk
- community adoption
- alternatives

Prefer open-source solutions whenever practical.

# Breaking Changes

Identify:

- API changes
- configuration changes
- migration effort
- compatibility risks

Estimate migration complexity.

# Performance Analysis

Estimate impact on:

- indexing
- retrieval
- inference
- evaluation
- memory
- startup
- runtime latency

Identify expected improvements and regressions.

# Long-Term Maintainability

Estimate maintenance cost over the next several years.

Consider:

- readability
- complexity
- documentation
- onboarding
- debugging
- extensibility

# Portfolio Value

Explain whether this change strengthens the project for:

- Senior SDET interviews
- AI Engineer interviews
- System Design discussions
- Open-source portfolio

Avoid changes that add complexity without meaningful value.

# Recommendation

Choose exactly one recommendation.

- Approve for the current feature branch
- Approve as a new feature branch
- Approve as a dedicated architecture branch
- Postpone to the roadmap
- Reject

Explain:

- Why this recommendation was chosen.
- Why the other options were rejected.
- What conditions would change the recommendation in the future.

# Implementation Strategy

If implementation is recommended:

Provide the safest migration strategy.

Divide the work into logical Git feature branches.

Estimate:

- implementation difficulty
- testing effort
- migration risk

# Risks

List technical risks.

List business risks.

List future maintenance risks.

# Repository Impact

Summarize how this proposal would affect the repository.

Include:

- Major files expected to be added
- Major files expected to be modified
- New dependencies (if any)
- Documentation updates
- Testing impact
- CI/CD impact
- Estimated implementation size

Keep this summary concise.

# Final Decision

Summarize:

- Should we do it?
- Why?
- Expected value
- Trade-offs
- Recommended next action

The final recommendation should prioritize long-term architectural quality over short-term implementation convenience.
```
