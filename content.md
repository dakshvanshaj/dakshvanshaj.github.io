# Content brief for dakshvanshaj.com — for Gemini to build the frontend from

This is content only. No layout, design, or framework opinions here — that's Gemini's call. Every fact below
traces to `career/profile.md`, `career/marketplace-profiles.md`, `career/components-to-sell.md`, or a project's own
public repo/docs. Don't add claims beyond what's written here.

## Identity

- **Name:** Daksh Vanshaj
- **Location:** Rehan, Himachal Pradesh, India. Open to relocation.
- **Contact:** davevanshaj55646@gmail.com · [linkedin.com/in/daksh-vanshaj](https://linkedin.com/in/daksh-vanshaj) · [github.com/dakshvanshaj](https://github.com/dakshvanshaj)
- **Logo:** a "DV" logo exists but isn't in this repo yet — Daksh will drop the file into `assets/` himself.
- **Photos:** candidates already on disk at `/home/daksh_linux/projects/my-profile/` (not copied here yet — pick
  one and copy it into `assets/` when building).

## Headline / positioning (pick one, or let Gemini vary by section)

- Short: **AI Automation & Workflow Builder — Claude Code, n8n, Python**
- Long: **I turn operational pain — messy CRMs, spreadsheets, manual follow-ups — into working automated systems
  using Claude Code, n8n and Python.**

## About (long form, for an About section)

AI automation specialist who turns operational pain — messy ERP exports, manual spreadsheets, repetitive tasks —
into working systems using Claude Code, n8n, Python and SQL. I build end to end, from the data pipeline to the AI
layer, not just individual nodes: validation, error handling, a human-approval step before anything goes out, and
documentation someone else could follow. As founder of Narada OS I built a full ops platform solo; day to day I
bring the same systems thinking to smaller builds — CRM/ops automations, internal tools, AI-assisted websites and
data analysis, whatever the operation actually needs.

**Honesty rules for this section — do not soften these:**
- Narada OS has no paying customers. Say what was built, never that distributors use it.
- Don't claim deep line-by-line authorship of the code. The honest framing: "I directed the architecture and
  product decisions, Claude Code implemented it, I reviewed every output." Agents are how it was built, not the
  headline.

## Services offered (what a visitor should understand you'd take on)

1. **CRM → Ops follow-up automation** (primary/lead offer) — when a deal closes, the right person gets a task and
   an alert automatically, with a follow-up due date and a weekly review. Works with HubSpot, Pipedrive,
   GoHighLevel, Zoho, Salesforce out of the box; adapts to others.
2. **Document / invoice / receipt extraction** (secondary offer) — turn a photo or PDF of an invoice/order into
   structured data a human reviews before it's used.
3. General: AI-assisted websites, internal tools, and data analysis/automation — "whatever the operation needs,"
   built with Claude Code, n8n, and Python.
4. **AI agents over your own business data** — a chat agent that answers from verified lookups only (never a
   guessed number) and can draft a purchase order, a supplier email, or a config change for your approval, never
   executing on its own. The architecture is proven in production (see Straight Answer Agent below); each build is custom
   to the client's own data and tools, not a resold copy.

## Proof projects (lead with these, in this order)

### 1. CloseLoop — never let a closed deal go cold (public, live docs)
- **What:** n8n automation — CRM deal closes → task created with a business-day-aware follow-up due date → owner
  alerted on WhatsApp/email → weekly review of what's overdue.
- **Links:** [repo](https://github.com/dakshvanshaj/CloseLoop) · [docs](https://dakshvanshaj.com/CloseLoop/)
- **Status:** rules fully tested (`handoff ok`); generalized from a real deployment; not yet run against a live
  client's CRM.

### 2. FirstReply — never let an interested lead go quiet (public, live docs)
- **What:** instant reply to a new lead (form, Meta Lead Ad, WhatsApp, email) + alert to the owner + logged to a
  sheet, with a morning digest for anyone needing a human follow-up.
- **Links:** [repo](https://github.com/dakshvanshaj/FirstReply) · [docs](https://dakshvanshaj.com/FirstReply/)
- **Status:** rules fully tested (`respond ok`); not yet run against a live client's intake source.

### 3. SnapTally — never type another invoice by hand (public, live docs)
- **What:** photo or PDF of an invoice/receipt → AI reads it (Claude vision) → the arithmetic gets checked →
  flagged for a quick human review before anything reaches accounting. Approval resets automatically if a
  re-scan's figures change.
- **Links:** [repo](https://github.com/dakshvanshaj/SnapTally) · [docs](https://dakshvanshaj.com/SnapTally/)
- **Status:** rules fully tested (`extract ok`); not yet run against a real client invoice.

### 4. RecapRelay — never let a call's follow-ups fall through (public, live docs)
- **What:** a call's transcript → AI extracts the summary, action items, and risk flags (budget pushback, a
  competitor mention) → logged to a Meetings/Action Items sheet → owner alerted; a weekly digest catches any
  action item still open. A human's "Done" mark on an action item always survives a re-processed transcript.
- **Links:** [repo](https://github.com/dakshvanshaj/RecapRelay) · [docs](https://dakshvanshaj.com/RecapRelay/)
- **Status:** rules fully tested (`recap ok`); not yet run against a real transcript source.

### 5. Straight Answer Agent — an AI agent that never makes up a number (public, live docs + video demo)
- **What:** case study describing the real tool-use agent behind Narada OS — plan/execute/narrate architecture,
  a 42-tool registry (34 read-only, 8 propose-only — a purchase order or supplier email draft, never sent or
  executed without a human), a four-part trust layer (input limits, prompt-injection fencing, cite-or-omit
  outputs, redacted logs), and tenant-isolated memory on a local embedding model.
- **Links:** [repo](https://github.com/dakshvanshaj/straight-answer-agent) · [docs](https://dakshvanshaj.com/straight-answer-agent/)
  — includes the real 2-minute product demo video and two annotated screenshots.
- **Honesty rules for this one — do not soften:** the production source is intentionally NOT published (it's
  real proprietary software for Narada OS, a venture with no paying customers — don't imply otherwise). This is
  a documentation/case-study repo, not a downloadable template; say "the architecture is proven, each build is
  custom," never "download and use this."

### 6. StoreCast — demand forecasting case study (public, demo)
- **What:** a medallion-architecture (PySpark/Polars/DuckDB) ML pipeline forecasting weekly retail demand across
  a 45-store pilot region, with anomaly detection and department-level market-basket analysis alongside it.
  Cuts the baseline "last-year-same-week" heuristic's error from 11.85% to 7.76% WMAPE (XGBoost, tuned with
  Optuna), tracked via MLflow/DVC.
- **Links:** [repo](https://github.com/dakshvanshaj/StoreCast) · [docs](https://dakshvanshaj.com/StoreCast/)
- **Honesty rules for this one — do not soften:** built on a public retail dataset, not a live client's data.
  The $20.5M working-capital figure is a *simulated* projection from that error-rate improvement (documented
  math in the repo's own feasibility report), not a result any business has actually realized. Say "demonstrates
  the forecasting methodology" or "a projected result on public data" — never "saved a client $20.5M."

### 7. Narada OS — proof I can build a proactive agent, not just a reactive automation

**Framing, important:** this is not a Narada OS sales pitch — don't mention pricing, the guarantee, or the
founding-member program anywhere in the portfolio. This piece exists to show capability: "I can build this kind
of system for your operation," not "buy Narada." A visitor should come away thinking about their *own* messy
ERP/spreadsheet/manual-planning problem, not about Narada's business model.

This is still the single richest piece in the whole portfolio and deserves the most visual real estate on the
site — real screenshots and a real demo video exist for it (see below), unlike the template sites (1-6 above),
which only have diagrams. Don't treat it as a brief supporting mention; just keep the framing on capability,
not a product sale.

- **What it does:** a proactive AI agent sitting on top of a distributor's existing ERP (Odoo, SAP B1,
  NetSuite) — the same workflow-automation-and-optimization pattern as the 6 templates above, built out into a
  full system. It doesn't wait to be asked: it ingests ERP data (API, CSV export, email webhooks) and runs 95
  diagnostics every night across cash, stock, suppliers, and customers, catching things like a reorder quantity
  nobody revisited after demand dropped — before it becomes a stockout or a pile of dead stock. A
  demand-forecasting layer (XGBoost/LightGBM across 10,000+ SKUs) feeds a drafting layer that writes the actual
  purchase order or supplier email — a human approves before anything sends, nothing executes on its own. Every
  number it surfaces traces back to a formula and the business's own source rows, so nothing is just
  asserted — the system shows its reasoning, not just a conclusion.
- **Low integration friction, worth noting as a capability:** it can start from a plain CSV export — no direct
  ERP access or integration work required to get useful output.
- **The kind of ROI this shape of system surfaces** (relatable to any operation with messy ERP data or manual
  planning, not a Narada-specific claim): dead stock sitting on a shelf because a reorder setting was never
  revisited, a stockout caught before the sale is already lost, a supplier follow-up drafted automatically
  instead of relying on someone remembering to chase it. The point is the pattern — proactive, explainable,
  human-approved automation — not any specific dollar figure Narada itself has claimed.
- **Visual assets available — real captures of the live running app, not mockups:**
  - 18 real app screenshots: `/home/daksh_linux/projects/narada-website/docs/app-reference/*.jpg` (board,
    forecast, purchase-orders, erp, email, reorder, review, review-overnight, stock-watch, today, cash, ledger,
    collections, analytics, issues, activity, guide, clear-stock)
  - A real demo video + poster frame: `/home/daksh_linux/projects/narada-website/public/video/launch.mp4` +
    `launch-poster.jpg`
  - Copy the relevant ones into `assets/` when building. Lean on these for the hero/showcase treatment rather
    than describing the UI in prose alone.
- **Links:** [naradaos.com](https://naradaos.com) (fine to link out, but the portfolio page itself should stay
  on "what I can build," not reproduce Narada's own sales page)
- **Stats:** 7,600+ commits, May–Oct 2026, solo, directed with Claude Code.
- **Honesty rules for this one — do not soften:** no paying customers. Say "built and shipped solo," never
  "distributors use it" or "clients see X every morning."

### Supporting (mention briefly, don't lead with)
- **flights-price-prediction-mlops** — most complete MLOps project (DVC, MLflow, CI/CD, Cloud Run). Shows classic
  ML/deployment skill, not automation specifically.

## Skills

Claude Code · n8n · Python · SQL / PostgreSQL · REST APIs · Webhooks · OAuth · Google Sheets / Apps Script ·
JavaScript/TypeScript · Docker · FastAPI · Workflow automation · AI agents · Data pipelines

## Education

- MS Computer Science (AI/ML), Woolf — self-paced, Jul 2024 – Jul 2027 (in progress)
- Data Science Trainee, AlmaBetter — Jun 2025 – Feb 2026
- BSc (PCM), WRS Govt. College, Dehri — 2021–2024

## Resume

Point a download/contact-me link at `career/resumes/Daksh_Vanshaj_Resume_AI_Operations_Automation.pdf` (the
current consolidated resume — copy it into `assets/` when building, don't relink the older per-role variants).

## What NOT to include

- No internship history (nothing recent enough or long enough to be worth a resume/portfolio line).
- No specific client names or revenue figures — none exist yet to show.
- No claim that any project has paying users/customers.
