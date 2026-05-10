# Stakeholder Communications

## Purpose

Draft status updates, escalation emails, and stakeholder presentations that communicate effectively.

## When to Use

- Weekly/monthly status updates
- Escalating blockers to leadership
- Preparing for stakeholder reviews
- Summarizing project status for executives

## Required Inputs

- **Update type:** Status update, escalation, announcement, or review prep
- **Audience:** Who's receiving this (exec, team, cross-functional)
- **Key points:** What happened, what's blocked, what's next
- **Tone:** Informational, urgent, celebratory

## Output Format

Structured communication with:
- Executive summary (2-3 bullets)
- Key updates by category
- Blockers/risks with asks
- Next steps

## Prompt

When asked to draft stakeholder comms, follow this approach:

```
Reference CLAUDE.md for:
- My stakeholders and their context
- My communication preferences
- My formatting preferences

Inputs provided:
- Update type: {type}
- Audience: {audience}
- Key points: {points}
- Tone: {tone}

Generate stakeholder communication:

---

## [Status Update / Escalation / Announcement]

**Date:** [Date]
**From:** [Your name]
**To:** [Audience]

### TL;DR
- [Key outcome or decision - 1 line]
- [Most important update - 1 line]
- [Blocker or ask if any - 1 line]

---

### Progress This [Week/Sprint/Month]

**Shipped:**
- [What was completed with impact]
- [What was completed with impact]

**In Progress:**
- [What's actively being worked on] - ETA: [Date]
- [What's actively being worked on] - ETA: [Date]

---

### Blockers & Risks

| Blocker | Impact | Ask |
|---------|--------|-----|
| [Blocker] | [What happens if not resolved] | [Specific request] |

**Risk to flag:** [Any emerging risk with mitigation plan]

---

### Next Steps
1. [Action] - Owner: [Name] - Due: [Date]
2. [Action] - Owner: [Name] - Due: [Date]

---

### Metrics Snapshot (if applicable)
| Metric | Target | Actual | Trend |
|--------|--------|--------|-------|
| [Metric] | [Target] | [Actual] | Up/Down/Flat |

---
```

## Example Usage

**Input:**
> "Write a weekly update for my engineering lead. We shipped the connector validation feature, bulk import is blocked on API changes, and we're on track for Q3 release."

**Output:**
Claude generates a structured update with TL;DR, progress, blockers table, and next steps.

## Communication Tips

- **Lead with outcomes:** What changed, not what you did
- **Be specific on asks:** "Need API changes by Friday" not "need help"
- **Right-size detail:** Execs want 3 bullets, team wants full context
- **Include the "so what":** Why does this matter to the reader?

## Templates

See also:
- `/templates/stakeholder-update.md` - Reusable template
- `/templates/release-notes.md` - Customer-facing announcements

## Related Skills

- `meeting-summarizer.md` - Summarize meetings for async stakeholders
