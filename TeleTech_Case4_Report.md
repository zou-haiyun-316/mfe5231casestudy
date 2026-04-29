# MFE 5231 Case Study Report
## Case 4: TeleTech Corporation, 2005
### Risk-Adjusted Hurdle Rates and Value Creation

**Group 4:** Rangxila GONG | Huihui LIU | Haiyun ZOU
**Course:** MFE 5231 Financial Management, 2nd Term 2025-2026, CUHK(Shenzhen)
**Instructor:** Prof. Joseph Cheng

---

## 1. Introduction

TeleTech Corporation is a large regional telecommunications company headquartered in Dallas, Texas. It defines itself as a "provider of integrated information movement and management" and operates two distinct business segments:

- **Telecommunications Services:** Provides long-distance, local, and cellular telephone service to over 7 million customer lines in the Southwest and Midwest. Revenues grow at ~3% annually; this segment benefits from stable, regulated cash flows.
- **Products & Systems (P&S):** Engages in the manufacture of computing and telecommunications equipment. Formed after TeleTech acquired a computer-workstation manufacturer in 2000; revenues grew nearly 40% in 2004 as a technology leader, but face high R&D requirements and increasing competition.

In October 2005, Victor Yossarian—a reclusive billionaire who acquired a 10% stake in TeleTech—publicly demanded that the company sell its P&S segment and focus on telecommunications. His claim: *"The firm is misusing its resources and not earning an adequate return."*

CFO Margaret Weston must respond to Yossarian's challenge, defend or revise TeleTech's capital allocation strategy, and determine the appropriate hurdle rates for each segment going forward.

---

## 2. Problem Identification

### 2.1 The Single Hurdle Rate

TeleTech currently applies a single, company-wide hurdle rate of **9.30%** to all investment and performance-measurement decisions. This rate represents TeleTech's blended Weighted Average Cost of Capital (WACC), calculated from its overall capital structure (Exhibit 1 of the case):

| Parameter | Value |
|---|---|
| Equity beta (β) | 1.15 |
| Risk-free rate (r_f) | 4.62% (30-yr Treasury) |
| Market return (r_M) | 10.12% |
| Market Risk Premium (MRP) | 5.50% |
| Cost of equity | 10.95% |
| Pre-tax cost of debt | 5.88% (A−/BBB+ rated) |
| Weight of debt (D/V) | 22.2% |
| Weight of equity (E/V) | 77.8% |
| **Corporate WACC** | **9.30%** |

### 2.2 Why This Is a Problem

The two segments differ fundamentally in their **business risk**:

| Feature | Telecom Services | Products & Systems |
|---|---|---|
| Industry | Regulated telecommunications | Competitive technology manufacturing |
| Revenue growth | ~3% p.a. (stable) | ~40% in 2004 (volatile) |
| Cash flow stability | High — regulated returns | Low — R&D-intensive, competitive |
| Bond rating (comparable firms) | A | BB |
| 2004 ROC (case text, p.2) | **9.10%** | **11.00%** |
| Capital (book value, p.2) | **$11.4 billion** | **$4.6 billion** |

When a company with two very different risk profiles uses one blended WACC, it creates **systematic misallocation of capital**:

- The **low-risk** Telecom segment faces an **overstated** hurdle rate → good projects get rejected
- The **high-risk** P&S segment faces an **understated** hurdle rate → bad projects get approved

This is precisely the concern raised by Rick Phillips (VP of Telecom Services) in the case, and supported by Exhibit 2's theoretical overview from Bernard Ingles.

### 2.3 Specific Questions to Address

**(a)** Should TeleTech use a single hurdle rate or risk-adjusted rates for each segment?

**(b)** What are the appropriate WACC estimates for the Telecom Services and P&S segments?

**(c)** Has the P&S segment been destroying value? Should TeleTech adopt risk-adjusted rates?

**(d)** What barriers would TeleTech face in implementing segment-specific hurdle rates?

---

