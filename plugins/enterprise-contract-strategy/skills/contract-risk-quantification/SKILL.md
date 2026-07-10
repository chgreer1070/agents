---
name: contract-risk-quantification
description: Quantify the financial impact of contract terms — working capital, margin, liability exposure, and expected monetary value of risk allocations. Use when pricing concessions, sizing liability caps, evaluating payment terms, or building a negotiation trade-off model.
---

# Contract Risk Quantification

Methods for putting numbers on contract terms so negotiations trade quantified value instead of adjectives.

## When to Use This Skill

- Sizing a liability cap or insurance requirement against realistic loss scenarios
- Pricing a payment-term change in working capital dollars
- Valuing flexibility bands and cancellation windows against demand volatility
- Building a concession trade-off model before a negotiation round
- Estimating litigation/dispute exposure for reserves or deal decisions

## Core Concepts

### 1. Working Capital Math

```
Payment terms value  = (ΔDPO days / 365) × annual spend × WACC
Inventory carry cost = avg inventory × (WACC + storage + obsolescence %)
Cash conversion      = DIO + DSO − DPO
```

Example: moving $200M annual spend from Net 45 to Net 75 at 9% WACC:
`(30/365) × $200M × 9% ≈ $1.48M/yr` — that is the price of the term, and what the counterparty will load into pricing.

### 2. Expected Monetary Value (EMV) of Risk Terms

```
EMV = Σ (probability of scenario × loss given scenario)
```

- Build P10 / P50 / P90 loss scenarios per risk (quality escape, E&O write-off, supply disruption, IP claim)
- Compare EMV against the cost of contractual protection (cap carve-out, insurance premium, price adder)
- A term is worth conceding when the price extracted exceeds the EMV retained

### 3. E&O Exposure Model

```
Exposure = Σ over BOM of:
  (authorized weeks of demand × weekly unit cost)
  × (1 − recovery rate)      # RTV, reallocation, scrap credit
  × P(demand shortfall)
```

Stress against: historical forecast error (MAPE), product end-of-life scenarios, and MOQ-driven overbuy on the top-20 value components (usually >80% of exposure).

### 4. Liability Cap Adequacy

| Loss Scenario | Model As |
| ------------- | -------- |
| Field failure / recall | Units in field × failure rate × per-unit remedy cost + logistics + requalification |
| Line-down (customer's) | Customer's daily margin loss × outage days — check if consequential waiver excludes it |
| Epidemic failure | Trigger % × install base × expanded remedy |
| IP infringement | Design-around cost vs. royalty vs. injunction (revenue at risk) |

Rule of thumb: a cap below P90 single-event loss is a retained risk decision — make it explicitly, price it, and note it in the risk register.

### 5. Margin Impact of Pricing Mechanics

- Cost-down commitments: `Σ (committed %/yr × spend)` over term, discounted
- Asymmetric pass-through (up-only indexation): value the embedded option using historical index volatility
- PPV retention: historical PPV as % of BOM × who keeps it
- MFC clause: probability-weighted margin compression across the affected portfolio, not just this deal

### 6. Negotiation Trade-off Table

Convert every open item into a common currency ($/yr or NPV) before the round:

| Open Term | Our Cost to Concede | Their Cost to Concede | Trade Candidate |
| --------- | ------------------- | --------------------- | --------------- |
| Net 75 → Net 60 | +$740K/yr | −$740K/yr | vs. 15% upside flex commitment |
| Cap 12mo → 24mo fees | EMV +$X | premium/pricing +$Y | vs. epidemic failure carve-in |

Trade across categories (a legal term for a commercial term) — that is where positive-sum exchanges hide.

## Best Practices

- State every assumption inline; a wrong-but-visible assumption is fixable, a hidden one is not
- Use ranges (P10/P50/P90), not point estimates, for anything driven by demand or failure rates
- Quantify the do-nothing baseline — status-quo terms have a cost too
- Sanity-check outputs against financial statements (a computed exposure larger than the counterparty's equity means the real remedy is diversification, not drafting)

## Output

- One-page exposure summary: top 5 quantified risks with EMV and mitigation
- Trade-off table in common currency for the negotiation team
- Cap adequacy check with explicit retained-risk statements
- Sensitivity notes: which two assumptions move the answer most
