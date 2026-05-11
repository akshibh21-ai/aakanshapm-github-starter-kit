# PM Workflows

Multi-step processes that chain skills together.

## Available Workflows

| Workflow | Purpose | When to Run |
|----------|---------|-------------|
| `feature-kickoff.md` | End-to-end feature launch setup | Starting a new feature |
| `sprint-planning.md` | Sprint planning ritual | Start of each sprint |
| `weekly-review.md` | Weekly status and blockers | End of each week |
| `spec-to-ticket.md` | Confluence spec to AHA! features | After spec approval |

## How to Use

Ask Claude to run a workflow:

> "Run the feature-kickoff workflow for [feature name]"

## Workflow Structure

Each workflow file contains:
- **Purpose:** What end-to-end process this automates
- **When to Run:** Trigger (weekly, per-feature, etc.)
- **Steps:** Ordered steps with skills to use
- **Checklist:** Verification steps
