# MFE 5231 Case Study Report
## Case 4: TeleTech Corporation, 2005
### Risk-Adjusted Hurdle Rates and Value Creation

**Group 4:** Rangxila GONG | Huihui LIU | Yin PANG | Haiyun ZOU  
**Course:** MFE 5231 Financial Management, 2nd Term 2025-2026, CUHK(Shenzhen)  
**Instructor:** Prof. Joseph Cheng

---

## Executive Summary

TeleTech Corporation operates two distinct business segments—**Telecommunications Services** and **Products & Systems (P&S)**—but applies a single corporate hurdle rate of **9.30%** to all capital allocation decisions. This report demonstrates that this practice is financially incorrect and leads to systematic value misallocation.

Using the unlever-relever beta methodology and CAPM (as taught in Chapter 14, Cost of Capital), we estimate that the **Telecommunications Services** segment has a true risk-adjusted WACC of approximately **8.84%**, while **Products & Systems** carries a far higher WACC of approximately **11.97%**, reflecting its substantially greater business risk.

Against these benchmarks, our Economic Value Added (EVA) analysis reveals that Telecom Services **creates** approximately **$59.3 million** of value per year, while Products & Systems **destroys** approximately **$62.6 million** per year—a finding entirely hidden when using the uniform 9.30% hurdle rate.

We recommend that TeleTech immediately adopt risk-adjusted hurdle rates by segment and simultaneously review the strategic future of the P&S segment.

---

## 1. Company Background and the Core Problem

### 1.1 TeleTech's Two Segments

TeleTech Corporation is a diversified telecommunications company with two business segments that differ fundamentally in their risk-return characteristics.

| Feature | Telecom Services | Products & Systems |
|---|---|---|
| Nature | Regulated, utility-like | Technology & manufacturing |
| Revenue (FY2004) | ~$9.6 billion (73% of total) | ~$3.5 billion (27% of total) |
| Cash Flow Stability | High — predictable regulated returns | Low — cyclical, competitive |
| ROIC (FY2004) | **9.63%** | **8.84%** |
| Current Hurdle Rate | 9.30% (corporate-wide) | 9.30% (corporate-wide) |
| Spread vs. Hurdle | +0.33% | −0.46% |

### 1.2 The Fundamental Problem

TeleTech's current practice is to evaluate **all** investment projects across both segments using a single corporate hurdle rate of **9.30%**. This rate is derived from the blended cost of capital of the entire firm, averaging across both segments.

The problem with this approach was articulated clearly in Chapter 14 (Cost of Capital):

> *"Cost of Capital: the minimum rate that must be achieved in order to satisfy the required return of all of the firm's investors."*

When a firm with multiple business segments uses one blended rate, it implicitly treats all segments as equally risky—a fundamentally flawed assumption given the stark differences between regulated telecommunications and competitive technology manufacturing.

**The result is a "cross-subsidy" mechanism:**

- The low-risk Telecom segment faces an **artificially high** hurdle rate (9.30% vs. its true WACC of 8.84%), causing good projects to be rejected.
- The high-risk P&S segment faces an **artificially low** hurdle rate (9.30% vs. its true WACC of 11.97%), causing bad projects to be accepted.

Capital flows in the wrong direction: from value-creating Telecom to value-destroying P&S.

---

## 2. Estimating Segment WACC (Question b)

### 2.1 Methodology

We follow the three-step methodology taught in Chapter 14 and used in the Boeing 7E7 and Star River cases:

```
Step 1: Find comparable pure-play firms for each segment (Exhibit 3)
Step 2: Unlever each comparable's beta to remove the effect of financial leverage
Step 3: Average unlevered betas → Re-lever using segment's target capital structure
Step 4: Apply CAPM to get Cost of Equity
Step 5: Weight Cost of Equity and after-tax Cost of Debt → WACC
```

**Key Parameters (fixed for both segments):**

| Parameter | Value | Rationale |
|---|---|---|
| Risk-free rate (r_f) | **4.62%** | Yield on 10-year U.S. Treasury (2005) |
| Market Risk Premium (MRP) | **5.50%** | Standard mid-point estimate for U.S. equity premium |
| Marginal Tax Rate (t) | **40%** | TeleTech's effective marginal tax rate |
| (1 − t) | **0.60** | Tax shield factor |

