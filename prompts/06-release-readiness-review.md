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

Treat the current Project Continuation Plan as the authoritative source of truth.

Review the entire project rather than only recent feature branches.

Assume this version is being evaluated as an official project release.

Think like an Enterprise Release Review Board responsible for approving production-quality software.

Base every recommendation on the current implementation and documented project state.

If implementation details are required and the relevant files have not been shared, request only the required files before making conclusions.

Do not recommend new features simply because they would be nice to have.

Evaluate only whether the planned release scope has been completed successfully.

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

# Release Scope Verification

Review the planned release scope.

Determine:

- Planned features
- Completed features
- Deferred features
- Removed features
- Unexpected additions

Explain whether the implemented scope matches the original release objective.

Do not penalize intentionally deferred work.

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

# Developer Experience Review

Review whether a new developer could successfully contribute.

Evaluate:

- onboarding
- setup instructions
- local development workflow
- troubleshooting
- command documentation
- repository discoverability

Estimate onboarding difficulty.

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

# Repository Governance Review

Verify:

- Branch protection rules
- GitHub Actions
- CODEOWNERS
- Pull request templates
- Issue templates
- Labels
- Releases
- Tags
- License
- Security policy

Recommend improvements only if they affect release quality.

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

Release Blockers

High Priority

Medium Priority

Low Priority

Future Roadmap

For every item include:

- Description
- Why it remains
- Recommended feature branch
- Required before next release? (Yes/No)

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

Finish with a Release Scorecard.

Provide scores (1–10) for:

- Architecture
- Code Quality
- Testing
- Documentation
- Security
- Performance
- Maintainability
- Developer Experience
- Portfolio Value
- Release Readiness

Then conclude with:

## Next Milestone Recommendation

Include:

- Current Release Status
- Next Recommended Version
- Highest Priority Feature Branch
- Estimated Repository Maturity
- Overall Project Health
```
