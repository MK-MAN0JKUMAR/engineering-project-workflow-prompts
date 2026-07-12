# Prompt 6 — Release Readiness Review

## Purpose

### Use this prompt before:

- Creating a GitHub release
- Merging a major feature into main
- Updating your portfolio
- Recording a demo
- Writing a project article
- Sharing the project in interviews
- Declaring a milestone complete (v0.5, v1.0, v2.0, etc.)

The goal is to verify that the project is production-quality and identify anything that should be completed before calling the release "done."

## When to Use
```
Feature Branches Completed
            │
            ▼
Merge into Main
            │
            ▼
Release Candidate
            │
            ▼
Paste Prompt 6
            │
            ▼
Release Readiness Review
            │
     ┌──────┴──────┐
     │             │
 READY         NOT READY
     │             │
     ▼             ▼
Git Tag      Fix Remaining Issues
GitHub Release
Portfolio Update
Interview Demo
```

---

# Prompt
```
Perform a complete Release Readiness Review for this project.

Assume this version is planned to become an official project release (for example v0.5, v1.0 or v2.0).

Review the entire current project state using the Project Continuation Plan as the single source of truth.

Do not review only recent work.

Think like a Principal Engineer responsible for approving a production release.

The objective is to determine whether this release is ready for:

- GitHub
- Portfolio
- Interview Demonstrations
- Technical Blogs
- Internal Team Adoption

Do not include implementation code.

Use the following structure.

# Release Summary

Include:

- Project name
- Planned version
- Release objective
- Major capabilities introduced
- Overall maturity

# Executive Assessment

State one of the following:

READY

READY WITH MINOR FIXES

NOT READY

Explain the reasoning.

# Feature Completion Review

Review every major feature.

For each feature include:

- Complete
- Partial
- Missing
- Experimental
- Deferred

Explain why.

# Functional Verification

Review whether the following are working correctly.

- Document Loading
- Chunking
- Embedding
- Vector Database
- Retrieval
- Hybrid Retrieval
- Parent Retrieval
- Metadata Filtering
- Prompt Pipeline
- LLM Providers
- Evaluation
- Reporting
- UI
- Configuration
- Logging

Identify incomplete functionality.

# Architecture Review

Verify that:

- architecture is consistent
- responsibilities are clear
- abstractions are justified
- no unnecessary duplication exists
- dependency graph is healthy

Identify architectural risks.

# Code Quality Review

Review:

- readability
- maintainability
- consistency
- naming
- modularity
- configuration-first approach
- error handling

Identify weak areas.

# Testing Review

Evaluate:

- Unit Testing
- Integration Testing
- End-to-End Testing
- AI Evaluation
- Regression Testing
- Manual Validation

For each include:

- current coverage
- confidence level
- remaining gaps

# Performance Review

Evaluate:

- indexing speed
- retrieval latency
- reranking latency
- inference latency
- evaluation latency
- memory usage
- startup time

Identify regressions.

# Security Review

Review:

- API key handling
- environment variables
- dependency security
- prompt injection protection
- document safety
- logging safety

Recommend improvements.

# Documentation Review

Verify the existence and quality of:

- README
- setup guide
- architecture documentation
- configuration guide
- contribution guide
- troubleshooting guide
- changelog

Identify missing documentation.

# Dependency Review

Review all major dependencies.

For each determine:

- actively maintained
- production ready
- experimental
- should be replaced
- acceptable for release

Explain concerns.

# GitHub Readiness

Verify whether the repository is ready for public release.

Review:

- folder organization
- commit quality
- branch cleanliness
- ignored files
- secrets
- licensing
- badges
- issue templates
- pull request template

Recommend improvements.

# Portfolio Readiness

Review whether this release demonstrates:

- enterprise architecture
- AI engineering
- testing strategy
- scalability
- maintainability
- software craftsmanship

Estimate interview impact.

# Interview Readiness

Review whether this version provides strong discussion material for:

- Senior SDET
- Staff SDET
- AI Test Engineer
- Automation Architect

List strengths.

List weak areas.

# Remaining Work

Categorize remaining work into:

Critical

Important

Optional

Future

Explain why.

# Release Checklist

Generate a checklist.

Examples:

[ ] All planned features complete

[ ] Tests passing

[ ] Documentation updated

[ ] Configuration verified

[ ] Dependencies reviewed

[ ] No known blockers

[ ] Performance acceptable

[ ] Security reviewed

[ ] Reports validated

[ ] Portfolio screenshots updated

[ ] README updated

[ ] GitHub cleaned

Mark each item as:

Complete

Incomplete

Not Applicable

# Final Recommendation

Choose exactly one.

APPROVE RELEASE

APPROVE AFTER MINOR FIXES

REJECT RELEASE

Explain the reasoning.

If the release is rejected, provide a prioritized list of actions required before approval.

Finish with an overall Release Quality Score from 1–10 for:

- Architecture
- Code Quality
- Testing
- AI Engineering
- Documentation
- Performance
- Security
- Maintainability
- Portfolio Value
- Overall Release Readiness
```