**Beta Adjustment Formulas (from Chapter 14 / Course Notes):**

$$\beta_U = \frac{\beta_L}{1 + (1-t) \times \frac{D}{E}} \quad \text{[Unlever: remove financial risk]}$$

$$\beta_L^{target} = \beta_U \times \left[1 + (1-t) \times \frac{D}{E}_{target}\right] \quad \text{[Re-lever: apply target structure]}$$

---

### 2.2 Telecom Services Segment

#### Step 1 & 2: Comparable Companies — Unlever Beta

The four comparable firms are regulated U.S. telecom carriers from Exhibit 3. Note that the capital structure weights used for each segment are the **average of comparable firms** (as instructed in the problem).

| Company | Levered β_L | D/V | E/V | D/E = D/V ÷ E/V | Unlevered β_U |
|---|---|---|---|---|---|
| BellSouth | 0.80 | 31.1% | 68.9% | 0.4514 | 0.80 ÷ (1 + 0.60 × 0.4514) = **0.630** |
| SBC Communications | 0.75 | 28.3% | 71.7% | 0.3948 | 0.75 ÷ (1 + 0.60 × 0.3948) = **0.606** |
| Verizon | 0.90 | 37.9% | 62.1% | 0.6103 | 0.90 ÷ (1 + 0.60 × 0.6103) = **0.653** |
| Sprint Nextel | 0.85 | 35.1% | 64.9% | 0.5408 | 0.85 ÷ (1 + 0.60 × 0.5408) = **0.637** |
| **Average** | **0.825** | **33.1%** | **66.9%** | **0.4943** | **0.632** |

**Sample Calculation (BellSouth):**
$$\beta_U^{BellSouth} = \frac{0.80}{1 + 0.60 \times 0.4514} = \frac{0.80}{1.2708} = 0.630$$

#### Step 3: Re-lever Beta for Telecom Segment

Target capital structure = average of comparables: **D/V = 33.1%, E/V = 66.9%, D/E = 0.4943**

$$\beta_L^{Telecom} = 0.632 \times (1 + 0.60 \times 0.4943) = 0.632 \times 1.2966 = \mathbf{0.820}$$

#### Step 4: Cost of Equity (CAPM)

$$r_e^{Telecom} = r_f + \beta_L^{Telecom} \times MRP = 4.62\% + 0.820 \times 5.50\% = 4.62\% + 4.51\% = \mathbf{9.13\%}$$

#### Step 5: WACC for Telecom Services

Pre-tax cost of debt for Telecom (average of comparables): **r_d = 5.74%**

$$WACC_{Telecom} = \underbrace{0.669 \times 9.13\%}_{\text{equity component}} + \underbrace{0.331 \times 5.74\% \times (1-0.40)}_{\text{after-tax debt}}$$

$$= 6.11\% + 1.14\% = \mathbf{8.84\%\ (Telecom\ Services\ WACC)}$$

---

### 2.3 Products & Systems Segment

#### Step 1 & 2: Comparable Companies — Unlever Beta

The four comparables are competitive technology/equipment companies from Exhibit 3.

| Company | Levered β_L | D/V | E/V | D/E | Unlevered β_U |
|---|---|---|---|---|---|
| Motorola | 1.60 | 19.6% | 80.4% | 0.2438 | 1.60 ÷ (1 + 0.60 × 0.2438) = **1.397** |
| Lucent Technologies | 1.75 | 31.0% | 69.0% | 0.4493 | 1.75 ÷ (1 + 0.60 × 0.4493) = **1.374** |
| Nortel Networks | 1.85 | 28.0% | 72.0% | 0.3889 | 1.85 ÷ (1 + 0.60 × 0.3889) = **1.499** |
| EDS | 1.45 | 22.5% | 77.5% | 0.2903 | 1.45 ÷ (1 + 0.60 × 0.2903) = **1.232** |
| **Average** | **1.6625** | **25.3%** | **74.7%** | **0.3388** | **1.375** |

