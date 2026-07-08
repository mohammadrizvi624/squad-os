# Sprint / Stakeholder Update — Workflow Spec

## Overview

Produces a dated squad update document. Runs interactively: each step has an
automated part (pull data, draft) and an interactive part (the PM reviews, adds
context, approves). Each section is written to the output file as it completes so
progress is visible in real time. The final step can auto-push the compiled
document to a Google Doc via the Google Workspace MCP.

---

## Process Flow

```
1. Create dated output file
2. Step 1: Sprint Status   -> "What We Shipped / Are Building" section
3. Step 2: Metrics Snapshot -> key OKR metrics table
4. Step 3: Next Steps      -> upcoming priorities, blockers, decisions
5. Step 4: Push to Google Doc (optional) -> via Google Workspace MCP
6. Step 5: Review & Finalize -> PM reviews, edits, signs off
```

---

## What changes every cycle vs. what's stable

### Changes every cycle
- **Sprint status:** which issues shipped / are in progress (from Jira + PM context)
- **Metrics snapshot:** latest numbers
- **Next steps:** upcoming priorities and blockers

### Stable across cycles (carried forward)
- **OKR structure and goals:** update only when OKRs change (see `../../strategy/okrs/`)
- **Section structure / table of contents**

---

## Conventions

- Business-goal-led headings, not feature-led
- Tables and bullets for scannable content; short paragraphs for narrative
- Map work to our two objectives — **Demand** (sourcing) and **Density** (discovery/connections)
- Keep it skimmable for stakeholders who weren't in the room

---

## File Naming

- Output files: `output/YYYY-MM-DD-sprint-update.md`

---

## Google Doc Auto-Push (optional)

Step 4 can push the compiled update to a Google Doc using the Google Workspace MCP
(`mcp__google_workspace__*`). The markdown file stays the source of truth. See
`step-4-push-to-gdoc.md`. Skip this step to transfer manually.

---

## Data sources

- **Jira** — completed/in-progress issues for the sprint status
- **Looker / Heap / Google Data Studio** — metrics (confirm canonical source with Data Foundations)
