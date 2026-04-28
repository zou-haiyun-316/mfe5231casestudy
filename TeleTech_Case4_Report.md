# MFE 5231 Case Study Report
## Case 4: TeleTech Corporation, 2005
### Risk-Adjusted Hurdle Rates and Value Creation

**Group 4:** Rangxila GONG | Huihui LIU | Yin PANG | Haiyun ZOU  
**Course:** MFE 5231 Financial Management, 2nd Term 2025-2026, CUHK(Shenzhen)  
**Instructor:** Prof. Joseph Cheng

---

## Executive Summary

TeleTech Corporation operates two distinct business segments—**Telecommunications Services** and **Products & Systems (P&S)**—but applies a single corporate hurdle rate of **9.30%** to all capital allocation decisions. This report demonstrates that this practice is financially incorrect and leads to systematic value misallocation.

Using the unlever-relever beta methodology and CAPM, with comparable companies drawn directly from **Exhibit 3** of the case, we estimate that the **Telecommunications Services** segment has a true risk-adjusted WACC of approximately **8.53%**, while **Products & Systems** carries a far higher WACC of approximately **11.22%**, reflecting its substantially greater business risk.

Against these benchmarks, our Economic Value Added (EVA) analysis—using the 2004 ROC figures stated explicitly in the case (Telecom: 9.10%; P&S: 11.00%) and book-value invested capital from the case—reveals:

- Telecom Services **creates** approximately **$65.5 million** of value per year (ROC 9.10% > WACC 8.53%)
- Products & Systems **destroys** approximately **$10.0 million** per year (ROC 11.00% < WACC 11.22%)
- Net firm EVA = **+$55.5 million/year**

We recommend that TeleTech immediately adopt risk-adjusted hurdle rates by segment and conduct a strategic review of P&S capital deployment.

---

## 1. Company Background and the Core Problem

### 1.1 TeleTech's Two Segments

TeleTech Corporation is a large regional telecommunications firm headquartered in Dallas, Texas. It defines itself as a "provider of integrated information movement and management" and has two main business segments:

| Feature | Telecom Services | Products & Systems |
|---|---|---|
| Nature | Regulated, utility-like | Technology manufacturing |
| 2004 Revenues | $11.0 billion | Approx. $5.5 billion |
| 2004 NOPAT | $1.18 billion (given) | $480 million (given) |
| 2004 Capital (book) | $11.4 billion (given) | $4.6 billion (given) |
| **2004 ROC** | **9.10%** (given in case) | **11.00%** (given in case) |
| Current Hurdle Rate | 9.30% (corporate-wide) | 9.30% (corporate-wide) |

*Source: Case text, page 2. ROC = NOPAT / Capital (Net Assets).*

### 1.2 The Fundamental Problem

TeleTech's current practice is to evaluate **all** investment projects across both segments using a single corporate hurdle rate of **9.30%**, derived from the blended cost of capital of the entire firm (Exhibit 1 of the case).

The problem: a blended rate implicitly treats all segments as equally risky—a flawed assumption given the stark differences between regulated telecommunications and competitive technology manufacturing.

**The result is a "cross-subsidy" mechanism:**

- The low-risk Telecom segment faces an **artificially high** hurdle rate (9.30% vs. true WACC of ~8.53%), causing value-creating projects to be rejected.
- The high-risk P&S segment faces an **artificially low** hurdle rate (9.30% vs. true WACC of ~11.22%), allowing value-destroying projects to be approved.

---

## 2. Estimating Segment WACC (Question b)

### 2.1 Methodology

We follow the three-step unlever-relever beta methodology:

```
Step 1: Identify comparable pure-play firms from Exhibit 3
Step 2: Unlever each comparable's equity beta to remove financial risk
Step 3: Average unlevered betas → Re-lever using segment's target capital structure
Step 4: Apply CAPM to get Cost of Equity
Step 5: Weight Cost of Equity and after-tax Cost of Debt → WACC
```

**Key Parameters (from Exhibit 1 and Exhibit 4 of the case):**

| Parameter | Value | Source |
|---|---|---|
| Risk-free rate (r_f) | **4.62%** | 30-year U.S. Treasury yield, Exhibit 4 |
| Market Risk Premium (MRP) | **5.50%** | Exhibit 1 (R_M − R_f = 10.12% − 4.62%) |
| Marginal Tax Rate (t) | **40%** | Case text, Exhibit 1 |