**Sample Calculation (Motorola):**
$$\beta_U^{Motorola} = \frac{1.60}{1 + 0.60 \times 0.2438} = \frac{1.60}{1.1463} = 1.397$$

#### Step 3: Re-lever Beta for P&S Segment

Target capital structure = average of comparables: **D/V = 25.3%, E/V = 74.7%, D/E = 0.3388**

$$\beta_L^{P\&S} = 1.375 \times (1 + 0.60 \times 0.3388) = 1.375 \times 1.2033 = \mathbf{1.655}$$

#### Step 4: Cost of Equity (CAPM)

$$r_e^{P\&S} = 4.62\% + 1.655 \times 5.50\% = 4.62\% + 9.10\% = \mathbf{13.72\%}$$

#### Step 5: WACC for P&S Segment

Pre-tax cost of debt for P&S (higher risk): **r_d = 6.30%**

$$WACC_{P\&S} = \underbrace{0.747 \times 13.72\%}_{\text{equity component}} + \underbrace{0.253 \times 6.30\% \times (1-0.40)}_{\text{after-tax debt}}$$

$$= 10.25\% + 0.96\% = \mathbf{11.21\%\ (P\&S\ WACC)}$$

---

### 2.4 Summary: Corporate vs. Segment WACCs

| Metric | Telecom Services | Products & Systems | Corporate Blended |
|---|---|---|---|
| Avg. Unlevered Beta (β_U) | 0.632 | 1.375 | — |
| Re-levered Beta (β_L) | **0.820** | **1.655** | ~1.04 |
| Cost of Equity (r_e) | **9.13%** | **13.72%** | ~10.34% |
| After-tax Cost of Debt | 3.44% | 3.78% | ~3.57% |
| E/V Weight | 66.9% | 74.7% | ~70% |
| D/V Weight | 33.1% | 25.3% | ~30% |
| **WACC** | **8.84%** | **11.21%** | **9.30%** |
| **ROIC (FY2004)** | **9.63%** | **8.84%** | **~9.40%** |
| **Spread (ROIC − WACC)** | **+0.79%** | **−2.37%** | **+0.10%** |

**Key Insight:** The corporate-blended WACC of 9.30% masks a 2.37 percentage point value-destruction gap in P&S, and simultaneously understates the value-creation in Telecom.

---

## 3. Constant vs. Risk-Adjusted Hurdle Rates (Question a)

### 3.1 The Decision Errors Created by a Uniform Rate

Using the **Security Market Line (SML)** framework, we can visualize the error embedded in TeleTech's uniform hurdle rate:

```
Expected Return
     │
13%  │                           ┌─────────────────────────────┐
     │                           │  TRUE cost of capital       │
     │                           │  for P&S = 11.21%           │
11%  │ - - - - - - - - - - - - -┼- - - - - - - -              │
     │  Uniform hurdle (9.30%)  ─┼────────────────────────────── ←── P&S is HERE
     │                          ─┼──────────────                │
 9%  │              Telecom SML ─┘                             │
     │                           ←── Telecom is HERE           │
 8%  │ ──── Telecom true WACC (8.84%) ─────────────────────    │
     │                                                          │
     └──────────────────────────────────────────────────────────
                     Telecom                    P&S
                  (Low Risk: β=0.82)       (High Risk: β=1.66)
```

**Systematic Decision Errors under Uniform Hurdle Rate (9.30%):**

| Scenario | What uniform rate says | What risk-adjusted rate says | Error Type |
|---|---|---|---|
| Telecom project, IRR = 9.20% | ACCEPT (9.20% > 9.30%? No → actually REJECT) | ACCEPT (9.20% > 8.84%) | Type I: Reject good projects |
| Telecom project, IRR = 9.00% | REJECT | ACCEPT (9.00% > 8.84%) | Type I: Reject good projects |
| P&S project, IRR = 10.00% | ACCEPT (10.00% > 9.30%) | REJECT (10.00% < 11.21%) | Type II: Accept bad projects |
| P&S project, IRR = 9.50% | ACCEPT | REJECT | Type II: Accept bad projects |

### 3.2 Implications for TeleTech's Resource Allocation Strategy

The uniform hurdle rate creates four specific distortions in how TeleTech allocates capital:

**Distortion 1 — Capital Over-allocation to P&S:**  
Projects in P&S with returns between 9.30% and 11.21% will be approved under the uniform rate but are actually destroying value. Management will over-invest in the high-risk segment.

**Distortion 2 — Capital Under-allocation to Telecom:**  
Projects in Telecom with returns between 8.84% and 9.30% will be rejected under the uniform rate, even though they create value. Value-creating investment is systematically starved.

**Distortion 3 — Flawed Strategic Signaling:**  
Under the uniform rate, Telecom appears to be only a marginal performer (+0.33% spread), while P&S appears nearly acceptable (−0.46% spread). In reality, Telecom is a strong performer and P&S is a significant value destroyer. The uniform rate produces precisely the *opposite* strategic signal.

**Distortion 4 — Managerial Incentive Misalignment:**  
If P&S managers are evaluated against a 9.30% hurdle, they face an inappropriate benchmark. A manager who generates 10.0% ROIC in P&S appears to be a strong performer, but is in fact destroying 1.21% of value annually relative to the true cost of capital.

---

## 4. Has P&S Destroyed Value? Should TeleTech Implement Risk-Adjusted Rates? (Question c)

### 4.1 Economic Value Added (EVA) Analysis

EVA directly answers whether each segment earned more than its cost of capital:

$$EVA = (ROIC - WACC_{segment}) \times Invested\ Capital$$

This is the NPV-equivalent metric for ongoing operations—a positive EVA means the segment has generated surplus returns above what investors require, while a negative EVA means value has been destroyed (analogous to a negative NPV project per Chapter 11).

**Estimating Invested Capital by Segment:**

Using TeleTech's revenue split as a proxy for capital allocation (revenues: Telecom 73%, P&S 27%; total firm invested capital ~$12 billion, consistent with Exhibit 2):

| Segment | Estimated Invested Capital |
|---|---|
| Telecom Services | **$8,760M** (~73% × $12B) |
| Products & Systems | **$3,240M** (~27% × $12B) |
| Total | **$12,000M** |

**EVA Calculation:**

| Segment | ROIC | Segment WACC | Spread | Invested Capital | Annual EVA |
|---|---|---|---|---|---|
| Telecom Services | 9.63% | 8.84% | **+0.79%** | $8,760M | **+$69.2M** |
| Products & Systems | 8.84% | 11.21% | **−2.37%** | $3,240M | **−$76.8M** |
| **Total (net)** | | | | **$12,000M** | **−$7.6M** |

### 4.2 Has Products & Systems Destroyed Value?

**Yes — definitively.** P&S has been destroying approximately **$76.8 million of shareholder value per year**.

More strikingly, TeleTech as a whole is a **net value destroyer** by approximately $7.6 million per year, despite the uniform hurdle rate suggesting the firm is earning 10 basis points above its cost of capital (+0.10% spread). The uniform rate masks the truth.

Under the uniform rate, management sees:

> *Telecom creates small value (+0.33%), P&S destroys small value (−0.46%), net firm is roughly OK.*

Under risk-adjusted rates, the truth is:

> *Telecom creates substantial value (+0.79%), P&S destroys massive value (−2.37%), the firm is actually destroying net value.*

### 4.3 Would Switching to Risk-Adjusted Rates Destroy Value?

**No.** The switch does not cause value destruction—it *reveals* destruction that is already occurring. The analogy is a thermometer: showing the patient's true temperature does not cause the fever.

In fact, implementing risk-adjusted rates would likely **improve** firm value by:
- Stopping approvals of P&S projects that clear the 9.30% hurdle but fall below 11.21%
- Unlocking previously rejected Telecom projects that clear 8.84% but fell below 9.30%
- Reallocating capital from value-destroying to value-creating uses

### 4.4 Should TeleTech Implement Risk-Adjusted Hurdle Rates?

**Our recommendation: Yes, implement immediately.**

The financial case is unambiguous:
- Chapter 14 (Cost of Capital): WACC must reflect the true risk of the specific project/division, not a blended average
- Chapter 11 (Capital Budgeting): The NPV decision rule requires discounting at the *appropriate* required rate—using the wrong rate leads to systematic accept/reject errors
- The EVA analysis shows the current system is destroying ~$76.8M/year in P&S alone

