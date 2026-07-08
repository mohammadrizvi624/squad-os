# Squad OS — Tailoring Decisions

Living record of keep / drop / adapt decisions as we convert the Forge example
repo into the **Marketplace Experience** Squad OS.

**Legend**
- **KEEP** — structure works as-is; just repopulate with our content
- **ADAPT** — keep the pattern but change it to fit our team/tools
- **DROP** — remove entirely; doesn't apply to us
- **NEW** — add something the example didn't have

**Status:** `Proposed` → `Confirmed` (after your sign-off) → `Done` (after actioned)

---

## A. Intelligence / scaffold layer

| # | Item | Recommendation | Rationale | Status |
|---|------|----------------|-----------|--------|
| A1 | Root `CLAUDE.md` | **ADAPT** | Rewrite team roster (trio + eng/QA + partners), Slack channels, doc index, terminology (NuOrder, buyers, brands, Brand Portal, Marketplace) | Confirmed |
| A2 | `feature-index.yaml` (master cross-ref) | **KEEP** (repopulate) | Great pattern — one lookup mapping each feature → PRD/RFC/tickets/metrics. Rebuild with our features + Jira keys | Confirmed |
| A3 | Per-folder `CLAUDE.md` navigation files | **KEEP / ADAPT** | The navigation backbone. Update each as its folder changes | Confirmed |
| A4 | `.claude/commands/customer-call.md` + `skills/customer-call-summary` | **DROP** | Rely on Dovetail for interview capture; remove the command + skill | Confirmed |
| A5 | `.claude/agents/onboarding.md` | **KEEP / ADAPT** | Useful for new squad members; update role list (PM, EM, Design, Eng, QA) and guides | Confirmed |
| A6 | `product/workflows/bi-weekly-update/` | **SIMPLIFY** | Reshape into a generic recurring sprint/stakeholder update template (sprint status + metrics + next steps + optional Google-Docs push). Drop the customer-call-synthesis core (doesn't apply) | Confirmed |

## B. Product content

| # | Item | Recommendation | Rationale | Status |
|---|------|----------------|-----------|--------|
| B1 | `product/PRDs/` | **KEEP** (rebuild) | Core PM artifact. Purge Forge PRDs, keep the template/structure | Confirmed |
| B2 | `product/strategy/` (vision, roadmaps, business-context) | **KEEP / ADAPT** | Vision, OKRs, and business context all apply directly. Seed with your North Star + 2 objectives | Confirmed |
| B3 | `product/customers/` (named accounts) | **DROP** | No per-account tracking; account-per-customer folder structure removed | Confirmed |
| B4 | `product/research/` (user research layer) | **NEW** (repurpose `customers/`) | Keep a research layer: interview summaries, insights, user research (Dovetail-sourced). No account-per-customer folders | Confirmed |
| B5 | `product/competitive-research/` | **KEEP** (rebuild) | You want to monitor competitors. Purge Forge's 6 competitors, set up your own | Confirmed |
| B6 | `product/product-context/` (reference docs) | **KEEP / ADAPT** | Great home for a NuOrder / Marketplace / Brand Portal system overview | Confirmed |
| B7 | `product/launch-emails/` → `launches/` | **KEEP / ADAPT** | GA launch (Aug 17, 2026) is a big moment; keep a launch-comms area | Confirmed |
| B8 | `product/sales-enablement/` | **DROP** ⚠️ | Not sales-facing; GTM/positioning owned by Kayla & Marisa (partners) | Confirmed |
| B9 | `product/processes/` | **KEEP (light)** | Useful for beta→GA process, release checklists | Confirmed |
| B10 | `product/meetings/` | **ADAPT** | Rework to your real cadences: daily standup, bi-weekly sprint planning, design sprint planning, weekly trio sync | Confirmed |

## C. Engineering / Analytics / Data / Design content

| # | Item | Recommendation | Rationale | Status |
|---|------|----------------|-----------|--------|
| C1 | `engineering/` (plans, rfcs, bug-investigations) | **KEEP** (rebuild) | Purge Forge, keep structure | Confirmed |
| C2 | `analytics/` (metrics, queries, schemas, dashboards, experiments, investigations, playbooks) | **KEEP / ADAPT** | High analytics maturity. Swap data sources to **MongoDB / Heap / Looker / Data Studio**; seed metrics from your KRs | Confirmed |
| C3 | `analytics/data-catalog.yaml` | **KEEP / ADAPT** | Table registry — repoint at your real sources | Confirmed |
| C4 | `data-engineering/` (plans, rfcs) | **KEEP (light)** | Light footprint for shared pipeline work with Connor's Data Foundations team | Confirmed |
| C5 | `design/` | **KEEP as stub** | Design lives in Figma; keep a stub that links out (matches example) | Confirmed |

## D. Team

| # | Item | Recommendation | Rationale | Status |
|---|------|----------------|-----------|--------|
| D1 | `team/onboarding-guides/` | **DEFER** | Leave for now and rewrite later with the squad's real onboarding process. ⚠️ NOTE: these 6 files still contain Forge content by choice until then | Confirmed |
| D2 | `team/retros/` | **KEEP** | Empty stub, useful going forward | Confirmed |

## E. Product-area taxonomy — DECIDED: keep it flat/general

**No forced product-area buckets.** Files live directly under their discipline
folder (`PRDs/`, `engineering/plans/`, `engineering/rfcs/`, `analytics/...`),
with a clear naming convention. Navigation is driven by **`feature-index.yaml`**,
not deep folder trees.

- Rationale: new squad, low volume, and initiatives cut across areas — rigid
  buckets force awkward "which folder?" calls exactly when work is cross-cutting.
- If a real cluster emerges later, add a subfolder **then** — and if we ever
  group, group by **initiative / Jira epic** (how the squad plans), not abstract
  product areas.

Status: Confirmed

---

## Resolved flags
1. **A4** — DROP the customer-call command + skill (rely on Dovetail). ✅
2. **A6** — SIMPLIFY the bi-weekly workflow into a generic sprint/stakeholder update template (drop customer-call synthesis). ✅
   - **D1** — Onboarding guides DEFERRED (still contain Forge content until rewritten). ✅
3. **B3 + B4** — DROP account-per-customer structure; ADD a `research/` layer (interview summaries, insights). ✅
4. **B8** — DROP `sales-enablement/` (default; veto anytime). ✅
5. **C4** — KEEP a light `data-engineering/` area. ✅
6. **E** — Product-area taxonomy — DECIDED: keep flat/general, navigate via feature-index; no forced buckets. ✅