**Beta Adjustment Formulas:**

$$\beta_U = \frac{\beta_L}{1 + (1-t) \times \frac{D}{E}} \quad \text{[Unlever: strip out financial risk]}$$

$$\beta_L^{*} = \beta_U \times \left[1 + (1-t) \times \frac{D}{E}^{*}\right] \quad \text{[Re-lever: apply segment target structure]}$$

Where D/V and E/V weights are measured at **market value** (from the "Mkt Val Debt/Capital" column in Exhibit 3).

---

### 2.2 Telecom Services Segment

#### Step 1 & 2: Comparable Companies — Unlever Beta

We select the six investment-grade, regulated telecom carriers from the **Telecommunications Services Industry** in Exhibit 3. We exclude AT&T Corp. (BB+, deeply negative P/E, financially distressed) and IDT Corp. (no bond rating, D/V only 2.1%, atypical capital structure).

| Company | β_L | D/V (MV) | E/V | D/E | β_U |
|---|---|---|---|---|---|
| Alltel Corp | 1.00 | 23.2% | 76.8% | 0.3021 | **0.8466** |
| BellSouth Corp | 1.00 | 22.9% | 77.1% | 0.2970 | **0.8487** |
| Centurytel Corp | 1.05 | 37.0% | 63.0% | 0.5873 | **0.7764** |
| SBC Communications | 1.05 | 20.0% | 80.0% | 0.2500 | **0.9130** |
| Sprint Corp | 1.15 | 30.3% | 69.7% | 0.4347 | **0.9121** |
| Verizon Communications | 1.00 | 24.1% | 75.9% | 0.3175 | **0.8400** |
| **Average** | **1.042** | **26.25%** | **73.75%** | **0.3559** | **0.8561** |

**Sample Calculation (Alltel):**
$$\beta_U^{Alltel} = \frac{1.00}{1 + 0.60 \times 0.3021} = \frac{1.00}{1.1813} = 0.8466$$

#### Step 3: Re-lever Beta for Telecom Segment

Target capital structure = average of comparables: **D/V = 26.25%, E/V = 73.75%, D/E = 0.3559**

$$\beta_L^{Telecom} = 0.8561 \times (1 + 0.60 \times 0.3559) = 0.8561 \times 1.2135 = \mathbf{1.039}$$

#### Step 4: Cost of Equity (CAPM)

$$r_e^{Telecom} = 4.62\% + 1.039 \times 5.50\% = 4.62\% + 5.71\% = \mathbf{10.33\%}$$

#### Step 5: WACC for Telecom Services

Pre-tax cost of debt: **5.74%** (A-rated bond yield, from Exhibit 1 Telecom column and Exhibit 4)

$$WACC_{Telecom} = 0.7375 \times 10.33\% + 0.2625 \times 5.74\% \times (1-0.40)$$

$$= 7.62\% + 0.90\% = \mathbf{8.53\%}$$

---

### 2.3 Products & Systems Segment

#### Step 1 & 2: Comparable Companies — Unlever Beta

P&S is a technology manufacturing business (computing + telecom equipment). We use the **Telecommunications Equipment Industry** and **Computer and Network Equipment Industry** companies from Exhibit 3. We exclude Lucent Technologies (B-rated, book D/E = 109.8%, severely distressed; atypical beta) and Gateway Inc. (negative earnings, not representative).

| Company | β_L | D/V (MV) | E/V | β_U |
|---|---|---|---|---|
| Avaya Inc | 1.35 | 4.4% | 95.6% | **1.3137** |
| Belden CDT Inc | 1.45 | 17.5% | 82.5% | **1.2863** |
| Commscope Inc | 1.10 | 22.4% | 77.6% | **0.9376** |
| Corning Inc | 1.45 | 11.8% | 88.2% | **1.3423** |
| Harris Corp | 1.05 | 10.7% | 89.3% | **0.9796** |
| Nortel Networks | 1.75 | 20.7% | 79.3% | **1.5130** |
| Plantronics Inc | 1.20 | 0.2% | 99.8% | **1.1986** |
| Scientific-Atlanta | 1.45 | 0.1% | 99.9% | **1.4491** |
| EMC Corp | 1.55 | 0.4% | 99.6% | **1.5463** |
| Hewlett-Packard | 1.45 | 7.8% | 92.2% | **1.3800** |
| IBM | 1.10 | 8.4% | 91.6% | **1.0426** |
| Lexmark Int'l | 1.15 | 1.4% | 98.6% | **1.1403** |
| NCR Corp | 1.20 | 4.5% | 95.5% | **1.1670** |
| Seagate Technology | 1.20 | 10.0% | 90.0% | **1.1250** |
| **Average** | **1.336** | **8.59%** | **91.41%** | **1.2444** |

