# Questions for NISSS — Gig Worker Prototype

**Purpose:** This prototype is ready for user testing, but several screens show placeholder text marked *"to be confirmed with NISSS."* This list separates what we already know (from the research report and the Ann-Marie King discovery session) from what still needs NISSS sign-off.

**Status key:** 🔴 **Open** — must ask NISSS · 🟡 **Partial** — exists but the number/detail is missing · 🟢 **Answered** — confirmed in the research, no need to ask (listed at the end for reference).

**File:** `index.html` — line references point to the exact text each answer will update.

---

## 🔴 Open — the real gaps (please answer in writing)

These block the placeholders and unverified facts in the prototype.

| # | Question | Updates | Why it's open |
|---|----------|---------|---------------|
| 1 | How is each benefit calculated for the self-employed — a % of declared/average earnings, or purely from the number of contributions? | Plan screen logic | Report's **#1 open question** and **#1 escalated risk**: "showing a wrong number is worse than no number." Must come from NISSS, not our reading of regulations. |
| 2 | **Old age pension:** confirm the "10 best years" formula and the minimum contributions to qualify. | Line 828 | From the discovery session, not the report — needs written confirmation. |
| 3 | **Sickness, maternity, paternity, invalidity, survivors:** payment rate and duration for each. | Lines 818–826 | Calculation logic explicitly not provided. |
| 5 | Are there **minimum and maximum** benefit figures we can show as a realistic range? | Plan screen | Not provided. |
| 9 | Confirm benefits begin after **one full year** of contributions. Does the qualifying period differ by benefit (pension vs sickness)? | Line 956 | From the discovery session, not the report. |
| 13 | Is there **any cross-reporting to the BRA** (tax) we must disclose, or is NISSS genuinely separate? | Trust messaging across flow | Report only frames NIS as *not* a tax; doesn't address data-sharing. |
| 15 | What documents does a **new** vs. **existing** NISSS-number holder need to register? | Lines 1130–1138 | Not addressed. |
| 16 | How are benefits **paid out** (bank transfer, cheque)? Can members see their contribution history today, or is that future? | `screenTracker` (line 1391) | Payment-*in* channels known; payout method and history-view are not. Confirms whether the tracker is "future." |
| 17 | Does policy distinguish **"gig worker" from "self-employed"** operationally, or is the "contract for services" definition sufficient? | Worker-type screen (line 516) | The report's own open question — worth resolving for segmentation. |

---

## 🟡 Partial — exists, but we need the number or detail

| # | Question | Updates | What we already know |
|---|----------|---------|----------------------|
| 4 | What is the **funeral grant** amount for the self-employed? | Plan screen (funeral grant card) | Confirmed it *exists* (Participant 1 saw NIS pay toward funerals); amount unknown. |
| 6 | What is the **contribution rate above the floor** — a fixed % of declared earnings? | `screenPlan` tier definitions | Floor confirmed ($1,200/yr ≈ **$23/week**); rate for higher tiers not given. |
| 11 | The **grant pathway:** what grant does someone get instead of a full benefit, and what triggers it? | Line 1202 | Confirmed for over-50s ("may still qualify for a grant"); trigger/amount unspecified. |
| 12 | Confirm which benefits are **operational today** vs. planned. | `screenBenefitsQuick` (line 975) | Report lists exactly **five payouts** and excludes employer reporting (Moore Resolution not yet law) — matches the prototype; just needs explicit confirmation. |
| 14 | Confirm the **Frank Walcott Building** address and phone **246-431-7400**. | Lines 1173–1175 | Online at **nis.gov.bb** and **SurePay/EZpay+** confirmed; the specific address and number are *not* in the report and need verifying. |
| 18 | Is the **5% retroactive surcharge waivable** for a limited promotional window? | Lines 1195, 1271, 1539 | The report flags this is sitting with the Minister — if approved, it changes the registration-guide copy. |

---

## 🟢 Answered by the research — no need to ask (for reference)

- **$1,200/year minimum**, equal to **$23/week** — confirmed; use directly in the tier slider.
- **How to pay irregular income** — Ann-Marie's **Adaptive Contribution Model**: weekly, monthly, lump sums, or catch up by **15 January**. NISSS already permits this.
- **3-year back-pay with 5% surcharge per missed year** — confirmed (whether it's waivable is Q18 above).
- **Registration is already online at nis.gov.bb** — we link out rather than rebuild it; payment via **SurePay / EZpay+**.
- **"You don't have to register a business to register for NIS"** — confirmed; a key misconception to correct.

---

*Prototype is not connected to real NISSS systems and stores no personal data. Figures shown are illustrative until confirmed.*
