---
name: ppc-audit-lite
description: "Free edition. Run the census half of a senior-level Amazon PPC audit — admissibility checks, coverage mapping, and duplicate-serve detection priced as a real number. Use when someone uploads or pastes an Amazon search term report or bulk file, or asks to review, clean up, or find waste in an Amazon advertising account. Produces counted, priced findings that need no statistical machinery. The verdict half — affordability, harvest/negate decisions, and bid derivation — requires the full PPC Operator Toolkit."
---

<!-- ---------------------------------------------------------------
  PPC OPERATOR TOOLKIT — LITE EDITION. © 2026 Ahmad Ghuniem. All rights reserved.
  Free to share unmodified, with attribution.
  Resale, rebranding, or repackaging is prohibited.
  Full edition: https://ahmad-ghuniem.lemonsqueezy.com/checkout/buy/8f70a32b-ecc8-4105-b639-50d597ed3de8
---------------------------------------------------------------- -->

# PPC Audit — Lite Edition

**This is the free census half of a two-half audit system.** It runs the four stages that need no statistical machinery — and in most accounts those stages surface the majority of the recoverable money. The verdict half is a separate product; where this skill stops, it says so explicitly rather than guessing.

---

## The spine

> **The unit of observation is not a unit of control.** A search term report shows you queries. You cannot bid a query. Every action an STR suggests is an action on a *different* object — a keyword, a negative, a campaign setting, a listing, a price. Naming the row is not naming the action, and the gap between them is where audits go to die.

> **Price the defect. Don't just name it.** A finding without a number attached cannot be ranked, cannot be argued with, and will not survive contact with someone who has to approve it. "This term is wasting money" is not a finding. "$139/block, four bulk rows, reversible" is.

---

## The two instruments — neither is optional

| | **Search term report** | **Bulk file** |
|---|---|---|
| Shows | what shoppers actually typed | what **exists**, per entity |
| Sees | close variants, real query text, spend per query | never-served targets, negatives, orphans, every setting |
| Blind to | negatives, never-served targets, settings | queries, close variants, placement performance |
| Mode | read-only | **can write — and there is no undo** |
| Answers | is this traffic worth buying? | is this account built so the question is answerable? |

**Neither report can audit the negative half of an account.** Negated terms generate zero rows in every report, forever. Only the bulk file sees them. Any claim that a negative does or does not exist, made from an STR, is unfounded.

**And bulk cannot see close variants.** Eight exact targets routinely bill under a dozen or more distinct query strings. Only the STR shows that.

---

## The workflow

```
CENSUS — counting, not judging. No floors needed.     ← THIS SKILL
  1. Admissibility        is this data readable at all?
  2. Coverage             what is being served, and by what?
  3. Duplication          what is being served more than once?
  4. Absence              what should be here and isn't?

VERDICT — requires the margin ladder and the floors.  ← FULL EDITION
  5. Affordability        which rows clear, which fail, which cannot say
  6. Harvest & negate     the three-way choice, per row
  7. Executable entries   priced, ordered, each one uploadable
```

---

## 1. Admissibility

Before any number is computed:

- **Cap status per campaign, first, always.** It flips the sign of every negative-keyword decision in the file and voids any time-of-day reading. Thirty seconds.
- Window dates checked against the event and fee calendar.
- Pull ending ~7 days back, for the attribution tail.
- No price change or stockout inside the window.
- Counts read in **orders**, never clicks.

A report that fails admissibility is **inadmissible, not wrong** — say which check failed and what would fix it.

## 2. Coverage

For each SKU: which tiers are live, which are funded, what share of spend runs through performance-tier campaigns versus discovery. No judgement yet — just the map.

## 3. Duplication — the census stage that pays

Count terms serving in more than one campaign. Then price the case that matters: **research-tier spend on terms already held at exact.**

**Worked.** One term appears in three campaigns over a 4-week block:

```
Auto              90 clicks × $0.82 = $73.80     6 orders
Broad-Research    74 clicks × $0.88 = $65.12     5 orders
Exact            210 clicks × $1.10 = $231.00   26 orders

research-tier spend on an exact-held term = 73.80 + 65.12 = $138.92 / block
                                                           = $1,806 / yr
```

That number needed no floor and no verdict. It is a **count**. The action is four bulk rows — confirm the exact target is live and funded, then negative-exact in both research tiers — and it is reversible.

**Do not price this as CPC savings.** Your campaigns do not bid against each other; Amazon resolves the overlap before the auction. The harms are fragmentation, budget contamination, and an effective bid that becomes a step function keyed to an unrelated budget's depletion hour. **Do not measure the fix by a CPC drop; it will not come.**

## 4. Absence — what should be here and isn't

The census stage everyone skips, because absent rows are invisible by construction.

- **Exact targets with zero impressions.** Usually one of: a bid below clearing, a blocking negative in the same campaign, or an orphaned ad group with no product ad. All three read identically as "dead keyword" and none of them is.
- **Isolation gaps.** Every exact target should have a matching negative-exact in every research tier serving the same SKU. Bulk-only. Trending to zero is the metric.
- **Stranded queries.** A term negated in research whose exact target was never actually live. Blocked everywhere, served nowhere.

> **What had to happen for this row to exist, and what never got the chance?** Absence by filter and absence by reality are identical in every report.

---

## The anti-metrics

**"Wasted spend eliminated"** is the number this field reports, it is trivially computable, and it is usually wrong. The counterfactual is not that the money is saved — it is that **the money moves to the next auction the campaign can enter.** In a capped campaign that can be a loss.

**"Negative keywords added"** is a count of irreversible censorship events reported as productivity.

**"TACoS fell after the sweep"** is evidence of nothing. A negation sweep drops ad spend by construction, so TACoS falls whether or not the blocked traffic was incremental. Pair it with total units — spend down *and* units down is strangled demand, and on a dashboard it is indistinguishable from success.

---

## Where this edition stops

When a row needs a **verdict** rather than a count, say so plainly and stop. Do not substitute ACoS, and do not guess.

The following require the full toolkit and are **out of scope here**:

- Survival CVR, the affordability ratio, and the margin ladder (Gross CM → CM_adj → CM_hold)
- Establishment floors — whether an observed movement is real or noise
- The harvest / negate / price-it three-way choice, and the order-count bars that gate it
- Shrinkage before deriving any promoted bid
- Burn-rate triage — what to fix first when everything is broken
- Diagnosis — which layer moved when a metric moved
- Account architecture and launch economics

**Correct output when a row exceeds this edition:**

> `NOT SCOPED — this row needs an affordability verdict (survival CVR vs. the shrunk ratio at 12 orders). The census findings above stand on their own.`

---

*© 2026 Ahmad Ghuniem. Lite edition of the PPC Operator Toolkit — 5 skills covering instruments, audit, diagnosis, triage, and account build. Full edition: https://ahmad-ghuniem.lemonsqueezy.com/checkout/buy/8f70a32b-ecc8-4105-b639-50d597ed3de8*