Without risk-adjusted hurdle rates, TeleTech will continue to misallocate capital, eroding shareholder wealth year after year.

---

## 5. Barriers to Implementation (Question d)

Despite the theoretical superiority of risk-adjusted hurdle rates, implementation in a real organization faces four major categories of barriers:

### 5.1 Organizational and Political Resistance

The most immediate barrier is internal politics. The P&S division currently benefits from an artificially low hurdle rate. Implementing segment-specific rates means P&S managers would face a 11.21% benchmark—nearly two percentage points higher than their current one. This would:

- Make many currently-approved P&S projects unacceptable
- Reduce P&S's capital budget and headcount
- Potentially lead to demotion or exit of P&S senior management

As a result, P&S leadership will almost certainly lobby against adoption. They may argue that the comparable firm selection is flawed, the beta estimate is too high, or that strategic value (not captured in ROIC) justifies the low returns. These objections may be partially valid but are likely to be self-serving.

Furthermore, the board may be reluctant to act on findings that imply a large segment of the firm has been destroying value—this implies past management decisions were wrong, a politically uncomfortable conclusion.

### 5.2 Technical and Analytical Challenges

Even setting aside politics, the methodology itself has limitations:

**Beta estimation instability:** Equity betas are estimated from historical stock returns and are inherently noisy. A beta of 1.655 for P&S could plausibly range from 1.3 to 2.0 depending on the estimation period, frequency, and peer group selected, implying a P&S WACC range of roughly 9.5% to 15.5%. This uncertainty may make management skeptical of the precision implied by a single-point estimate.

**Comparable company selection subjectivity:** There is no single "correct" set of comparable firms. Different analysts selecting different comparables would produce different unlevered betas. This invites gaming: divisions have incentives to propose comparables that minimize their hurdle rate.

**Corporate-level debt allocation:** TeleTech raises debt at the corporate level; it does not issue segment-specific bonds. Allocating debt costs to each segment requires judgment about how to apportion financial risk—a technically complex issue with no objectively correct answer.

**Interdependencies between segments:** TeleTech's two segments may share infrastructure, management, customer relationships, or R&D. These synergies mean neither segment can be cleanly separated and independently valued. A mechanically applied segment WACC ignores this interdependence.

### 5.3 Incentive and Compensation Misalignment

Changing the hurdle rate without simultaneously changing compensation systems will lead to behavioral inconsistencies. If P&S managers are still evaluated on metrics linked to the old 9.30% hurdle (e.g., EVA bonuses calibrated to the old rate), they will continue to behave as before—the new hurdle rate on paper will have no effect on actual investment decisions.

Moreover, a higher hurdle rate in P&S may create perverse incentives toward short-termism: managers might cut long-term R&D spending (which reduces near-term ROIC headcount) to meet the new ROIC benchmark, even if the R&D investments have positive NPV over a longer horizon.

### 5.4 Organizational Learning and Change Management

Finally, a practical barrier is the organizational effort required to shift the culture:

- **Education:** Every business unit finance team, regional manager, and project sponsor needs to understand why their division now faces a different hurdle—and why this is fair rather than punitive.
- **System updates:** Capital budgeting approval systems, financial models, and reporting dashboards need to be recalibrated to apply different discount rates.
- **Continuous recalibration:** Unlike a single corporate rate that can be set once and revisited annually, segment-specific rates require ongoing monitoring of comparable firm betas and capital structures.
- **External communication:** Investors and analysts expect consistency in how management discusses value creation. Introducing segment WACCs may require recommunicating the firm's capital allocation philosophy.

---

## 6. Conclusion and Recommendations

### 6.1 Summary of Findings

| Question | Key Finding |
|---|---|
| **a. Hurdle Rate Choice** | Uniform 9.30% creates systematic Type I (reject good) and Type II (accept bad) errors; risk-adjusted rates correctly align capital with risk |
| **b. Segment WACC** | Telecom Services: **8.84%** | Products & Systems: **11.21%** (vs. blended 9.30%) |
| **c. Value Creation** | P&S destroys **$76.8M/year**; Telecom creates **$69.2M/year**; net firm is a **value destroyer** under current rate. Should implement risk-adjusted rates |
| **d. Barriers** | Political resistance, beta/comparables subjectivity, incentive misalignment, organizational learning curve |

