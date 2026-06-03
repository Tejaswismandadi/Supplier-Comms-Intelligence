# Supplier Communications & Intelligence Program

**A complete operational framework for managing global supplier outreach at scale.**

Built to demonstrate end-to-end program management capability for supplier communications, data integrity, escalation management, and leadership reporting across a complex global supply base.

---

## The problem this solves

Global manufacturers buy from 800+ suppliers across 20+ countries. Managing communication with all of them — collecting compliance data, running risk assessments, tracking who responded and who didn't — is typically done through scattered emails and spreadsheets with no visibility or accountability.

This program provides a structured, connected, end-to-end approach: from scoring and prioritizing suppliers using a proven risk methodology, to designing campaigns, to tracking responses, to escalating gaps, to reporting to leadership.

---

## The complete package

| Deliverable | What it is |
|---|---|
| **[Live Platform →](https://tejaswismandadi.github.io/Supplier-Comms-Intelligence/)** | Interactive web tool — add suppliers, run campaigns, track responses, export reports |
| **Excel Operations Tool** | 7-sheet connected workbook — REI scoring, contact database, campaign calendar, live tracker, escalation log, dashboard, email templates |
| **Program Plan PPT** | 8-slide deck covering the problem, solution, campaign types, process flow, and metrics |

---

## How the program works — 7 steps in sequence

### Step 1 — Supplier Prioritization (Simchi-Levi REI Method)

Before any campaign launches, every supplier is scored using the **Risk Exposure Index (REI)** developed by MIT Professor David Simchi-Levi.

**REI = Time to Recover (TTR) − Time to Survive (TTS)**

| Factor | Definition |
|---|---|
| **TTR — Time to Recover** | How many weeks to find an alternate source if this supplier goes down |
| **TTS — Time to Survive** | How many weeks KLA can continue production without this supplier |
| **REI Score** | TTR minus TTS. Positive = critical risk. Supplier takes longer to recover than KLA can survive. |

**Composite Risk Score adds:**
- Single source flag (25% weight) — automatic P1 if only approved source
- Annual spend exposure (20% weight)
- Financial risk flag (10% weight) — watch list trigger
- Performance history inverse score (10% weight)

**Resulting segments:**

| Segment | Criteria | Escalation Window |
|---|---|---|
| **Critical / P1** | Single source OR REI score high OR spend ≥$5M | 7 days |
| **Strategic / P2** | Spend ≥$2M | 14 days |
| **Preferred / P3** | Spend ≥$500K | 21 days |
| **Approved / P4** | Lower spend | 30 days |
| **Watch List** | Financial risk flag OR 2+ performance failures | Immediate |

### Step 2 — Supplier Master List

Complete contact database. Segment and escalation window pull automatically from Step 1 via formula — never re-entered manually.

### Step 3 — Campaign Calendar

Annual plan for all supplier outreach. Escalation windows per segment flow from Step 1 automatically.

| Campaign Type | What we collect | Frequency |
|---|---|---|
| **Regulatory Compliance** | CO2 emissions, CBAM certificates, conflict minerals, RoHS/REACH | Quarterly / Annual |
| **Risk & Financial Health** | REI inputs, business continuity plans, sub-tier visibility | Annual |
| **Performance & Corrective Action** | Root cause analysis, corrective action plans | Event-triggered |
| **Contact & Master Data** | Contact verification, portal registration, code of conduct | Semi-annual |

### Step 4 — Campaign Tracker

Daily operations sheet. Supplier name, region, tier, and email pull automatically from Step 2. You only update the STATUS column. Days since outreach and escalation flags calculate automatically based on the supplier's REI segment escalation window.

### Step 5 — Escalation Log

Suppliers marked Escalated in the tracker auto-populate here. Document every action taken with a date. This is the audit trail.

### Step 6 — Dashboard

All KPIs, response rates by region and tier, segment portfolio breakdown, and gap analysis pull automatically from the tracker and REI sheet. Share this tab with leadership monthly.

### Step 7 — Email Templates

Five ready-to-use templates referencing the supplier's REI segment and escalation window:
1. Compliance data request
2. Annual risk assessment (references REI score)
3. Corrective action request
4. Contact verification
5. Escalation reminder — Stage 2

---

## How the sheets connect

```
Sheet 1 — REI Prioritization
    ↓ Segment + Escalation Window (INDEX/MATCH)
Sheet 2 — Supplier Master
    ↓ Name, Region, Tier, Email (direct reference)
Sheet 4 — Campaign Tracker
    ↓ KPI metrics, response rates (COUNTIFS)        ↓ Escalated rows (direct reference)
Sheet 6 — Dashboard                              Sheet 5 — Escalation Log
```

Change a supplier's TTR in Sheet 1 → REI score updates → segment updates → escalation window updates → tracker flag updates → dashboard reflects change.

---

## Who does what — RACI

| Activity | Program Manager | Sourcing / Category Mgr | Compliance | Quality | IT |
|---|---|---|---|---|---|
| REI scoring and segmentation | **R** | C | I | I | I |
| Design and launch campaign | **R** | C | C | C | C |
| Track supplier responses | **R** | I | I | I | C |
| Stage 1-2 reminders | **R** | I | I | I | I |
| Stage 3+ escalation | R notifies | **R** acts | I | I | I |
| Validate data received | C | C | **R** | **R** | I |
| Build leadership dashboard | **R** | C | C | I | C |
| Monthly leadership report | **R** | A | C | I | I |

---

## Success metrics

| Metric | Target |
|---|---|
| Response rate per campaign | 85%+ |
| Average supplier response time | Under 5 days |
| Contact data accuracy | 95%+ verified |
| Escalation resolution time | Under 14 days (P1: under 7 days) |
| REI scores updated | Quarterly |

---

## Tools built

**Excel Operations Tool** — 7 connected sheets, 295 live formulas, Simchi-Levi REI scoring, cross-sheet INDEX/MATCH references, auto-calculated escalation flags, live dashboard charts.

**Web Platform** — HTML/CSS/JavaScript with Chart.js. Campaign management, supplier tracking, live dashboards, gap analysis, escalation tracker, CSV import/export, leadership report generation.

---

## About

**Tejaswi Sreerama** — Supply Chain Program Manager
12 years automotive engineering experience | MSCM, University of Michigan Ross School of Business

- Email: tejaswismandadi@gmail.com
- LinkedIn: [linkedin.com/in/tejaswisreerama](https://linkedin.com/in/tejaswisreerama)
- AutoCost Pro (automotive sourcing intelligence): [tejaswismandadi.github.io/Autocost-pro](https://tejaswismandadi.github.io/Autocost-pro)