**Sample Calculation (Corning):**
$$\beta_U^{Corning} = \frac{1.45}{1 + 0.60 \times \frac{0.118}{0.882}} = \frac{1.45}{1 + 0.60 \times 0.1338} = \frac{1.45}{1.0803} = 1.3423$$

#### Step 3: Re-lever Beta for P&S Segment

Target capital structure = average of comparables: **D/V = 8.59%, E/V = 91.41%, D/E = 0.0940**

$$\beta_L^{P\&S} = 1.2444 \times (1 + 0.60 \times 0.0940) = 1.2444 \times 1.0564 = \mathbf{1.315}$$

#### Step 4: Cost of Equity (CAPM)

$$r_e^{P\&S} = 4.62\% + 1.315 \times 5.50\% = 4.62\% + 7.23\% = \mathbf{11.85\%}$$

#### Step 5: WACC for P&S Segment

Pre-tax cost of debt: **7.47%** (BB-rated bond yield from Exhibit 1 and Exhibit 4)

$$WACC_{P\&S} = 0.9141 \times 11.85\% + 0.0859 \times 7.47\% \times (1-0.40)$$

$$= 10.83\% + 0.39\% = \mathbf{11.22\%}$$

---

### 2.4 Summary: Corporate vs. Segment WACCs

| Metric | Telecom Services | Products & Systems | Corporate (given) |
|---|---|---|---|
| # Comparables used | 6 | 14 | — |
| Avg. Unlevered Beta (β_U) | **0.8561** | **1.2444** | — |
| Re-levered Beta (β_L) | **1.039** | **1.315** | 1.15 |
| Cost of Equity (r_e) | **10.33%** | **11.85%** | 10.95% |
| Cost of Debt (pre-tax) | 5.74% (A) | 7.47% (BB) | 5.88% (A−/BBB+) |
| After-tax Cost of Debt | 3.44% | 4.48% | 3.53% |
| E/V Weight | **73.75%** | **91.41%** | 77.8% |
| D/V Weight | **26.25%** | **8.59%** | 22.2% |
| **WACC** | **8.53%** | **11.22%** | **9.30%** |
| **ROC (2004, case given)** | **9.10%** | **11.00%** | ~9.58% |
| **Spread (ROC − WACC)** | **+0.57%** | **−0.22%** | +0.28% |

**Key Insight:** The corporate-blended WACC of 9.30% masks value destruction in P&S (ROC 11.00% < WACC 11.22%) while simultaneously overstating the hurdle for Telecom (ROC 9.10% > WACC 8.53%). Under the single-rate system, Telecom appears barely profitable (+0.57% is correct but understated in impact) while P&S appears profitable at the corporate rate (+1.70% spread at 9.30% — misleadingly positive).

> **Sanity check:** The case states prospective ROC ≈ 9.58%. Our segment-weighted WACC: 0.75 × 8.53% + 0.25 × 11.22% = 6.40% + 2.81% = **9.21%** ≈ the case's stated 9.30% corporate WACC. This confirms our segment WACC estimates are internally consistent.

---

## 3. Constant vs. Risk-Adjusted Hurdle Rates (Question a)

### 3.1 The Decision Errors Created by a Uniform Rate

Using the **Security Market Line (SML)** framework, there are two systematic error types:

```
Expected Return
     │
12%  │                           
     │       P&S true WACC = 11.22%  ─────────────────────────────────
11%  │ ─────────────────────────────────────────────────────── P&S ROC = 11.00%
     │
10%  │       Telecom ROC = 9.10%  ──────────────────────────
     │       Corp hurdle = 9.30%  ──────────────────────────
 9%  │       
     │
8.5% │  Telecom true WACC = 8.53%  ────────────────────────
     │
     └──────────────────────────────────────────────────────────
                    Telecom                    P&S
                 (Low Risk: β=1.04)       (High Risk: β=1.32)
```

