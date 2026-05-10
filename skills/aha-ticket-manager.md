# AHA! Ticket Manager

## Purpose

Create, update, and organize AHA! features and requirements from specs, conversations, or PRDs.

## When to Use

- Creating a new master feature or feature in AHA!
- Breaking down a PRD into AHA! requirements
- Updating feature status or details
- Organizing features on the prioritization board

## Required Inputs

- **Feature context:** Description of what needs to be built
- **Priority context:** Business value, customer demand, effort estimate
- **Release target:** (Optional) Target release or timeframe
- **Related items:** Links to Confluence specs, Figma designs, or parent features

## Output Format

AHA!-ready feature content with:
- Feature name (concise, action-oriented)
- Description (problem + solution)
- Acceptance criteria
- Priority recommendation
- Dependencies

## Prompt

When asked to create or update AHA! features, follow this approach:

```
Reference CLAUDE.md for:
- My product area and current focus
- My team context and stakeholders
- My formatting preferences

Inputs provided:
- Feature context: {feature_description}
- Priority context: {business_value_and_effort}
- Release target: {target_release}
- Related items: {links_or_context}

Generate AHA! feature content:

## Feature Name
[Action-oriented name: "Enable bulk connector import"]

## Description

### Problem
[2-3 sentences: What pain point does this solve?]

### Solution
[2-3 sentences: What are we building to solve it?]

### Customer Impact
[Who benefits? How much?]

## Acceptance Criteria
- [ ] [Specific, testable criterion]
- [ ] [Specific, testable criterion]
- [ ] [Specific, testable criterion]
- [ ] [Edge case or error handling]

## Priority Recommendation

| Factor | Assessment |
|--------|------------|
| Customer demand | High / Medium / Low |
| Business value | High / Medium / Low |
| Effort estimate | S / M / L / XL |
| Dependencies | [List any blockers] |

**Recommended priority:** [Must-have / Should-have / Nice-to-have]
**Reasoning:** [1 sentence why]

## Dependencies
- **Upstream:** [What needs to happen first]
- **Downstream:** [What depends on this]

## Related Items
- Parent feature: [If applicable]
- Confluence spec: [Link]
- Figma design: [Link]

## Release Target
[Target release or date]
```

## Example Usage

**Input:**
> "Create an AHA! feature for the bulk import capability from the PRD. High customer demand, medium engineering effort, target Q3."

**Output:**
Claude generates AHA!-ready feature content with name, description, acceptance criteria, and priority recommendation.

## Tips for AHA!

- **Naming convention:** Start with a verb (Enable, Add, Improve, Fix)
- **Acceptance criteria:** Write as testable checkboxes
- **Dependencies:** Be explicit about blockers
- **Linking:** Always link to source Confluence spec

## Related Skills

- `prd-writer.md` - Generate the PRD first
- `spec-reviewer.md` - Review technical spec before creating tickets
