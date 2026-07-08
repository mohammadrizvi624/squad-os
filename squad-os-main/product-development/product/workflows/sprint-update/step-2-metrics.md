# Step 2: Metrics Snapshot

## Goal

Produce a short, scannable snapshot of our key OKR metrics and their recent movement.

---

## Process

### 1. Pull the metrics
Pull the current values for our OKR metrics (see `../../strategy/okrs/2026-q3-okrs.md`) from the canonical source (Looker / Heap / Data Studio — confirm with Data Foundations).

**Demand**
- Search-to-positive-interaction rate
- Add-to-cart rate
- 90-day repeat add-to-cart rate

**Density**
- Connection requests / buyer / month
- Connection approval rate / month
- New-connection activation rate (90d)

### 2. Compute movement
For each metric, show current value, prior-period value, and delta (↑/↓/→). Note anything notable (a big move, a metric off-track vs. target).

### 3. Interactive check
Present the table to the PM. Ask: **"Anything to caveat or exclude? Any metric to add for this update?"**

### 4. Write to output file
Append the snapshot below the sprint-status section.

---

## Output format

```markdown
## Metrics Snapshot

| Metric | Current | Prior | Δ | Notes |
|--------|---------|-------|---|-------|
| Add-to-cart rate | | | | |
| New-connection activation (90d) | | | | |
```

## Notes
- Keep it to the metrics that matter for the story — not every number we track.
- If a metric isn't yet instrumented, mark it `not yet measured` rather than guessing.