**Systematic Decision Errors under Uniform Hurdle Rate (9.30%):**

| Scenario | What uniform rate says | What risk-adjusted rate says | Error Type |
|---|---|---|---|
| Telecom project, IRR = 9.00% | REJECT (9.00% < 9.30%) | ACCEPT (9.00% > 8.53%) | Type I: Reject good projects |
| Telecom project, IRR = 8.80% | REJECT | ACCEPT (8.80% > 8.53%) | Type I: Reject good projects |
| P&S project, IRR = 10.50% | ACCEPT (10.50% > 9.30%) | REJECT (10.50% < 11.22%) | Type II: Accept bad projects |
| P&S project, IRR = 9.50% | ACCEPT | REJECT | Type II: Accept bad projects |

### 3.2 The Critical Illusion: P&S Appears Profitable Under the Uniform Rate

Under the **9.30% uniform hurdle rate**, P&S earns a "spread" of +1.70% (ROC 11.00% − hurdle 9.30%). Management would conclude: **P&S is creating value.** This is Victor Yossarian's entire point—management is wrong.

Under **risk-adjusted rates**, the truth is reversed: P&S spread = 11.00% − 11.22% = **−0.22%**. P&S is **destroying** shareholder value.

This is exactly Rick Phillips's argument from the case text: the uniform rate creates a false sense of security in the high-risk segment while unfairly penalizing the safe segment.

### 3.3 Four Capital Allocation Distortions

**Distortion 1 — Capital Over-allocation to P&S:**  
P&S projects with returns between 9.30% and 11.22% will be approved under the uniform rate but are actually destroying value.

**Distortion 2 — Capital Under-allocation to Telecom:**  
Telecom projects with returns between 8.53% and 9.30% will be rejected even though they create value. This misallocated zone spans 0.77 percentage points.

**Distortion 3 — Flawed Strategic Signaling:**  
Under uniform rate: Telecom appears modest (+0.57% apparent spread from our analysis, but +1.70% would be the corporate hurdle comparison if ROC > 9.30% — actually Telecom ROC 9.10% < corporate 9.30%, so Telecom looks like a *loser* under the corporate rate). Under risk-adjusted rates: Telecom creates genuine value (+0.57% spread). The corporate hurdle produces exactly the wrong strategic signal.

**Distortion 4 — Managerial Incentive Misalignment:**  
P&S managers evaluated at 9.30% have an easy benchmark—their actual required rate (11.22%) is nearly 2 percentage points higher.

---

## 4. Has P&S Destroyed Value? Should TeleTech Implement Risk-Adjusted Rates? (Question c)

### 4.1 Economic Value Added (EVA) Analysis

$$EVA = (ROC - WACC_{segment}) \times Invested\ Capital\ (Book)$$

**Invested Capital from Case Text (Book Value of Net Assets, 2004):**

| Segment | Book Capital | Source |
|---|---|---|
| Telecom Services | **$11.4 billion** | Case text, page 2 |
| Products & Systems | **$4.6 billion** | Case text, page 2 |
| Total | **$16.0 billion** | — |

**EVA Calculation:**

| Segment | ROC | Segment WACC | Spread | Invested Capital | Annual EVA |
|---|---|---|---|---|---|
| Telecom Services | 9.10% | 8.53% | **+0.57%** | $11,400M | **+$65.5M** |
| Products & Systems | 11.00% | 11.22% | **−0.22%** | $4,600M | **−$10.0M** |
| **Total (net)** | | | | **$16,000M** | **+$55.5M** |

### 4.2 Has Products & Systems Destroyed Value?

**Yes — under risk-adjusted hurdle rates, P&S has been destroying shareholder value.**

The magnitude is approximately **$10.0 million per year** — smaller than Yossarian implies, but the directional conclusion is clear: P&S earns less than its risk-adjusted cost of capital.

**The uniform-rate illusion:** Under the corporate 9.30% hurdle, P&S appears to be creating value (+1.70% spread). This is precisely the error that Yossarian is trying to expose. The risk-adjusted analysis shows that once we account for P&S's higher systematic risk (β = 1.32 vs. Telecom's 1.04), the apparent value creation evaporates.

**Telecom Services:** Creates **$65.5M** of value annually — a solid positive spread driven by stable regulated cash flows that more than compensate shareholders for their risk.

