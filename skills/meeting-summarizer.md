# Meeting Summarizer

## Purpose

Summarize Teams meeting recordings into decisions, action items, and key discussion points.

## When to Use

- After important meetings (stakeholder reviews, planning sessions)
- Sharing meeting outcomes with absent team members
- Creating async-friendly meeting notes
- Extracting commitments and deadlines

## Required Inputs

- **Meeting transcript:** Pasted Teams transcript
- **Meeting context:** Type of meeting, attendees, purpose
- **Focus areas:** (Optional) Specific topics to highlight

## Output Format

Structured summary with:
- Key decisions
- Action items with owners
- Discussion highlights
- Follow-up questions
- Parking lot items

## Prompt

When asked to summarize a meeting, follow this approach:

```
Reference CLAUDE.md for:
- My stakeholders
- My current priorities
- My formatting preferences

Inputs provided:
- Meeting transcript: {transcript}
- Meeting context: {meeting_type_and_attendees}
- Focus areas: {specific_topics}

Generate meeting summary:

## Meeting Summary

**Meeting:** [Meeting name/type]
**Date:** [Date]
**Attendees:** [Names]
**Duration:** [Length]

---

## TL;DR

[2-3 sentences: What was decided? What's the next step?]

---

## Decisions Made

| Decision | Owner | Context |
|----------|-------|---------|
| [Decision 1] | [Who decided] | [Why/background] |
| [Decision 2] | [Who decided] | [Why/background] |

---

## Action Items

| Action | Owner | Due Date | Status |
|--------|-------|----------|--------|
| [Action 1] | @[Name] | [Date] | Open |
| [Action 2] | @[Name] | [Date] | Open |
| [Action 3] | @[Name] | [Date] | Open |

---

## Discussion Highlights

### [Topic 1]

**Context:** [What was discussed]

**Key points:**
- [Point 1]
- [Point 2]

**Outcome:** [Resolution or next step]

---

### [Topic 2]

[Same structure]

---

## Open Questions

1. [Question raised but not answered] - Follow up with: [Person]
2. [Question that needs research] - Owner: [Person]

---

## Parking Lot

*Items mentioned but deferred:*
- [Future topic 1]
- [Future topic 2]

---

## Next Meeting

**Scheduled:** [Date/time if mentioned]
**Agenda items:** [Any mentioned topics for next time]

---

*Summary generated from Teams recording. Reach out to [attendee names] for clarification.*
```

## Example Usage

**Input:**
> "Summarize this sprint planning meeting. Attendees: engineering lead, designer, and me. Focus on commitments and blockers. [paste transcript]"

**Output:**
Claude generates a structured summary with sprint commitments as action items, blockers discussed, and follow-up items.

## Tips for Meeting Summaries

- **Prioritize decisions:** What actually got decided?
- **Name owners explicitly:** Every action needs an owner
- **Include due dates:** Vague "soon" doesn't work
- **Note parking lot:** Don't lose deferred items
- **Keep it scannable:** Busy people skim

## Related Skills

- `stakeholder-comms.md` - Turn summary into stakeholder update
