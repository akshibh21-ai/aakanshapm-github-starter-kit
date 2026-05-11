# Weekly Review Workflow

## Purpose

End-of-week ritual to assess progress, update stakeholders, and plan next week.

## When to Run

- Every Friday (or last day of your work week)
- Before weekly stakeholder syncs
- After sprint completion

## Time Required

30-45 minutes

---

## Steps

### Step 1: Review Progress

**Goal:** Assess what got done this week

**Actions:**
1. Check AHA! for completed features/updates
2. Review merged MRs in GitLab
3. Check completed items in your task list

**Questions to answer:**
- What shipped?
- What moved forward?
- What's still blocked?

**Output:** List of accomplishments and blockers

---

### Step 2: Update GOALS.md

**Goal:** Keep priorities current

**Actions:**
1. Update sprint tasks (check off completed)
2. Move blocked items to "Blocked" section
3. Add new items for next week

**File:** `GOALS.md`

**Checklist:**
- [ ] Completed items checked off
- [ ] Blocked items have "waiting on" noted
- [ ] Next week's priorities added

---

### Step 3: Draft Stakeholder Update

**Skill:** `skills/stakeholder-comms.md`

**Input:**
- Progress from Step 1
- Blockers that need escalation
- Next week's focus

**Output:** Weekly status update

**Checklist:**
- [ ] TL;DR is clear and concise
- [ ] Blockers have specific asks
- [ ] Next steps have owners and dates

---

### Step 4: Update Context Files

**Goal:** Keep context fresh for next week

**Actions:**
1. Update `context/aha/` with current feature status
2. Archive stale context files
3. Note any new context needed

**Checklist:**
- [ ] Context files are current
- [ ] Stale files removed or archived
- [ ] New context needs identified

---

### Step 5: Plan Next Week

**Goal:** Set up for a productive Monday

**Actions:**
1. Review calendar for key meetings
2. Identify top 3 priorities
3. Block focus time for deep work

**Output:** Next week's priorities in GOALS.md

**Checklist:**
- [ ] Top 3 priorities identified
- [ ] Calendar reviewed for conflicts
- [ ] Focus time blocked

---

## Weekly Review Checklist

- [ ] **Progress reviewed** - What shipped, what's blocked
- [ ] **GOALS.md updated** - Current priorities reflected
- [ ] **Stakeholder update sent** - Status communicated
- [ ] **Context files refreshed** - Stale content removed
- [ ] **Next week planned** - Top priorities set

---

## Template: Weekly Update

```
## Weekly Update: [Date]

### TL;DR
- [Biggest win this week]
- [Top blocker or risk]
- [Next week's focus]

### Shipped
- [Item 1]
- [Item 2]

### In Progress
- [Item] - ETA: [Date]

### Blocked
- [Item] - Waiting on: [Person/thing]

### Next Week
1. [Priority 1]
2. [Priority 2]
3. [Priority 3]
```

---

## Example Run

> "Run the weekly-review workflow"

Claude will guide you through each step, helping you update GOALS.md and draft your stakeholder update.