**Net verdict:** The firm as a whole creates **+$55.5M** of net economic profit per year, but this is entirely driven by Telecom, with P&S acting as a drag.

### 4.3 Should TeleTech Implement Risk-Adjusted Hurdle Rates?

**Our recommendation: Yes, implement immediately.**

The financial case:
- Chapter 14 (Cost of Capital): WACC must reflect the true risk of the specific division, not a blended firm average
- Chapter 11 (Capital Budgeting): Using the wrong discount rate produces systematic NPV errors
- The EVA analysis confirms P&S is destroying value while Telecom creates it

Implementing risk-adjusted rates would:
1. Stop approvals of P&S projects that appear value-creating at 9.30% but are actually destroying value at 11.22%
2. Unlock Telecom projects with returns between 8.53% and 9.30% that are currently rejected
3. Send correct strategic signals about each segment's true economic performance

---

## 5. Barriers to Implementation (Question d)

### 5.1 Organizational and Political Resistance

The most immediate barrier is internal politics. Under a 9.30% uniform rate, P&S appears to be the star performer (ROC 11.00% >> hurdle 9.30%). Implementing risk-adjusted rates would reverse this: P&S suddenly becomes a value destroyer, facing a 11.22% hurdle it cannot clear.

- P&S leadership (Helen Buono in the case) will lobby against adoption
- Board members may resist conclusions that imply prior capital allocation decisions were wrong
- The shift could trigger demands for segment divestitures or management changes

### 5.2 Technical and Analytical Challenges

**Beta estimation instability:** Betas change over time, and the choice of estimation window, frequency, and index affects results significantly. Our P&S β_U of 1.2444 could plausibly range from 1.0 to 1.5 across reasonable methodological choices, implying a P&S WACC range of roughly 10%–14%.

**Comparable company selection subjectivity:** With 23 companies in Exhibit 3, different analysts would make different inclusion/exclusion decisions. We excluded Lucent and Gateway as outliers, but others might include them, shifting results materially.

**Corporate-level debt allocation:** TeleTech does not issue separate segment bonds — all debt is raised at the corporate level. Allocating the corporate bond rating and associated costs to individual segments requires judgment about how financial risk is attributed.

**Segment interdependencies:** TeleTech's strategy is explicitly to integrate telecom services and computing technology. Clean segment separation may not capture the cross-segment value of their combined platform.

### 5.3 Incentive and Compensation Misalignment

If compensation systems are not updated simultaneously, the new hurdle rate will have no behavioral impact. Managers evaluated on old metrics will make old decisions.

Moreover, a higher P&S hurdle creates short-termism risk: managers may cut long-term R&D investment to meet the ROIC benchmark, even if those R&D projects have positive long-run NPV.

### 5.4 Organizational Learning and Change Management

- **Education:** Every finance team and project sponsor needs to understand why different segments face different hurdles — and why this is fair, not punitive
- **System updates:** Capital budgeting models, approval workflows, and dashboards must be recalibrated
- **Ongoing recalibration:** Unlike a single corporate rate, segment WACCs require annual review as comparable firms' betas and capital structures change
- **External communication:** Investors and analysts need to understand the new performance measurement framework

---

## 6. Conclusion and Recommendations

### 6.1 Summary of Findings

| Question | Key Finding |
|---|---|
| **a. Hurdle Rate Choice** | Uniform 9.30% creates systematic errors; P&S appears profitable (+1.70% spread) when it is actually destroying value (−0.22% risk-adjusted spread) |
| **b. Segment WACC** | Telecom Services: **8.53%** | Products & Systems: **11.22%** (vs. blended 9.30%) |
| **c. Value Creation** | P&S destroys **$10.0M/year**; Telecom creates **$65.5M/year**; firm net EVA = **+$55.5M/yr** |
| **d. Barriers** | Political resistance, beta/comparables subjectivity, incentive misalignment, organizational change costs |

### 6.2 Action Plan

| Priority | Recommendation | Timeline |
|---|---|---|
| **Immediate** | Adopt risk-adjusted hurdle rates: Telecom 8.53%, P&S 11.22% | Q1 2006 |
| **Short-term** | Recalibrate manager compensation to EVA benchmarks using segment WACCs | Q2 2006 |
| **Medium-term** | Strategic review of P&S: restructure, divest non-core units, or set explicit ROIC turnaround targets | 2006 |
| **Ongoing** | Annual update of segment betas using Exhibit 3-style comparable analysis | Annual |