## 3. Method: Estimating Segment WACCs

### 3.1 Framework

To estimate a segment-specific WACC, we need two components:
1. **Cost of Equity** via CAPM: $r_e = r_f + \beta \times MRP$
2. **Cost of Debt** from the bond market, adjusted for taxes: $r_d \times (1-t)$

Then: $WACC = (E/V) \times r_e + (D/V) \times r_d \times (1-t)$

### 3.2 Comparable Company Approach (Exhibit 3)

Since TeleTech's segments do not issue their own securities, we identify **publicly traded pure-play firms** in each industry from Exhibit 3, and use their industry averages directly:

**Key parameters (from Exhibit 1 and Exhibit 4):**

| Parameter | Value | Source |
|---|---|---|
| Risk-free rate (r_f) | 4.62% | 30-year U.S. Treasury yield, Exhibit 4 |
| Market Risk Premium (MRP) | 5.50% | Exhibit 1 (R_M − R_f = 10.12% − 4.62%) |
| Tax rate (t) | 40% | Case text |

We use the **industry average equity beta** (β) and **average market-value debt ratio (D/V)** directly from Exhibit 3, without adjustment. This reflects the typical risk profile of each comparable industry. The cost of debt is determined by the bond rating most representative of each segment.

---

## 4. Solution

### 4.1 Segment WACC Estimates (Question b)

#### Telecom Services Segment

**Comparables:** Telecommunications Services Industry (Exhibit 3, all 9 companies)

| Exhibit 3 Average | Value |
|---|---|
| Average equity beta (β) | **1.04** |
| Market-value debt ratio (D/V) | **27.1%** |
| Market-value equity ratio (E/V) | **72.9%** |

**WACC Calculation:**

$$r_e = 4.62\% + 1.04 \times 5.50\% = 4.62\% + 5.72\% = \mathbf{10.34\%}$$

Cost of debt: **5.74%** (A-rated bonds, from Exhibit 1 Telecom column and Exhibit 4)

$$WACC_{Telecom} = 0.729 \times 10.34\% + 0.271 \times 5.74\% \times 0.60 = 7.54\% + 0.93\% = \mathbf{8.47\%}$$

---

#### Products & Systems Segment

**Comparables:** P&S engages in both computing and telecom equipment manufacturing, so we use the average of the **Telecommunications Equipment Industry** and **Computer & Network Equipment Industry** (Exhibit 3), both in their entirety.

| Exhibit 3 | Telecom Equipment | Computer/Network Equipment | P&S Average |
|---|---|---|---|
| Average equity beta (β) | 1.39 | 1.33 | **1.36** |
| Market-value D/V | 13.1% | 5.3% | **9.2%** |
| Market-value E/V | 86.9% | 94.7% | **90.8%** |

**WACC Calculation:**

$$r_e = 4.62\% + 1.36 \times 5.50\% = 4.62\% + 7.48\% = \mathbf{12.10\%}$$

Cost of debt: **7.47%** (BB-rated bonds, from Exhibit 1 and Exhibit 4)

$$WACC_{P\&S} = 0.908 \times 12.10\% + 0.092 \times 7.47\% \times 0.60 = 10.99\% + 0.41\% = \mathbf{11.40\%}$$

---

#### Summary: Segment WACCs vs. Corporate WACC

| Metric | Telecom Services | Products & Systems | Corporate (Exhibit 1) |
|---|---|---|---|
| Comparable industry | Telecom Services | Equip. + Computer (blended) | — |
| Equity beta (β) | **1.04** | **1.36** | 1.15 |
| Cost of equity (r_e) | **10.34%** | **12.10%** | 10.95% |
| Cost of debt (pre-tax) | 5.74% (A) | 7.47% (BB) | 5.88% (A−/BBB+) |
| D/V weight | 27.1% | 9.2% | 22.2% |
| E/V weight | 72.9% | 90.8% | 77.8% |
| **Segment WACC** | **8.47%** | **11.40%** | **9.30%** |
| ROC (2004, case p.2) | **9.10%** | **11.00%** | ~9.58% |
| **Spread (ROC − WACC)** | **+0.63%** | **−0.40%** | +0.28% |

