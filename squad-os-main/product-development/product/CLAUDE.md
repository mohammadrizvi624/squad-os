# Marketplace Experience — Product Context

## Overview

The Marketplace Experience is a new, consumer-like shopping and discovery
experience for B2B wholesale on **NuOrder**, letting retailers ("buyers") browse
and shop with brands and discover new brands. In beta since ~Aug 2025; GA to the
full retailer base targeted **Aug 17, 2026**. Coexists with the legacy Brand Portal.

**North Star:** Be the go-to place for network retailers to effortlessly source
from brands they already trust and seamlessly discover new brands they'll love.

**New here?** Read the [product overview & glossary](product-context/marketplace-overview.md) first.

---

## Strategic thrusts

Both map directly to our current objectives (see [OKRs](strategy/okrs/2026-q3-okrs.md)):

| Thrust | What it means | Objective |
|--------|---------------|-----------|
| **Demand** | Remove friction from the sourcing journey so buyers do more, faster, and return | Drive network demand |
| **Density** | Improve discovery and make new buyer↔brand connections activate into orders | Increase network density |

---

## Folder Structure

```
product/
├── product-context/          # Product primer + glossary (read first)
├── strategy/                 # Vision + OKRs
├── PRDs/                     # Product requirement documents
├── research/                 # User research: interviews & insights (Dovetail)
├── competitive-research/     # Competitor intel
├── launch-emails/            # Launch communications
├── processes/                # Operational processes
├── meetings/                 # Cadences, agendas, summaries
└── workflows/                # Workflow specs (e.g. recurring updates)
```

Note: `analytics/`, `engineering/`, `data-engineering/`, and `design/` are sibling folders to `product/` under `product-development/`. Each folder has its own `CLAUDE.md`.

Files are organized **flat** within each area (no forced product-area buckets) — navigation is driven by `feature-index.yaml`. See `DECISIONS.md` (repo root) for the rationale.

---

## Key Documents

| Purpose | Path |
|---------|------|
| Product overview & glossary | `product-context/marketplace-overview.md` |
| Vision | `strategy/vision/marketplace-vision.md` |
| OKRs (current) | `strategy/okrs/2026-q3-okrs.md` |
| Competitive research | `competitive-research/CLAUDE.md` |
| User research | `research/CLAUDE.md` |
| PRDs | `PRDs/CLAUDE.md` |
| Analytics | `../analytics/CLAUDE.md` |

---

## Terminology

Full glossary in [`product-context/marketplace-overview.md`](product-context/marketplace-overview.md#glossary). Core terms: **buyer** (retailer sourcing on NuOrder), **brand** (supplier), **connection** (buyer↔brand relationship enabling orders), **connection activation** (a new connection producing a real order within 90 days), **sourcing** (search→browse→add-to-cart→order), **discovery** (finding new brands), **Brand Portal** (legacy experience, coexists).
