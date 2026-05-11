# Context Folder

Store synced context from your external tools here. Keep summaries, not full documents.

## Folder Structure

```
context/
├── aha/                  # AHA! requirements snapshots
├── ideas-portal/         # Customer feedback themes from AHA! Ideas
├── confluence/           # Key spec summaries
├── figma/                # Design context and notes
└── gitlab/               # Active MR context
```

## How to Use

### AHA! (`context/aha/`)
- Export prioritization board snapshots
- Save key feature summaries
- Example: `active-features-2026-05.md`

### Ideas Portal (`context/ideas-portal/`)
- Export and synthesize customer feedback themes
- Example: `feedback-themes-q2.md`, `top-requests.md`

### Confluence (`context/confluence/`)
- Save summaries of key specs (not full docs)
- Example: `connector-sdk-spec-summary.md`

### Figma (`context/figma/`)
- Save design notes and state descriptions
- Example: `dashboard-redesign-notes.md`

### GitLab (`context/gitlab/`)
- Save active MR context when relevant
- Example: `active-mrs.md`

## Sync Frequency

| Source | Frequency | How |
|--------|-----------|-----|
| AHA! | Weekly | Manual export |
| Ideas Portal | Weekly | Manual export + synthesis |
| Confluence | On-demand | Paste key sections |
| Figma | On-demand | Paste design notes |
| GitLab | On-demand | Paste MR context |

## Tips

- Keep files small (summaries, not full docs)
- Date your snapshots for freshness
- Delete stale context regularly
- Use these files to give Claude project context
