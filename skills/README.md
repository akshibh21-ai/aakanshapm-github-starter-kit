# PM Skills

Callable PM capabilities that reference your `CLAUDE.md` context.

## Available Skills

| Skill | Purpose | When to Use |
|-------|---------|-------------|
| `prd-writer.md` | Generate PRDs from rough context | Starting a new feature |
| `aha-ticket-manager.md` | Manage AHA! features/requirements | Creating/updating requirements |
| `stakeholder-comms.md` | Draft status updates, escalations | Weekly updates, blockers |
| `spec-reviewer.md` | Review tech specs, flag gaps | Before spec sign-off |
| `figma-handoff-notes.md` | Generate dev handoff docs | Design -> Engineering handoff |
| `gitlab-mr-context.md` | Add PM context to MRs | Before MR merge |
| `customer-feedback-synth.md` | Synthesize Ideas Portal feedback | Prioritization planning |
| `meeting-summarizer.md` | Summarize Teams recordings | After key meetings |

## How to Use

Ask Claude to use a skill by name:

> "Use the prd-writer skill to create a PRD for [feature description]"

Or reference the skill file:

> "Follow the approach in skills/spec-reviewer.md to review this spec: [paste spec]"

## Skill Structure

Each skill file contains:
- **Purpose:** What the skill does
- **When to Use:** Trigger situations
- **Required Inputs:** What you need to provide
- **Output Format:** What you'll get back
- **Prompt:** The actual instructions Claude follows
