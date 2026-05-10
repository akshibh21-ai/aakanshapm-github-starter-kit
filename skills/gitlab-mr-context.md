# GitLab MR Context

## Purpose

Add PM context to GitLab merge requests: why the change matters, customer impact, and rollout considerations.

## When to Use

- Before MR merge for significant features
- When engineering requests PM context
- For MRs that affect customer-facing behavior
- Agentic spec kit changes that need business context

## Required Inputs

- **MR context:** MR link or description of changes
- **Feature context:** What feature/initiative this supports
- **Customer impact:** Who's affected and how

## Output Format

MR comment with:
- PM context summary
- Customer impact
- Rollout considerations
- Related links

## Prompt

When asked to add PM context to a GitLab MR, follow this approach:

```
Reference CLAUDE.md for:
- My product area
- My role context
- My formatting preferences

Inputs provided:
- MR context: {mr_description}
- Feature context: {feature_name}
- Customer impact: {impact_details}

Generate MR context comment:

---

## PM Context

### Why This Change

[2-3 sentences: What problem does this solve? Why are we doing this now?]

### Customer Impact

| Aspect | Details |
|--------|---------|
| **Who's affected** | [User segment or customer type] |
| **What changes** | [Behavior change from user perspective] |
| **Expected outcome** | [Benefit to customers] |

### Business Context

- **Initiative:** [Parent feature or initiative]
- **Priority:** [Why this is prioritized now]
- **Success metric:** [How we'll measure success]

---

## Rollout Considerations

### Feature Flag
- [ ] Behind feature flag: [Flag name]
- [ ] Gradual rollout planned: [Percentage/timeline]

### Communication
- [ ] Customer docs needed: [Yes/No - link if yes]
- [ ] Internal announcement: [Yes/No]
- [ ] Customer notification: [Yes/No]

### Risks
| Risk | Mitigation |
|------|------------|
| [Risk 1] | [How we'll handle it] |

---

## Related Links

- **AHA! Feature:** [Link]
- **PRD:** [Confluence link]
- **Design:** [Figma link]
- **Spec:** [Confluence link]

---

/cc @[stakeholder] for awareness
```

## Example Usage

**Input:**
> "Add PM context to the MR for bulk connector validation. It's part of the bulk import feature, affects data engineers, and should reduce setup errors by 50%."

**Output:**
Claude generates a structured MR comment with customer impact, rollout considerations, and related links.

## When to Add Context

**Always add for:**
- Customer-facing behavior changes
- New features or capabilities
- Breaking changes or deprecations
- Performance-significant changes

**Skip for:**
- Internal refactoring with no behavior change
- Bug fixes with obvious impact
- Documentation-only changes

## Related Skills

- `stakeholder-comms.md` - For broader announcements about shipped features
- `spec-reviewer.md` - Review the spec this MR implements
