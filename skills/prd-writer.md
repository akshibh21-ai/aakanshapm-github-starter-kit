# PRD Writer

## Purpose

Generate Product Requirements Documents from rough context, customer insights, and feature ideas.

## When to Use

- Starting a new feature or initiative
- Converting customer feedback into a formal requirement
- Documenting a feature before engineering kickoff

## Required Inputs

- **Problem statement:** What problem are we solving? Who has it?
- **Customer context:** Who are the users? What's their current pain?
- **Rough solution idea:** (Optional) Initial direction if you have one
- **Related context:** Links to AHA! features, Confluence specs, or Figma designs

## Output Format

Structured PRD with these sections:
1. Problem Statement
2. Target Users
3. Goals & Success Metrics
4. Proposed Solution
5. User Stories
6. Out of Scope
7. Open Questions
8. Dependencies

## Prompt

When asked to write a PRD, follow this approach:

```
Reference CLAUDE.md for:
- My role and product area
- My stakeholders and team context
- My formatting preferences

Inputs provided:
- Problem: {problem_statement}
- Customer context: {customer_context}
- Solution direction: {rough_solution}
- Related context: {links_or_pasted_content}

Generate a PRD with:

## Problem Statement
[2-3 sentences: What's broken? Who feels the pain? Why now?]

## Target Users
[Describe the primary user persona and their context]

## Goals & Success Metrics
- **Primary goal:** [One sentence]
- **Success metrics:**
  - [Metric 1 with target]
  - [Metric 2 with target]

## Proposed Solution
[High-level description of what we're building. Focus on WHAT, not HOW.]

### Key Capabilities
- [Capability 1]
- [Capability 2]
- [Capability 3]

## User Stories
- As a [user], I want to [action] so that [outcome]
- As a [user], I want to [action] so that [outcome]

## Out of Scope
- [What we're explicitly NOT doing]
- [Future considerations]

## Open Questions
1. [Question needing input from engineering/design/stakeholders]
2. [Question about edge cases or constraints]

## Dependencies
- [Technical dependency]
- [Team/resource dependency]
- [External dependency]
```

## Example Usage

**Input:**
> "Write a PRD for a bulk connector import feature. Customers are asking to import multiple connectors at once instead of one-by-one. Main users are data engineers setting up new environments."

**Output:**
Claude generates a structured PRD with problem statement, success metrics (e.g., "Reduce connector setup time by 80%"), proposed solution, and user stories.

## Related Skills

- `spec-reviewer.md` - Review the technical spec that follows
- `aha-ticket-manager.md` - Create AHA! feature from this PRD