### 6.3 Response to Victor Yossarian

Yossarian is **directionally correct**: the uniform hurdle rate does distort capital allocation and P&S is destroying value on a risk-adjusted basis. However, his recommendation to sell P&S entirely may be premature: P&S ROC (11.00%) is very close to its WACC (11.22%), and strategic synergies with Telecom may justify continuing operations while aggressively improving ROIC.

TeleTech's best response to Yossarian is to:
1. Acknowledge the analytical validity of segment-specific hurdle rates
2. Adopt risk-adjusted WACCs immediately
3. Set a 12-month ROIC improvement target for P&S with management accountability
4. Demonstrate to shareholders that the firm's capital allocation framework now correctly measures and incentivizes value creation

---

## Appendix A: WACC Calculation Detail

### A.1 Formula Reference

| Formula | Expression | Source |
|---|---|---|
| CAPM | $r_e = r_f + \beta_L \times MRP$ | Chapter 14 |
| Unlever Beta | $\beta_U = \beta_L / [1 + (1-t)(D/E)]$ | Course Notes |
| Re-lever Beta | $\beta_L^* = \beta_U \times [1 + (1-t)(D/E)^*]$ | Course Notes |
| WACC | $WACC = (E/V) r_e + (D/V) r_d (1-t)$ | Chapter 14 |
| EVA | $EVA = (ROC - WACC) \times IC$ | Chapter 14 |

### A.2 Sensitivity Analysis: Segment WACCs Under Different MRP Assumptions

| MRP Assumption | Telecom WACC | P&S WACC | WACC Gap |
|---|---|---|---|
| MRP = 4.5% | 7.91% | 10.53% | 2.62% |
| MRP = 5.0% | 8.22% | 10.87% | 2.65% |
| MRP = 5.5% (base case) | **8.53%** | **11.22%** | **2.69%** |
| MRP = 6.0% | 8.84% | 11.56% | 2.72% |
| MRP = 6.5% | 9.16% | 11.91% | 2.75% |

**Sensitivity to β_U estimation (P&S WACC only):**

| P&S Avg β_U Scenario | P&S β_L (relevered) | P&S WACC | P&S Spread (ROC=11%) |
|---|---|---|---|
| Low β_U = 1.10 | 1.162 | 10.52% | **+0.48%** (value creating) |
| Base β_U = 1.24 | 1.315 | 11.22% | **−0.22%** (value destroying) |
| High β_U = 1.40 | 1.481 | 12.37% | **−1.37%** (value destroying) |

**Conclusion from sensitivity:** The conclusion that P&S is destroying value is sensitive to beta estimation. At lower beta estimates (excluding high-beta outliers), P&S could be marginally value-creating. This reinforces that the story is one of marginal performance near the WACC threshold—not catastrophic value destruction.

### A.3 Corporate WACC Cross-Check

From the case (Exhibit 1), TeleTech corporate WACC = 9.30%, with MV weights: 75% Telecom, 25% P&S.

Our segment WACCs pass the consistency check:

$$WACC_{corporate} \approx 0.75 \times 8.53\% + 0.25 \times 11.22\% = 6.40\% + 2.81\% = 9.21\%$$

This is very close to the stated 9.30%, confirming our estimates are internally consistent (the small difference reflects estimation error and the ignored corporate treasury segment discussed in Exhibit 2).

### A.4 Capital Structure Theory (Chapter 15)

The choice of different D/V ratios for each segment reflects the trade-off theory of capital structure:

- **Telecom (D/V = 26.25%):** Stable, regulated cash flows enable more leverage; lower default risk allows A-rated debt financing
- **P&S (D/V = 8.59%):** Higher cash flow volatility and competitive risk means minimal debt; BB-rated debt carries a 173 bps premium over A-rated Telecom bonds

The dramatically lower leverage in P&S comparables (9% vs. 26% D/V) explains why the unlever-relever adjustment has a relatively modest impact on P&S beta: most of the P&S beta is **operating risk**, not financial risk.

---

*Report prepared by Group 4, MFE 5231 Financial Management, CUHK(Shenzhen), 2025-2026.*
