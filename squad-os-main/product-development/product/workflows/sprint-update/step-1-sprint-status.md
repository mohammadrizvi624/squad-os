# Step 1: Sprint Status

## Goal

Produce the "What We Shipped / Are Building" section, organized by our two
objectives (Demand and Density).

---

## Automated part

### 1. Pull recent Jira issues
Query Jira for issues completed and in-progress in the current sprint (or the last 2 weeks).

**Filters:** squad's Jira project · state: Done + In Progress · updated within the window.

### 2. Map issues to objectives
Categorize each issue under one of our objectives (see `../../strategy/okrs/2026-q3-okrs.md`):
- **Demand** — sourcing journey: search, browse, add-to-cart, reorder
- **Density** — discovery and connections: requests, approvals, activation

Flag anything that doesn't map cleanly.

### 3. Draft status
For each objective, draft a short status: what shipped, what's in progress, what's next.

---

## Interactive part

### 4. Present the issue summary to the PM
Show completed + in-progress issues grouped by objective, plus anything unmapped.

### 5. Ask for context
Prompt: **"Dump any additional context — decisions, blockers, status not captured in Jira."**

### 6. Synthesize and write
Combine Jira data + PM context into the section and write it to the output file. Present for review before Step 2.

---

## Output format

```markdown
# Sprint Update — YYYY-MM-DD

## What We Shipped / Are Building

### Demand (sourcing)
| Work | Why it matters | Status |
|------|----------------|--------|
| **[Item]** | [Impact] | [Shipped / In progress / Next] |

### Density (discovery & connections)
| Work | Why it matters | Status |
|------|----------------|--------|
| **[Item]** | [Impact] | [Shipped / In progress / Next] |
```

## Notes
- OKR goals don't change within a quarter — only the rows and statuses do.
- If something shipped, note it in a "Shipped" line and drop it from the in-progress rows next cycle.