> **Internal consistency check:** 0.75 × 8.47% + 0.25 × 11.40% = 6.35% + 2.85% = **9.20%** ≈ 9.30% corporate WACC ✓

---

### 4.2 Single vs. Risk-Adjusted Hurdle Rates (Question a)

#### The Illusion Created by a Single Rate

Under the **9.30% uniform hurdle rate**:
- Telecom ROC (9.10%) **< 9.30%** → Telecom appears to **destroy** value (spread = −0.20%)
- P&S ROC (11.00%) **> 9.30%** → P&S appears to **create** value (spread = +1.70%)

This produces exactly the **wrong strategic signal.**

Under **risk-adjusted rates**:
- Telecom ROC (9.10%) **> 8.47%** → Telecom **creates** value (spread = +0.63%) ✓
- P&S ROC (11.00%) **< 11.40%** → P&S **destroys** value (spread = −0.40%) ✗

#### Decision Errors Under Uniform Rate

| Project Scenario | Uniform Rate (9.30%) Says | Risk-Adjusted Rate Says | Error |
|---|---|---|---|
| Telecom project, IRR = 9.00% | REJECT (< 9.30%) | ACCEPT (> 8.47%) | Type I: Reject good project |
| Telecom project, IRR = 8.80% | REJECT | ACCEPT | Type I: Reject good project |
| P&S project, IRR = 10.50% | ACCEPT (> 9.30%) | REJECT (< 11.40%) | Type II: Accept bad project |
| P&S project, IRR = 9.80% | ACCEPT | REJECT | Type II: Accept bad project |

This is Rick Phillips's argument from the case: "Telecommunications services lowers the risk of the whole corporation, and should not be penalized."

---

### 4.3 EVA Analysis — Has P&S Destroyed Value? (Question c)

**Economic Value Added (EVA)** measures whether a segment earns above or below its risk-adjusted cost of capital:

$$EVA = (ROC - WACC_{segment}) \times Invested\ Capital$$

Using book-value invested capital from the case (page 2):

| Segment | ROC | Segment WACC | Spread | Capital (Book) | Annual EVA |
|---|---|---|---|---|---|
| Telecom Services | 9.10% | 8.47% | **+0.63%** | $11.4B | **+$71.7M** |
| Products & Systems | 11.00% | 11.40% | **−0.40%** | $4.6B | **−$18.4M** |
| **Net** | — | — | — | **$16.0B** | **+$53.3M** |

**Answer: Yes, P&S has been destroying value — approximately $18.4 million per year on a risk-adjusted basis.**

The key finding: P&S earns 11.00% ROC, which appears impressive in absolute terms. But once we account for the *higher risk* of this business (WACC = 11.40%), the true picture changes — P&S is marginally below its cost of capital.

**Should TeleTech implement risk-adjusted rates?** Yes. The switch does not create destruction — it *reveals* destruction already occurring. Implementing risk-adjusted rates would:
1. Stop approvals of P&S projects that appear profitable at 9.30% but are below the 11.40% risk-adjusted threshold
2. Unlock Telecom projects with returns between 8.47% and 9.30% that are currently rejected under the uniform rate
3. Send correct signals to segment managers about actual value creation

---

### 4.4 Barriers to Implementation (Question d)

Despite the theoretical clarity, four major barriers stand in the way:

**1. Organizational and Political Resistance**
Under the current 9.30% rate, P&S appears to be the star (+1.70% spread). Adopting risk-adjusted rates would expose P&S as a value destroyer. P&S leadership (Helen Buono in the case) will lobby against this, arguing that "all money is green" — the same hurdle rate should apply to all investments.

