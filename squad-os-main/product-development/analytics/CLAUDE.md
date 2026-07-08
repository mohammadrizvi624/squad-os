# Analytics

Analytics resources for the Marketplace Experience. We work closely with
**Data Foundations** (Connor Courtney's team), who own platform-level data and
insights across the Wholesale Network.

## Contents

| Folder/File | Description |
|-------------|-------------|
| `queries/` | SQL query patterns |
| `schemas/` | Table / collection documentation for our data sources |
| `metrics/` | Metric definitions |
| `dashboards/` | Dashboard docs (what's where, how to read them) |
| `experiments/` | A/B experiment designs & results |
| `investigations/` | Ad hoc analyses |
| `playbooks/` | Repeatable analysis playbooks (e.g. funnel analysis) |

Organized **flat** (no product-area subfolders); tie analytics artifacts to features via `../feature-index.yaml`.

> These subfolders are created as content lands — don't be surprised if some don't exist yet.

---

## Data Sources

Our data is spread across several systems:

| Source | Description |
|--------|-------------|
| **MongoDB** | Application/operational data |
| **Heap** | Product analytics — user actions, funnels, feature adoption |
| **Looker** | BI / modeled metrics & dashboards |
| **Google Data Studio** | Reporting dashboards |

> Access details and the canonical source for each metric: confirm with Data Foundations.

---

## Core Metrics (from our OKRs)

See [`../product/strategy/okrs/2026-q3-okrs.md`](../product/strategy/okrs/2026-q3-okrs.md) for objectives and targets.

**Demand (sourcing journey)**
| Metric | Definition |
|--------|------------|
| Search-to-positive-interaction rate | % of buyer searches that lead to a positive interaction |
| Add-to-cart rate | % of buyers / sessions that add to cart |
| 90-day repeat add-to-cart rate | % of buyers who add to cart again within 90 days |

**Density (discovery & connections)**
| Metric | Definition |
|--------|------------|
| Connection requests / buyer / month | Avg connection requests a buyer sends to brands per month |
| Connection approval rate / month | % of requests brands approve |
| New-connection activation rate (90d) | % of new connections where the buyer orders an item from the brand within 90 days |

---

## Dashboards

_To document as we stand them up (Looker / Data Studio)._
