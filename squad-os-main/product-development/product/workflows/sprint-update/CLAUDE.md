# Sprint / Stakeholder Update Workflow

## Purpose

A reusable, interactive workflow that compiles a recurring squad update —
**what we shipped and are building, key metrics, and what's next** — into a
presentation-ready doc, with an optional auto-push to a shared Google Doc.

> **Status: template (not yet wired up).** No recurring report is committed to
> this cadence yet. Use/adapt this when the squad wants a standing update
> (e.g. end-of-sprint or a stakeholder summary).

## What this workflow does

1. **Sprint status** — pull completed Jira issues + PM context → "what we shipped / are building"
2. **Metrics snapshot** — pull key OKR metrics (Looker / Heap / Data Studio)
3. **Next steps** — upcoming priorities, blockers, decisions needed
4. **Push to Google Doc** — optional auto-push via Google Workspace MCP
5. **Review & finalize** — PM reviews, edits, signs off

Each step reads its own instruction file (`step-1-…` … `step-5-…`).

## Output

- Location: `output/YYYY-MM-DD-sprint-update.md`
- The markdown file is the source of truth; the Google Doc (if used) is a distribution copy.

## Cadence

Not fixed — trigger it when you want an update. If it becomes standing, the natural
fit is the bi-weekly sprint boundary (see [`../../meetings/cadences.md`](../../meetings/cadences.md)).
