# Squad Intake — Working Notes (temporary)

> Scratchpad captured during Phase 0 intake. We'll distill this into the real
> root `CLAUDE.md` and content files in later phases, then delete this file.
> Anything marked ❓ is an open question to confirm.

---

## 1. Squad & Mission

### Org placement
Lightspeed → **Retail** org → **Wholesale B2B** → **Network Foundations** pod → **Marketplace Experience** squad (us).

### Product context
- Lightspeed has a retail POS system and a B2B wholesale website called **NuOrder**.
- **NuOrder** is where retailers ("**buyers**") source products for their stores: connect with brands they already work with, browse catalogs, build line sheets, place/book orders — and discover *new* brands to expand their catalog, connections, and revenue.
- **Marketplace Experience** (our product) launched **~August 2025** as a **beta to ~10,000 retailers** (out of a total base of ~100,000). It's a new, more **consumer-like shopping & discovery** experience for B2B wholesale — a new way for retailers to browse/shop with brands and discover new ones.
- It does **not** replace the legacy **Brand Portal** experience, which still exists on NuOrder and coexists.
- Currently in **beta**; targeting **General Access (GA) launch to all ~100k retailers by mid-August 2026 (Aug 17, 2026)**.

### Vision / North Star
> Be the go-to place for network retailers to effortlessly source from brands they already trust and seamlessly discover new brands they'll love.

### Quarterly Objectives & Key Results

**Objective 1 — Drive network demand** by streamlining the sourcing journey and eliminating key friction points for buyers.
- KR: Increase **search-to-positive-interaction rate** (buyers)
- KR: Increase **add-to-cart rate** (buyers)
- KR: Increase **90-day repeat add-to-cart rate** (buyers)

**Objective 2 — Increase network density** by improving discovery and closing cross-grabs between network buyers and brands.
- KR: Increase avg **connection requests sent per buyer per month** (to brands)
- KR: Increase **connection approval rate per month** (from brands)
- KR: Increase **new-connection activation rate within 90 days** (buyer places an order for an item from the newly connected brand within 90 days)

---

## 2. Team

### Core squad — leadership trio
| Role | Name | Location |
|------|------|----------|
| Product Manager | Mohammad Rizvi (you) | ❓ |
| Engineering Manager | Nev Sutter | ❓ |
| Product Designer | Sinnah Koromai | ❓ |

### Core squad — engineering
| Role | Name | Location |
|------|------|----------|
| Staff Engineer | Wayne Renaud | Ontario |
| Senior Engineer | Marc Sangster | Belfast |
| Senior Engineer | Mathieu Hendey | Belfast |
| Senior Engineer | Steven Adams | Belfast |
| Engineer II | Dmytro Liakhov | Turkey |
| Engineer I | Vitali Sokolov | Poland |
| QA II | Artem Aksani | Poland |
| QA II | Sumeet Singh | London |

### Extended partners / cross-functional (confirmed: partners, not core squad)
| Role | Name | Location | Notes |
|------|------|----------|-------|
| Data Foundations Team Lead | Connor Courtney | ❓ | Operates at platform level across the Wholesale Network; puts data/insights at the heart of product strategy, measures product performance, builds data products |
| Sr Product Marketing Manager | Kayla Shaw | Toronto | PMM for the Wholesale Network; key partner for positioning, messaging, GTM |
| Senior GTM Program Manager | Marisa Aziz | ❓ | |

---

## 3. Tools & systems

| Category | Tool(s) |
|----------|---------|
| Issue tracker / planning | **Jira** (main planning & dev) |
| Docs / wiki | **Confluence** |
| Team chat | **Slack** |
| Productivity | **Google Workspace** (Drive, Docs, Sheets, Gmail) |
| Design | **Figma** |
| Data (scattered) | **MongoDB**, **Heap** (product analytics), **Looker**, **Google Data Studio** |
| Meetings | **Zoom** + **Google Meet** |
| User research | **Dovetail** |

## 4. What applies to your squad

- **External customer accounts:** ❌ NOT tracked. Squad is in development, interacts with customers; no per-account CRM-style tracking.
- **User/customer interviews:** ✅ Done from time to time, tracked in **Dovetail** → want a lightweight research area, not an accounts structure.
- **Competitors:** ✅ KEEP — want to monitor competitors (may not be doing it formally yet).
- **Analytics maturity:** ✅ High — run A/B experiments, have SQL, maintain dashboards, work with Data Foundations (Connor's team).
- **Data engineering:** ✅ Interact with Connor's Data Foundations team (platform-level).
- **Design docs:** Primarily in **Figma** (can also keep in repo, but Figma is source of truth) → keep design as a stub/link-out.

## 5. Rituals & cadences (immediate squad)

| Ritual | Cadence | Time (Toronto) | Attendees |
|--------|---------|----------------|-----------|
| Daily standup | Daily | 9:00 am | Squad |
| Sprint planning | Bi-weekly, Thursdays | 9:30 am | Squad |
| Design sprint planning | Bi-weekly, Thursdays | 3:00 pm | Design + squad |
| Trio sync & planning | Weekly, Tuesdays | 10:30 am | PM + EM + Designer |

- Other recurring meetings with business stakeholders (Product Ops, GTM, Marketing) exist but are **deferred** — will add as needs emerge.
- No specific recurring report named yet to automate (candidate: adapt the bi-weekly workflow to Google Docs later).
