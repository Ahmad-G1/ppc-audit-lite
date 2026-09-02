# PPC Audit — Lite Edition

**A senior-level Amazon PPC audit, installable as a Claude Skill.**

Free edition. Runs the *census* half of a two-half audit system — the stages that need no statistical machinery, and that in most accounts surface the majority of the recoverable money.

---

## The problem this exists to fix

Your analyst pulls a search term report, sorts by spend, flags the expensive terms with no orders, and hands you a list.

The list is wrong. Not slightly — structurally.

Half those terms are statistical noise at 11 clicks. Negating them in a budget-capped campaign hands the money to *worse* traffic. The duplicate-serve leak actually costing $1,800/yr never appears, because it isn't a bad row — it's the same row in three campaigns. And the headline number reported back, "wasted spend eliminated," is an anti-metric that measures nothing.

---

## What this skill does

**Four census stages, in order:**

| Stage | Question |
|---|---|
| **Admissibility** | Is this data readable at all? (Cap status first — it flips the sign of every negative decision in the file.) |
| **Coverage** | What is being served, and by what? |
| **Duplication** | What is being served more than once — and what does that cost? |
| **Absence** | What should be here and isn't? |

**A real finding from stage 3**, computed with no floors and no verdict — it's a *count*:

```
One term, three campaigns, one 4-week block:

Auto              90 clicks × $0.82 = $73.80     6 orders
Broad-Research    74 clicks × $0.88 = $65.12     5 orders
Exact            210 clicks × $1.10 = $231.00   26 orders

research-tier spend on an exact-held term = $138.92 / block
                                          = $1,806 / yr

Action: 4 bulk rows. Reversible.
```

It will also tell you **not** to measure that fix by a CPC drop — your campaigns don't bid against each other, so the drop won't come, and calling that a failure is a mistake most operators make.

---

## What makes it different from a prompt pack

**It refuses to answer when it can't.** Below the evidence bar there is no verdict, not a small one. It says `NOT SCOPED` and names what would settle it.

**It names the anti-metrics** — "wasted spend eliminated," "negatives added," "TACoS fell after the sweep." Three numbers this industry reports that measure nothing.

**It knows what each report structurally cannot show.** Negatives are invisible in every STR, forever. Close variants are invisible in bulk. Claims from the wrong instrument are unfounded, and this won't make them.

---

## Install

**Claude.ai (web or desktop app):**
1. Settings → Capabilities → enable **Code execution and file creation** (skills need it)
2. Download **[ppc-audit-lite.zip](../../raw/main/ppc-audit-lite.zip)** from this repo
3. **Customize → Skills** → **+** → upload that zip → toggle it on

**Claude Code:**
```bash
git clone https://github.com/Ahmad-G1/ppc-audit-lite.git
mkdir -p ~/.claude/skills
cp -r ppc-audit-lite/ppc-audit-lite ~/.claude/skills/
```

Then paste or upload a search term report and ask for an audit. The skill triggers on its own.

---

## What's not in this edition

The census half is free. The **verdict** half is the paid toolkit:

- Survival CVR, the affordability ratio, and the margin ladder (Gross CM → CM_adj → CM_hold)
- Establishment floors — whether a movement is real or noise
- The harvest / negate / price-it three-way choice and the order-count bars gating it
- Shrinkage before deriving any promoted bid
- Burn-rate triage — what to fix first when everything is broken
- Diagnosis — which layer moved when a metric moved
- Account architecture and launch economics

**→ [Full PPC Operator Toolkit — 5 skills, 6 reference modules, full methodology PDF](https://ahmad-ghuniem.lemonsqueezy.com/checkout/buy/8f70a32b-ecc8-4105-b639-50d597ed3de8)**

---

## License

Free to share unmodified, with attribution. Resale, rebranding, or repackaging prohibited. See [LICENSE](LICENSE).

© 2026 Ahmad Ghuniem
