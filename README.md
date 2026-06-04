# Supplier Communications & Intelligence Program

**A complete Program Manager tool for managing global supplier outreach at scale.**

Built to demonstrate end-to-end program management capability across supplier communications, data governance, RACI ownership, campaign planning, escalation management, trade compliance, and leadership reporting.

**Live platform:** https://tejaswismandadi.github.io/Supplier-Comms-Intelligence

---

## The complete package

| Deliverable | What it is |
|---|---|
| **[Live Web Platform](https://tejaswismandadi.github.io/Supplier-Comms-Intelligence/)** | 15-tab interactive PM tool covering strategy, operations, intelligence, and governance |
| **[Download Excel Operations Tool](https://github.com/Tejaswismandadi/Supplier-Comms-Intelligence/raw/main/Supplier_Comms_REI_Tool.xlsx)** | 10-sheet connected Excel workbook with 299 live formulas |
| **[Download Program Plan PDF](https://github.com/Tejaswismandadi/Supplier-Comms-Intelligence/raw/main/Supplier_Comms_Program_Plan.pdf)** | 8-slide program plan covering the problem, REI method, campaign types, process flow, and metrics |

---

## The problem this solves

Global manufacturers buy from 800 or more suppliers across 20 or more countries. Managing communication with all of them is typically done through scattered emails and spreadsheets with no visibility or accountability:

- Different teams email the same suppliers with no central tracking
- Nobody knows which suppliers responded and which need escalation
- Contact data decays at 15% per year with no governance process
- Leadership has no clean answer on supplier performance

This program provides a structured, connected approach: from scoring suppliers using a proven risk methodology, to designing campaigns, tracking responses, escalating gaps, and reporting to leadership.

---

## Tool structure

The web platform is organized as a full Program Manager tool across four sections.

### Strategy

**Program Overview**
Live program health dashboard. Response rate, escalation count, segment distribution, gap analysis, and activity log. All metrics update automatically as you change supplier statuses in Campaign Tracker.

**Campaign Calendar**
Annual plan for all 12 campaigns across 4 campaign types. Each campaign shows owner, target segment, frequency, quarter, collection window, escalation trigger rule, and output deliverable. Designed before the year starts and reviewed with sourcing and compliance teams.

**RACI Matrix**
17 program activities mapped across Program Manager, Category Manager, Compliance Team, Quality Engineering, IT and Data, Finance, and Leadership. Grouped by Strategy, Operations, Governance, and Reporting. R = Responsible, A = Accountable, C = Consulted, I = Informed.

**Program Timeline**
Full-year Gantt view of all campaigns across January to December. Color coded by campaign type. Current month highlighted. Shows when each campaign runs, who owns it, and how campaigns overlap across the year.

### Operations

**REI Scoring**
Simchi-Levi Risk Exposure Index scoring for every supplier. Enter TTR, TTS, spend, single source flag, financial risk flag, and performance score. REI score, composite risk score, segment, and escalation window calculate automatically.

**Supplier Master**
Complete contact database. Segment and escalation window pull from REI Scoring automatically. Missing emails flagged in red.

**Campaign Tracker**
Daily operations sheet. Update the STATUS dropdown only for each supplier. Response rate, escalation flags, dashboard metrics, and escalation log all update automatically. Escalation triggers per REI segment window.

**Escalation Log**
Suppliers marked Escalated populate here automatically. Shows segment, email, escalation window, and action button. Document every action with a date for a full audit trail.

### Intelligence

**Dashboard**
Leadership-ready reporting. Response rate by region and tier, segment portfolio, before vs after comparison, and gap analysis. All metrics auto-update from Campaign Tracker and REI Scoring.

**Trend Analysis**
Quarter-over-quarter response rates by region and campaign type across Q3 2025 to Q2 2026. Emerging pattern identification with recommended actions.

**Compliance**
Trade compliance campaign tracking. CO2 emissions, CBAM certificates, conflict minerals (CMRT), and RoHS/REACH. Includes real-world CBAM project data from Nexteer Automotive (Kearney consulting, 2025).

### Governance

**Contact Governance**
Five-step contact data governance process with trigger, owner, action, and timeline for each step. Contact health tracker below shows last verified date, next review date, email status, portal status, and action required for every supplier.

**Internal Stakeholder Communications**
Meeting cadence table showing who meets when and what the Program Manager delivers to each team. Information flow table showing what each internal team provides to the Program Manager and when.

---

## Step 1: Simchi-Levi REI Method

Before any campaign launches, every supplier is scored using the Risk Exposure Index developed by MIT Professor David Simchi-Levi.

**REI = Time to Recover (TTR) minus Time to Survive (TTS)**

| Factor | Definition |
|---|---|
| TTR | Weeks to find an alternate source if this supplier goes down |
| TTS | Weeks production continues without this supplier |
| REI Score | TTR minus TTS. Positive = critical risk. |

Composite score weights: single source flag 25%, annual spend 20%, financial risk flag 10%, performance history 10%, REI normalized 35%.

**Resulting segments:**

| Segment | Criteria | Escalation Window |
|---|---|---|
| Critical / P1 | Single source OR high REI OR spend above $5M | 7 days |
| Strategic / P2 | Spend above $2M | 14 days |
| Preferred / P3 | Spend above $500K | 21 days |
| Approved / P4 | Lower spend | 30 days |
| Watch List | Financial risk flag OR repeated failures | Immediate |

---

## The four campaign types

| Campaign | What we collect | Frequency |
|---|---|---|
| Regulatory Compliance | CO2 emissions, CBAM certificates, conflict minerals, RoHS/REACH | Quarterly and Annual |
| Risk and Financial Health | REI inputs, business continuity plans, sub-tier visibility | Annual |
| Performance and Corrective Action | Root cause analysis, corrective action plans | Event-triggered |
| Contact and Master Data | Contact verification, portal registration, code of conduct | Semi-annual |

---

## Six-step process flow

| Step | Activity | Owner | When |
|---|---|---|---|
| 1 | Design campaign | PM + Compliance + Sourcing | Week 1 |
| 2 | Launch outreach | Program Manager | Week 2 |
| 3 | Track and follow up | Program Manager | Daily, weeks 2-4 |
| 4 | Escalate gaps | PM notifies, Category Manager acts | Per REI segment trigger |
| 5 | Validate data received | Compliance and Quality | After submission window closes |
| 6 | Report to leadership | Program Manager | Monthly |

---

## How the Excel sheets connect

```
Sheet 1: REI Prioritization
    Segment + Escalation Window via INDEX/MATCH
    |
    v
Sheet 2: Supplier Master
    Name, Region, Tier, Email via direct reference
    |
    v
Sheet 4: Campaign Tracker
    |                      |
    COUNTIFS for KPIs      Escalated rows auto-populate
    |                      |
    v                      v
Sheet 6: Dashboard     Sheet 5: Escalation Log
```

Change a supplier's TTR in Sheet 1 and the REI score updates, the segment updates, the escalation window updates, the tracker flag updates, and the dashboard reflects the change automatically.

### All 10 Excel sheets

| Sheet | What it does |
|---|---|
| 1. REI Prioritization | Simchi-Levi scoring. Enter inputs. Score, segment, and escalation window auto-calculate. |
| 2. Supplier Master | Contact database. Segment and escalation window pull from Sheet 1 via INDEX/MATCH. |
| 3. Campaign Calendar | Annual plan for all 12 campaigns. Escalation windows flow from Sheet 1. |
| 4. Campaign Tracker | Daily operations. Supplier data from Sheet 2. Update STATUS only. Flags auto-trigger. |
| 5. Escalation Log | Escalated suppliers auto-populate from tracker. Every action documented with date. |
| 6. Dashboard | All KPIs, response rates by region and tier, before vs after. Auto-updates from tracker. |
| 7. Email Templates | Five ready-to-use templates referencing supplier REI segment and escalation window. |
| 8. Trend Analysis | Quarter-over-quarter by region and campaign type. Emerging pattern identification. |
| 9. Contact Governance | Five-step governance process. Health tracker per supplier with last verified and next review. |
| 10. Internal Stakeholder Comms | Meeting cadence and information flow between all internal teams. |

### Cell legend

| Color | Meaning |
|---|---|
| Yellow | Enter your data here |
| Teal | Auto-calculated from another sheet. Do not edit. |
| Red | Urgent attention required |
| Green | All clear |

---

## Before vs after

| Activity | Before | After | Saved |
|---|---|---|---|
| Supplier outreach | 5 teams emailing independently | Single structured campaign with auto-reminders | 80% effort reduction |
| Response tracking | Manual spreadsheet checks | Auto-calculated live in tracker | 4-6 hours per week |
| Escalation management | No system, escalations missed | REI auto-flag per segment, full audit trail | Zero missed |
| Contact data | Scattered, 15% annual decay | Verified master list, 5-step governance | 90% bounce reduction |
| Leadership reporting | Manual, 3-4 hours each time | One-click dashboard, auto-updated | 3-4 hours per month |

---

## Trade compliance experience

Built a semi-automated CBAM compliance tool for Nexteer Automotive (Kearney consulting project, 2025):
- 800+ suppliers across 7 countries
- Automated CN code mapping, CO2 data collection, weight validation, and CBAM tax calculation
- Delivered a Power BI dashboard for supplier carbon footprint comparison and CBAM cost forecasting
- Reduced manual compliance effort from hundreds of hours per quarter to minutes

---

## Success metrics

| Metric | Target |
|---|---|
| Response rate per campaign | 85% or above |
| Average supplier response time | Under 5 days |
| Contact data accuracy | 95% or above verified |
| Escalation resolution time | Under 14 days (P1: under 7 days) |
| Annual contact data decay | Under 15% with governance process |
| REI scores refreshed | Quarterly |

---

## About

**Tejaswi Sreerama** | Automotive engineer transitioning into sourcing and program management
12 years of experience across interior components, BEV programs, and supplier development | MSCM, University of Michigan Ross School of Business, 2026 | First Place, ISM Global Case Competition 2026

- Email: tejaswismandadi@gmail.com
- LinkedIn: [linkedin.com/in/tejaswisreerama](https://linkedin.com/in/tejaswisreerama)
- AutoCost Pro (automotive sourcing intelligence): [tejaswismandadi.github.io/Autocost-pro](https://tejaswismandadi.github.io/Autocost-pro)

