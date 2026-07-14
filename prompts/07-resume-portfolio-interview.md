# Prompt 7 — Resume, Portfolio & Interview Translation

## Purpose

Use this prompt after completing one or more major feature branches, before updating:

- Resume
- LinkedIn
- GitHub
- Portfolio
- Interview preparation
- Performance review
- Promotion documentation

The goal is to transform technical implementation into professional achievements without exaggeration or inventing work.

## When to Use
```
Feature Branch Completed
            │
            ▼
Merged into Master
            │
            ▼
Paste Prompt 7
            │
            ▼
Resume & Portfolio Translation
            │
            ▼
Update
• Resume
• LinkedIn
• GitHub
• Portfolio
• Interview Notes
```

---

# Prompt
```
Act as a Principal Software Engineer, Senior SDET Interviewer, Engineering Manager, Technical Recruiter, Resume Reviewer, and Hiring Panel Member.

Treat the current Project Continuation Plan as the authoritative source of truth.

Review the entire project rather than only recent feature branches.

Do not invent features, metrics, or business impact.

Describe only work that has actually been implemented and documented.

Whenever quantitative metrics are unavailable, describe achievements qualitatively instead of estimating numbers.

The objective is to translate engineering work into accurate, professional resume, portfolio, GitHub, and interview material suitable for senior AI testing and automation roles.

Think from the perspective of someone reviewing candidates for:

- Senior SDET
- Staff SDET
- AI Test Engineer
- AI QA Engineer
- Test Automation Architect
- AI Platform Engineer
- Software Development Engineer in Test
- Principal Automation Engineer

Use the following structure.

# Executive Summary

Provide a concise summary of the project.

Explain:

- what was built
- why it matters
- who would benefit
- why it is technically impressive

# Project Evolution

Summarize how the project evolved.

Include:

- Major milestones
- Important feature branches
- Architecture evolution
- Engineering maturity gained

Keep this concise.

The objective is to help explain the project's journey during interviews.

# Resume Translation

Generate resume bullet points grouped into:

- Architecture
- AI Engineering
- Automation
- Testing
- DevOps
- Developer Experience
- Software Quality
- Open Source Engineering

For every bullet:

- Start with a strong action verb.
- Mention technologies only when they add value.
- Avoid generic buzzwords.
- Avoid exaggerated claims.
- Keep each bullet suitable for a professional resume.

# ATS Keywords

Generate ATS keywords based only on technologies currently implemented in the repository.

Do not include technologies that are only planned for future development.

Group keywords by technical domain.

Generate important ATS keywords grouped by category.

Examples:

Programming

Frameworks

Testing

AI

LLMs

Vector Databases

Retrieval

Evaluation

Cloud

CI/CD

Architecture

Observability

DevOps

# LinkedIn Project Description

Write a professional LinkedIn project description.

Requirements:

- Technical
- Concise
- Human-written
- No motivational language
- No emojis
- No marketing exaggeration

# GitHub Project Description

Generate:

Short Description

Long Description

Key Features

Highlights

Technical Stack

Architecture Summary

Future Roadmap

Suitable for the GitHub repository homepage.

# Recruiter Summary

Generate a concise summary suitable for recruiters.

Requirements:

- 100–150 words
- Technical but easy to understand
- Focus on business value and engineering maturity
- Avoid implementation details

# Portfolio Summary

Write a portfolio description that explains:

- the engineering challenges solved
- architecture decisions
- technologies used
- AI testing capabilities
- scalability
- maintainability

Assume this is being reviewed by an engineering hiring manager.

# Interview Story

Create a complete interview story.

Include:

Situation

Problem

Constraints

Architecture

Implementation

Trade-offs

Challenges

Testing Strategy

Results

Lessons Learned

This should be suitable for answering:

"Tell me about your most impressive project."

# Interview Talking Points

Generate concise talking points for interviews.

Include:

- 2-minute explanation
- 5-minute explanation
- 10-minute deep dive

For each version:

- Key architecture
- Biggest challenge
- Biggest engineering decision
- Lessons learned

Do not script exact answers.

Provide structured talking points.

# Deep Technical Questions

Generate realistic interview questions based on the project.

Categorize by:

Architecture

Python

Playwright

AI

LLMs

RAG

Evaluation

Vector Databases

CI/CD

Testing Strategy

Performance

Security

Design Patterns

Configuration

For every question provide:

- expected senior-level answer outline
- common mistakes
- follow-up questions

# System Design Discussion

Generate discussion topics suitable for a System Design interview.

Examples:

Why this architecture?

How would it scale?

How would you support multiple providers?

How would you support multiple vector databases?

How would you deploy this?

How would you monitor it?

How would you test it?

# Leadership Discussion

Generate interview questions for Engineering Manager or Staff-level discussions.

Examples:

Architecture decisions

Trade-offs

Technical debt

Project prioritization

Code quality

Release management

Team collaboration

Explain what strong answers should include.

# Project Strengths

Identify the strongest aspects of the project.

Explain why they stand out.

# Evidence Matrix

For every major project claim identify the evidence supporting it.

Use the following format:

| Claim | Evidence |
|--------|----------|
| Example claim | Feature branch, architecture, tests, documentation |

Every important resume statement should be traceable to actual implementation.

Do not fabricate evidence.

# Current Weaknesses

Identify areas that still reduce interview impact.

Recommend future feature branches that would strengthen the portfolio.

Only recommend changes that provide meaningful long-term engineering value.

# Career Positioning

Based on the completed project, estimate which roles the project currently supports.

Examples:

Automation Engineer

Senior SDET

Lead SDET

AI QA Engineer

AI Test Engineer

Automation Architect

Platform Engineer

AI Platform Engineer

For each role explain:

- strengths
- gaps
- recommended future improvements

# Final Assessment

Provide scores (1–10) for:

Architecture

Code Quality

AI Engineering

Testing Strategy

Automation

Scalability

Maintainability

Documentation

Portfolio Value

Interview Readiness

Overall Engineering Maturity

Conclude with:

## Hiring Manager Assessment

State whether this project would strengthen a candidate's profile for:

- Senior SDET
- Staff SDET
- AI Test Engineer
- AI QA Engineer
- Automation Architect
- AI Platform Engineer

For each role include:

- Current readiness
- Biggest strengths
- Biggest remaining gap

Finish with:

## Highest ROI Next Feature Branches

Recommend the next feature branches that would provide the greatest improvement for:

- Resume
- Portfolio
- Interview performance

Rank them by expected impact.
```
