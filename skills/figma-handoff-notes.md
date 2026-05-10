# Figma Handoff Notes

## Purpose

Generate developer handoff documentation from Figma designs, covering states, interactions, and edge cases.

## When to Use

- Design is finalized and ready for engineering
- Preparing for design-to-dev handoff meeting
- Documenting interaction specifications
- Clarifying design details for remote/async teams

## Required Inputs

- **Design context:** Figma link, screenshots description, or pasted design notes
- **Feature context:** What feature this design supports
- **Interaction notes:** Any specific behaviors, animations, or states

## Output Format

Structured handoff document with:
- Screen overview
- Component states
- Interaction specifications
- Edge cases and empty states
- Responsive behavior
- Questions for design

## Prompt

When asked to create Figma handoff notes, follow this approach:

```
Reference CLAUDE.md for:
- My product area
- My team context (engineering, design)
- My formatting preferences

Inputs provided:
- Design context: {figma_link_or_description}
- Feature context: {feature_name}
- Interaction notes: {interaction_details}

Generate handoff documentation:

## Figma Handoff: [Feature Name]

**Figma Link:** [Link]
**Designer:** [Name]
**Date:** [Date]
**Status:** Ready for dev / In progress

---

## Screen Overview

[1-2 sentence description of what this screen/component does]

### Key Components
| Component | Purpose |
|-----------|---------|
| [Component 1] | [What it does] |
| [Component 2] | [What it does] |

---

## Component States

### [Component Name]

| State | Description | Visual |
|-------|-------------|--------|
| Default | [Description] | [How it looks] |
| Hover | [Description] | [Changes on hover] |
| Active/Pressed | [Description] | [Click feedback] |
| Disabled | [Description] | [Greyed out behavior] |
| Loading | [Description] | [Loading indicator] |
| Error | [Description] | [Error appearance] |

---

## Interaction Specifications

### [Interaction 1: e.g., "Submit Form"]
- **Trigger:** [User action]
- **Behavior:** [What happens]
- **Feedback:** [Visual/audio feedback]
- **Duration:** [Animation timing if applicable]

### [Interaction 2: e.g., "Expand Panel"]
- **Trigger:** [User action]
- **Behavior:** [What happens]
- **Animation:** [Easing, duration]

---

## Edge Cases & Empty States

| Scenario | Design | Notes |
|----------|--------|-------|
| No data / Empty | [Description] | [CTA or message] |
| Too much data / Overflow | [Description] | [Truncation, scroll] |
| Error state | [Description] | [Error message, retry] |
| Offline | [Description] | [If applicable] |
| First-time user | [Description] | [Onboarding, tooltips] |

---

## Responsive Behavior

| Breakpoint | Changes |
|------------|---------|
| Desktop (>1024px) | [Default layout] |
| Tablet (768-1024px) | [Layout changes] |
| Mobile (<768px) | [Mobile-specific changes] |

---

## Accessibility Notes

- [ ] Color contrast meets WCAG AA
- [ ] Interactive elements are keyboard accessible
- [ ] Screen reader labels defined
- [ ] Focus states are visible

---

## Questions for Design

1. [Question about ambiguous behavior]
2. [Question about missing state]

---

## Implementation Notes

[Any specific notes for engineering: libraries to use, existing components to reference, etc.]
```

## Example Usage

**Input:**
> "Create handoff notes for the new connector setup wizard. It's a 3-step flow with validation on each step. Figma link: [link]"

**Output:**
Claude generates structured handoff docs covering each step's states, validation behaviors, error handling, and responsive behavior.

## Related Skills

- `prd-writer.md` - The PRD this design implements
- `spec-reviewer.md` - The technical spec for this feature
