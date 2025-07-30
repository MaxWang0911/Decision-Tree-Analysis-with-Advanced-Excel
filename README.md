# Decision Analysis for Clean & Brite Toothpaste Launch

> 📌 **Real-world business decision case**: This project models and optimises Clean & Brite's decision on whether to launch a new toothpaste brand, using decision tree analysis, risk profiling, and value-of-information methods implemented in Excel.

---

## 🧩 Problem Overview

Clean & Brite (C&B), a consumer goods company, is evaluating whether to launch a new brand of toothpaste. The decision is complex and risky:

- ✅ If successful, the launch could generate **$1,800,000** in profits.
- ❌ If it fails, it could lead to a **$750,000** loss.
- 🚫 If not launched, no profit or loss will occur.
- 🎯 The product manager estimates the probability of success as **p₁ = 0.35**.
- 🔬 C&B may invest **$130,000** in market research to better inform the decision.

This scenario is a classic **decision under uncertainty** problem, ideal for structured decision analysis using tools such as **decision trees**, **Bayesian inference**, **Expected Value of Sample Information (EVSI)**, and **Expected Value of Perfect Information (EVPI)**.

---

## ⚙️ Analytical Approach

### 1. **Decision Tree Construction**

A decision tree was built to model:
- Launch vs. no launch options
- Conditional probabilities of success and failure
- Incorporation of a market research decision node
- Calculation of **expected monetary value (EMV)** for all strategies

### 2. **Bayesian Probability Updates**
- Posterior probabilities were calculated using **Bayes’ Theorem**, based on research accuracy:
  - p₂ = P(Research predicts success | actual success) = 0.8
  - p₃ = P(Research predicts failure | actual failure) = 0.7
- Updated probabilities of actual success/failure were computed from research predictions.

### 3. **Risk Analysis**
- The **risk profile** of each strategy (profit/loss probability distribution) was assessed.
- Probabilities of achieving profit, incurring loss, or earning zero were estimated.
- A **trade-off** between expected value and risk exposure was discussed using Pareto front reasoning.

### 4. **EVSI and Sensitivity Analysis**
- A two-way data table was built in Excel to assess how changes in p₁, p₂, and p₃ affect the **Expected Value of Sample Information** (EVSI).
- Key insight: **Improving accuracy of external research (p₂ and p₃)** has the greatest impact on increasing EVSI.

### 5. **EVPI Calculation**
- The **Expected Value of Perfect Information (EVPI)** was computed to quantify the **maximum value of eliminating uncertainty**.
- For p₁ = 0.35, EVPI = **$487,500**, representing the upper bound on what should be spent on market research.

---

## 💡 Key Results

| Strategy                                  | Expected Value (EMV) | Notes                                              |
|------------------------------------------|-----------------------|-----------------------------------------------------|
| Launch with no research                  | $142,500              | Moderate expected profit but high failure risk      |
| Launch only if research predicts success | **$227,750**          | Optimal strategy based on current parameters        |
| No launch                                | $0                    | Zero risk, but also zero return                     |
| EVSI (with current p₁, p₂, p₃)           | $215,250              | Significant value in market research                |
| EVPI (p₂ = 1, p₃ = 1)                    | $487,500              | Maximum value of perfect prediction                 |

---

## 📊 Tools Used

- **Microsoft Excel**: Decision tree modelling, probability computation, sensitivity analysis using data tables
- **Bayesian Analysis**: Posterior probability calculation
- **Risk Profiling**: Strategy comparison via outcome distributions
- **Value of Information**: EVSI and EVPI assessments
---

## ✅ Conclusion

To maximise expected profit while controlling for risk, **Clean & Brite should invest in market research** and proceed with the product launch **only if the research predicts success**. This strategy balances profit potential with downside risk, supported by a rigorous decision analysis framework.

This project demonstrates how **structured decision-making**, supported by **advanced Excel modelling and probabilistic reasoning**, can provide actionable insights for real-world product launch decisions under uncertainty.

---

## 📚 Reference

Winston, W. L., & Albright, S. C. (2017). *Practical Management Science* (5th ed.). South-Western Cengage Learning.
