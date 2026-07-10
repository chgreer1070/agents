---
name: ems-contract-playbook
description: Clause-level negotiation playbook for EMS and contract manufacturing agreements covering demand flexibility, inventory liability, pricing mechanics, liability architecture, IP, and exit. Use when drafting, reviewing, or negotiating manufacturing services agreements, supply agreements, or SOWs.
---

# EMS Contract Playbook

Clause-by-clause negotiation playbook for electronics manufacturing services (EMS) and contract manufacturing agreements, from both the customer (OEM) and manufacturer sides.

## When to Use This Skill

- Drafting or reviewing a manufacturing services agreement (MSA) or supply agreement
- Negotiating forecast, flexibility, or inventory liability terms
- Structuring pricing, cost-down, and PPV mechanics
- Designing liability caps, warranty, and epidemic failure provisions
- Planning termination, transition, and second-source rights

## Core Concepts

### 1. The Five Value-Bearing Clause Clusters

| Cluster | What It Really Controls | Typical Value at Stake |
| ------- | ----------------------- | ---------------------- |
| **Demand & Flexibility** | Who eats volume volatility | 1–3% of annual spend |
| **Inventory & E&O Liability** | Working capital and write-off risk | 4–12 weeks of material cost |
| **Pricing Mechanics** | Margin over the contract life | 50–300 bps of margin |
| **Liability Architecture** | Catastrophic loss allocation | Cap multiple × annual revenue |
| **Term, Exit & Transition** | Switching costs and leverage at renewal | 6–18 months of disengagement cost |

### 2. Demand & Flexibility Framework

```
Forecast Horizon:
├── Firm zone (0–4 wks):     PO-backed, 0% reduction, reschedule fees
├── Flex zone (5–13 wks):    ±20–30% quantity flexibility bands
├── Material zone (14–26 wks): Authorization for long-lead buys only
└── Planning zone (27+ wks): Non-binding, capacity planning only
```

Key negotiation points:

- **Upside flexibility**: commit the manufacturer to defined upside (e.g., +25% within 4 weeks) or it is best-efforts only
- **Reschedule rights**: number of pushes allowed per PO before it converts to cancellation liability
- **Cancellation ladder**: liability should decay with distance from delivery date, not be flat
- **Long-lead-time (LLT) authorization**: separate written authorization for components beyond the material window; never blanket authority

### 3. Inventory & E&O Liability

- Liability should attach only to **demand-driven procurement** consistent with the flexibility framework and MOQ/lot-size realities
- Require **mitigation duties** before invoicing: return-to-vendor, reallocation to other customers/programs, scrap credit
- Set an **aging and reporting cadence** (e.g., quarterly E&O report, claims expire if not raised within 2 quarters)
- Cap **MOQ-driven overbuy** exposure or require pre-approval above thresholds
- Distinguish obsolescence caused by **customer ECN** (customer liability) vs. **manufacturer process change** (manufacturer liability)

### 4. Pricing Mechanics

- **Cost model transparency**: BOM cost, value-add, and margin visible separately; audit rights on pass-through components
- **PPV allocation**: define who keeps purchase price variance — favorite exploit of whichever side controls procurement
- **Cost-down sharing**: scheduled productivity commitments (e.g., 2–4%/yr) plus 50/50 sharing of engineered savings
- **Index/pass-through triggers**: commodity, FX, tariff, and freight adjustments with symmetric triggers (both directions), defined indices, and re-pricing cadence
- **MFC clauses**: resist most-favored-customer language; if unavoidable, narrow to comparable volume/mix/geography and self-certification

### 5. Liability Architecture

```
Liability Stack:
├── Warranty (workmanship): 12–36 months, repair/replace remedy
├── Epidemic failure: defined trigger (e.g., >2% same root cause
│   within 6 months), expanded remedy incl. recall logistics
├── IP indemnity: uncapped or super-cap, control of defense
├── General cap: 12–24 months of fees/revenue under the agreement
└── Carve-outs: IP infringement, confidentiality, willful misconduct,
    bodily injury — negotiate hard on whether recall costs sit
    inside or outside the cap
```

- Consequential damages waivers: ensure defined direct damages (rework, recall, cover purchases) are expressly **not** excluded
- Match insurance requirements (product liability, recall) to the cap structure

### 6. Term, Exit & Transition

- **Termination for convenience**: notice period priced against inventory liability tail; the real cost is the wind-down formula
- **Transition assistance**: obligated cooperation, test/tooling transfer, and last-time-buy rights survive termination for cause in either direction
- **Tooling & NRE**: customer-paid tooling is customer-owned, with possession/return mechanics and no manufacturer lien
- **Technology escrow / second source**: manufacturing documentation package deliverable on defined triggers
- **Data & IP return**: defined package (test scripts, fixtures, AVL, process docs) with a delivery deadline

## Common Exploits by Opposing Counsel

- Order-of-precedence conflicts between MSA, SOW, PO terms, and quality agreement
- "Course of dealing" arguments built on informal forecast emails that bypass flexibility bands
- Undefined "commercially reasonable efforts" in supply assurance clauses
- Notice provisions with short claim windows silently extinguishing E&O or warranty claims
- Battle-of-the-forms via PO acknowledgment terms reintroducing rejected language

## Output Checklist

- Clause redlines with rationale per change
- Flexibility/liability matrix quantified against actual demand volatility
- Liability stack diagram with cap adequacy check vs. realistic loss scenarios
- Exit cost model (transition timeline, LTB exposure, requalification cost)
- Negotiation posture: open, fallback, walk-away, and required reciprocity per concession