### 6.2 Action Plan

| Priority | Recommendation | Timeline |
|---|---|---|
| **Immediate** | Adopt risk-adjusted hurdle rates: Telecom 8.84%, P&S 11.21% | Q1 2006 |
| **Short-term** | Recalibrate compensation systems to EVA benchmarks using segment WACCs | Q2 2006 |
| **Medium-term** | Strategic review of P&S: restructure, divest, or set explicit turnaround targets | 2006 |
| **Ongoing** | Annual update of segment betas and comparable company data | Annual |

### 6.3 Final Verdict

TeleTech's current uniform hurdle rate is not merely theoretically impure—it is causing real, measurable, ongoing destruction of shareholder value. The risk-adjusted approach reveals a firm where one segment (Telecom) is a solid value creator being starved of capital, while another (P&S) is a value destroyer being over-fed with capital.

The finance principle is clear: as taught in Chapter 14, the purpose of estimating a cost of capital is to enable correct resource allocation between divisions. TeleTech must adopt risk-adjusted hurdle rates—not just as an academic exercise, but as an operational imperative.

---

## Appendix A: WACC Calculation Detail

### A.1 Formula Reference

| Formula | Expression | Source |
|---|---|---|
| CAPM | $r_e = r_f + \beta_L \times MRP$ | Chapter 14 |
| Unlever Beta | $\beta_U = \beta_L / [1 + (1-t)(D/E)]$ | Course Notes / Boeing Case |
| Re-lever Beta | $\beta_L^* = \beta_U \times [1 + (1-t)(D/E)^*]$ | Course Notes |
| WACC | $WACC = (E/V) r_e + (D/V) r_d (1-t)$ | Chapter 14 |
| EVA | $EVA = (ROIC - WACC) \times IC$ | Chapter 14 / Performance Measurement |

### A.2 Sensitivity Analysis: WACC Under Different MRP Assumptions

| MRP Assumption | Telecom WACC | P&S WACC | Gap |
|---|---|---|---|
| MRP = 4.5% | 8.31% | 10.06% | 1.75% |
| MRP = 5.5% (base case) | **8.84%** | **11.21%** | **2.37%** |
| MRP = 6.5% | 9.37% | 12.36% | 2.99% |
| MRP = 7.0% | 9.64% | 12.95% | 3.31% |

**Conclusion from sensitivity:** Regardless of MRP assumption, the qualitative conclusion is unchanged. Telecom WACC is always materially below P&S WACC, and P&S ROIC (8.84%) always falls well below P&S WACC.

### A.3 Capital Budgeting Decision Framework (Chapter 11)

The NPV rule (Chapter 11) requires:

$$NPV = \sum_{t=1}^{n} \frac{CF_t}{(1 + WACC_{correct})^t} - IO$$

Using the wrong discount rate (9.30% for P&S instead of 11.21%) overstates the NPV of P&S projects by:

$$\Delta NPV \approx \frac{CF}{WACC_{wrong}} - \frac{CF}{WACC_{correct}} = \frac{CF}{0.093} - \frac{CF}{0.1121} > 0$$

The positive $\Delta NPV$ means P&S projects *look* better than they are—a direct consequence of the uniform hurdle rate error.

### A.4 Capital Structure Theory (Chapter 15)

The choice of different D/V ratios for each segment (Telecom: 33.1%; P&S: 25.3%) reflects the chapter's teaching on the moderate position:

- Stable, regulated businesses (Telecom) can support more debt, because the lower volatility of cash flows reduces bankruptcy risk, allowing a higher optimal D/V.
- Cyclical, competitive businesses (P&S) should use less debt, because higher cash flow volatility combined with high leverage dramatically increases bankruptcy costs.

This theoretical prediction is confirmed by the real-world capital structures of the comparable companies in each segment.

---

*Report prepared by Group 4, MFE 5231 Financial Management, CUHK(Shenzhen), 2025-2026.*
