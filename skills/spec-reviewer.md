# Spec Reviewer

## Purpose

Review technical specs for completeness, clarity, and PM concerns before sign-off.

## When to Use

- Before approving a technical spec in Confluence
- During spec review meetings
- When engineering asks for PM sign-off
- Validating alignment between PRD and technical approach

## Required Inputs

- **Spec content:** Pasted spec or key sections
- **PRD context:** (Optional) Related PRD or requirements
- **Review focus:** Full review, or specific concerns

## Output Format

Structured review with:
- Summary assessment
- Gaps and missing elements
- Questions for engineering
- Risk flags
- Approval recommendation

## Prompt

When asked to review a spec, follow this approach:

```
Reference CLAUDE.md for:
- My product area context
- My stakeholders
- My documentation standards

Inputs provided:
- Spec content: {spec_content}
- PRD context: {prd_or_requirements}
- Review focus: {specific_concerns}

Generate spec review:

## Review Summary

**Spec:** [Spec name]
**Reviewer:** [Your name]
**Date:** [Date]
**Verdict:** Ready / Needs revision / Major gaps

---

## Checklist

### Problem & Goals
- [ ] Problem statement is clear
- [ ] Goals align with PRD
- [ ] Success metrics are defined and measurable
- [ ] Target users are identified

### Solution Design
- [ ] Approach is clearly explained
- [ ] Key components/systems are identified
- [ ] Data flow is documented
- [ ] API contracts are defined (if applicable)

### Edge Cases & Errors
- [ ] Edge cases are documented
- [ ] Error handling is specified
- [ ] Empty/null states are covered
- [ ] Concurrent access is considered

### Operations
- [ ] Rollback plan exists
- [ ] Monitoring/alerting is defined
- [ ] Performance requirements are stated
- [ ] Security considerations are addressed

### Dependencies
- [ ] External dependencies are listed
- [ ] Team dependencies are identified
- [ ] Timeline dependencies are clear

---

## Gaps & Missing Elements

| Gap | Severity | Recommendation |
|-----|----------|----------------|
| [Missing element] | High/Medium/Low | [What to add] |

---

## Questions for Engineering

1. **[Question about approach]** - Needed to understand [why]
2. **[Question about edge case]** - Risk: [what could go wrong]
3. **[Question about timeline]** - Dependency on [what]

---

## Risk Flags

| Risk | Likelihood | Impact | Mitigation |
|------|------------|--------|------------|
| [Risk] | High/Med/Low | High/Med/Low | [Suggested mitigation] |

---

## Recommendation

**Approve / Request Changes / Escalate**

**Reasoning:** [1-2 sentences on the key issue or why it's ready]

**Next step:** [Specific action]
```

## Example Usage

**Input:**
> "Review this Confluence spec for the bulk connector import feature: [paste spec content]"

**Output:**
Claude generates a structured review with checklist, gaps table, questions for engineering, and approval recommendation.

## What to Look For

**Red flags:**
- No success metrics
- Missing rollback plan
- Vague error handling ("handle errors gracefully")
- No consideration of scale/performance
- Dependencies not called out

**Good signs:**
- Clear problem statement
- Defined API contracts
- Explicit out-of-scope items
- Performance targets with numbers

## Related Skills

- `prd-writer.md` - The PRD this spec should align with
- `aha-ticket-manager.md` - Create tickets after spec approval