**2. Technical and Analytical Challenges**
Equity betas from comparable firms vary with the choice of estimation window and comparable set. A different selection of firms from Exhibit 3 could shift P&S's WACC by 1–2 percentage points, changing the qualitative conclusion. There is no single "correct" answer.

**3. Incentive and Compensation Misalignment**
If compensation systems remain tied to the 9.30% benchmark, managers will ignore the new hurdle rates in practice. Worse, a higher P&S threshold may push managers toward short-term ROIC improvements (cutting R&D) at the expense of long-run value.

**4. Organizational Change and Consistency**
Margaret Weston raises this concern in the case: using different discount rates across segments makes NPV and EVA results incomparable. A single rate ensures consistency across business units. The move to multiple rates requires extensive education, system updates, and ongoing recalibration.

---

## 5. Conclusion and Recommendations

### 5.1 Key Findings

| Question | Answer |
|---|---|
| **a. Single vs. risk-adjusted?** | Risk-adjusted. Uniform 9.30% produces wrong signals: Telecom looks unprofitable, P&S looks profitable. Both are reversed under correct rates. |
| **b. Segment WACCs** | Telecom Services: **8.47%** \| Products & Systems: **11.40%** |
| **c. P&S value creation?** | P&S destroys **−$18.4M/yr**; Telecom creates **+$71.7M/yr**. Net firm EVA = +$53.3M. Yes, adopt risk-adjusted rates. |
| **d. Barriers** | Political resistance (P&S lobby), technical subjectivity (beta estimation), incentive misalignment, organizational change costs |

### 5.2 Response to Yossarian

Yossarian is **directionally correct**: the uniform hurdle rate masks P&S's risk-adjusted underperformance. However, his call to immediately sell P&S may be premature. P&S's gap is small (−0.40%, or −$18.4M/yr), and the strategic benefits of integrating computing and telecom technology may justify continuing while improving ROIC.

TeleTech's best response:
1. **Acknowledge** the validity of segment-specific risk analysis
2. **Adopt** risk-adjusted hurdle rates immediately (Telecom: 8.47%, P&S: 11.40%)
3. **Set** a 12-month ROIC improvement target for P&S (target: exceed 11.40%)
4. **Reserve** the divestiture option if P&S cannot meet the revised performance threshold

### 5.3 Action Plan

| Priority | Action | Timeline |
|---|---|---|
| **Immediate** | Adopt risk-adjusted hurdle rates: Telecom 8.47%, P&S 11.40% | Q1 2006 |
| **Short-term** | Recalibrate management compensation to segment-specific EVA benchmarks | Q2 2006 |
| **Medium-term** | Strategic review of P&S: set ROIC improvement targets or consider divestiture | 2006 |
| **Ongoing** | Annual update of segment betas using comparable industry data | Annual |

---

## Appendix: WACC Calculation Reference

### Formula Summary

| Formula | Expression |
|---|---|
| CAPM | $r_e = r_f + \beta \times MRP$ |
| WACC | $WACC = (E/V) \times r_e + (D/V) \times r_d \times (1-t)$ |
| EVA | $EVA = (ROC - WACC) \times Invested\ Capital$ |

### Sensitivity Analysis: Segment WACCs Under Different MRP Assumptions

| MRP | Telecom WACC | P&S WACC | Telecom Spread | P&S Spread |
|---|---|---|---|---|
| 4.5% | 8.02% | 10.74% | +1.08% | +0.26% |
| 5.0% | 8.24% | 11.07% | +0.86% | −0.07% |
| **5.5% (base)** | **8.47%** | **11.40%** | **+0.63%** | **−0.40%** |
| 6.0% | 8.70% | 11.72% | +0.40% | −0.72% |
| 6.5% | 8.93% | 12.05% | +0.17% | −1.05% |

Note: P&S destroys value under MRP ≥ ~5.0%, and Telecom creates value under all scenarios.

---

*Report prepared by Group 4 (Rangxila GONG | Huihui LIU | Haiyun ZOU), MFE 5231 Financial Management, CUHK(Shenzhen), 2025-2026.*
