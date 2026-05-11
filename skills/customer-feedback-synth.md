# Customer Feedback Synthesis

## Purpose

Synthesize feedback from AHA! Ideas Portal into actionable themes, patterns, and priorities.

## When to Use

- Preparing for prioritization planning
- Building customer evidence for PRDs
- Quarterly roadmap planning
- Understanding customer sentiment on a feature area

## Required Inputs

- **Feedback data:** Exported Ideas Portal data or pasted feedback
- **Focus area:** (Optional) Specific product area to analyze
- **Time range:** (Optional) Recent vs. all-time feedback

## Output Format

Synthesis report with:
- Theme clusters
- Top requests ranked
- Sentiment patterns
- Customer segments
- Recommendations

## Prompt

When asked to synthesize customer feedback, follow this approach:

```
Reference CLAUDE.md for:
- My product area
- My current priorities (from GOALS.md)
- My formatting preferences

Inputs provided:
- Feedback data: {feedback_content}
- Focus area: {product_area}
- Time range: {time_range}

Generate feedback synthesis:

## Customer Feedback Synthesis

**Source:** AHA! Ideas Portal
**Date range:** [Time range]
**Focus area:** [Product area or "All"]
**Total ideas analyzed:** [Count]

---

## Executive Summary

[3-4 sentences: Key takeaway, biggest theme, and recommended action]

---

## Theme Clusters

### Theme 1: [Theme Name] (X ideas, Y votes)

**Pattern:** [What customers are asking for]

**Representative quotes:**
> "[Direct customer quote]"
> "[Direct customer quote]"

**Customer segments:** [Who's asking - enterprise, SMB, specific industries]

**Implication:** [What this means for the product]

---

### Theme 2: [Theme Name] (X ideas, Y votes)

[Same structure]

---

### Theme 3: [Theme Name] (X ideas, Y votes)

[Same structure]

---

## Top Requests (Ranked)

| Rank | Request | Votes | Customers | Effort Est. | Impact |
|------|---------|-------|-----------|-------------|--------|
| 1 | [Request] | [#] | [Segments] | S/M/L | High/Med/Low |
| 2 | [Request] | [#] | [Segments] | S/M/L | High/Med/Low |
| 3 | [Request] | [#] | [Segments] | S/M/L | High/Med/Low |

---

## Sentiment Patterns

| Sentiment | % of Feedback | Key Driver |
|-----------|---------------|------------|
| Positive | [%] | [What's working] |
| Neutral | [%] | [Feature requests] |
| Negative | [%] | [Pain points] |

**Trend:** [Improving / Stable / Declining]

---

## Customer Segments

| Segment | Top Ask | Volume |
|---------|---------|--------|
| Enterprise | [Request] | [#] ideas |
| SMB | [Request] | [#] ideas |
| [Industry] | [Request] | [#] ideas |

---

## Recommendations

### Prioritize Now
- [Recommendation 1] - Why: [customer evidence]

### Investigate Further
- [Recommendation 2] - Why: [need more data on]

### Deprioritize
- [Recommendation 3] - Why: [low volume, niche request]

---

## Raw Data Summary

Save to: `context/ideas-portal/feedback-themes-[date].md`
```

## Example Usage

**Input:**
> "Synthesize the last quarter's Ideas Portal feedback for the connector product area. Here's the export: [paste data]"

**Output:**
Claude generates a themed synthesis with top requests, customer segments, and prioritization recommendations.

## Tips for Ideas Portal Analysis

- **Look for vote patterns:** High votes = broad demand
- **Check customer segments:** Enterprise vs SMB priorities differ
- **Watch for trends:** New themes vs. recurring asks
- **Quote customers:** Direct quotes are powerful in PRDs

## Related Skills

- `prd-writer.md` - Use synthesis as customer evidence in PRDs
- `aha-ticket-manager.md` - Create features from top requests
