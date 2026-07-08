# Marketplace Experience — Squad OS

The shared brain of the **Marketplace Experience** squad. Start here.

We own the **Marketplace Experience** on NuOrder — a new, consumer-like shopping
and discovery experience for B2B wholesale, currently in beta and heading to GA
on **Aug 17, 2026**. New here? Read
[`product-development/product/product-context/marketplace-overview.md`](product-development/product/product-context/marketplace-overview.md).

**Org placement:** Lightspeed → Retail → Wholesale B2B → Network Foundations pod → **Marketplace Experience** squad.

---

## Squad

### Core squad
| Function | Name | Location |
|----------|------|----------|
| Product Manager | Mohammad Rizvi | — |
| Engineering Manager | Nev Sutter | — |
| Product Designer | Sinnah Koromai | — |
| Staff Engineer | Wayne Renaud | Ontario |
| Senior Engineer | Marc Sangster | Belfast |
| Senior Engineer | Mathieu Hendey | Belfast |
| Senior Engineer | Steven Adams | Belfast |
| Engineer II | Dmytro Liakhov | Turkey |
| Engineer I | Vitali Sokolov | Poland |
| QA II | Artem Aksani | Poland |
| QA II | Sumeet Singh | London |

### Extended partners (cross-functional)
| Function | Name | Location | How we work together |
|----------|------|----------|----------------------|
| Data Foundations Team Lead | Connor Courtney | — | Platform-level data & insights across the Wholesale Network; our measurement partner |
| Sr Product Marketing Manager | Kayla Shaw | Toronto | Positioning, messaging, GTM for the Wholesale Network |
| Sr GTM Program Manager | Marisa Aziz | — | GTM program management |

> GitHub handles, Jira account IDs, and Slack IDs are `TBD` — add as needed.

---

## Tools & Systems

| Category | Tool |
|----------|------|
| Issue tracking / planning | **Jira** |
| Docs / wiki | **Confluence** |
| Team chat | **Slack** |
| Productivity | **Google Workspace** (Drive, Docs, Sheets, Gmail) |
| Design | **Figma** |
| Product analytics & data | **MongoDB**, **Heap**, **Looker**, **Google Data Studio** |
| User research | **Dovetail** |
| Meetings | **Zoom**, **Google Meet** |

> Slack channels: `TBD` — add the squad's channels + IDs here.

---

## Rituals & Cadences

| Ritual | Cadence | Time (Toronto) | Attendees |
|--------|---------|----------------|-----------|
| Daily standup | Daily | 9:00 am | Squad |
| Sprint planning | Bi-weekly (Thu) | 9:30 am | Squad |
| Design sprint planning | Bi-weekly (Thu) | 3:00 pm | Design + squad |
| Trio sync & planning | Weekly (Tue) | 10:30 am | PM + EM + Designer |

Details: [`product-development/product/meetings/CLAUDE.md`](product-development/product/meetings/CLAUDE.md).

---

## Terminology

The full glossary (buyer, brand, connection, activation, line sheet, sourcing,
discovery, Brand Portal…) lives in the
[product overview](product-development/product/product-context/marketplace-overview.md#glossary).
Quick anchors: **buyers** = retailers sourcing on NuOrder; **brands** = the
suppliers they source from; **connections** = buyer↔brand relationships that
enable ordering.

---

## Doc Index

**When looking up artifacts for a specific feature (PRDs, RFCs, plans, metrics, tickets), check `product-development/feature-index.yaml` first.** It maps every feature to all related artifacts in one place.

| Area | File | Description |
|------|------|-------------|
| Feature index | `product-development/feature-index.yaml` | Master lookup — feature → PRDs, RFCs, plans, metrics, Jira keys |
| Product overview | `product-development/product/product-context/marketplace-overview.md` | Product primer + glossary — **read first** |
| Product | `product-development/product/CLAUDE.md` | Product context, strategic thrusts, folders |
| Strategy | `product-development/product/strategy/CLAUDE.md` | Vision + OKRs |
| PRDs | `product-development/product/PRDs/CLAUDE.md` | Product requirement documents |
| Research | `product-development/product/research/CLAUDE.md` | User research: interview summaries & insights (Dovetail) |
| Competitive research | `product-development/product/competitive-research/CLAUDE.md` | Competitor intel |
| Launches | `product-development/product/launch-emails/CLAUDE.md` | Launch communications |
| Processes | `product-development/product/processes/CLAUDE.md` | Operational processes |
| Meetings | `product-development/product/meetings/CLAUDE.md` | Cadences, agendas, summaries |
| Analytics | `product-development/analytics/CLAUDE.md` | Metrics, SQL, dashboards, experiments |
| Engineering | `product-development/engineering/CLAUDE.md` | Plans, RFCs, bug investigations |
| Data engineering | `product-development/data-engineering/CLAUDE.md` | Shared pipeline work with Data Foundations |
| Design | `product-development/design/CLAUDE.md` | Design (source of truth in Figma) |
| Team | `team/CLAUDE.md` | Onboarding guides and team resources |

---

## Agents

| Agent | Purpose |
|-------|---------|
| `sprint-summary` | PM agent — reads the active Jira sprint and produces a high-level summary + per-ticket, plain-English breakdown of what each person is working on and why it matters. Team-agnostic; config in `.claude/sprint-summary.config.yaml` (pre-set to Market Experience Board, `NU`). Guided first-time setup if unconfigured |
| `onboarding` | Walks a new squad member through the onboarding guides |
