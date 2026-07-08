# Credit Card Spend Behaviour Analysis

An end-to-end **Python** dashboard analyzing credit card customer spending behavior — segmenting customers, flagging risky accounts, and uncovering the patterns behind balances, purchases, and cash advances to support credit risk management.

---

## Project Overview

Understanding how customers spend, borrow, and repay is key to reducing credit risk. This project analyzes **8,950 credit card customers**, using Python for data cleaning, feature engineering, customer segmentation, and visualization building a complete analytics dashboard from raw data to business-ready insights, entirely without a BI tool.

The dashboard covers 9 visual panels: balance distribution, spend types, active/inactive status, credit limit vs. purchases, customer segments, risk by segment, a correlation heatmap, risky vs. safe comparison, and a summary panel.

---

## Business Problem

The business wants to understand:
- Which customers are financially at-risk or likely to churn
- How balance, purchases, and cash advances relate to each other
- Which customer segments carry the highest risk
- How active vs. inactive customers differ in spending behavior
- Where to focus retention and risk-mitigation efforts

---

## Data Source

- **Dataset:** Kaggle
- **Records:** 8,950 customers
- **Fields used:** Balance, Purchases, One-off Purchases, Installment Purchases, Cash Advance, Payments, Credit Limit, Tenure, and related usage frequency fields

---

## Key KPIs

| Metric | Value |
|---|---|
| Total Customers | 8,950 |
| Risky Customers | 47 (0.5%) |
| Inactive Customers | 2,044 |
| Champions | 1,632 |
| Lost Customers | 0 |
| Active vs Inactive | 77.2% / 22.8% |

---

## Dashboard Panels

1. **Balance Distribution** — histogram of customer balances
2. **Spend Types** — total spend across One-off Purchases, Installment Purchases, and Cash Advance
3. **Active vs Inactive** — customer activity split
4. **Credit Limit vs Purchases** — scatter plot of spending vs. available credit
5. **Customer Segments** — segment sizes (At Risk, Loyal, Best Customer, Might Churn, Potential Loyal, Big Spender at Risk)
6. **Risk by Segment** — risky customer counts per segment
7. **Correlation Heatmap** — relationships between Balance, Purchases, Cash Advance, Payments, and Credit Limit
8. **Risky vs Safe Comparison** — Balance, Cash Advance, and Payments compared by risk flag
9. **Summary Panel** — key totals at a glance

---

## Key Insights

- Cash Advance spending far exceeds One-off and Installment Purchases combined a major red flag for risk exposure
- **"At Risk"** is the largest customer segment and also carries the highest concentration of risky accounts
- Balance and Cash Advance show a moderate positive correlation with Credit Limit (0.53 and 0.30), meaning higher limits often coincide with riskier borrowing behavior
- Purchases and Payments are the most strongly correlated metrics (0.60), showing spending discipline aligns closely with repayment behavior
- Purchases and Cash Advance are essentially uncorrelated (-0.05) — these are largely independent spending behaviors
- Risky customers (RISK_FLAG = 1) carry noticeably higher Balances and Cash Advances but make far fewer Payments than safe customers
- Despite high inactivity (22.8%), zero customers fall into the "Lost" category — a good sign for long-term retention potential

---

## Tools & Techniques Used

- **Python** — end-to-end analysis and dashboard generation
- **Pandas / NumPy** — data cleaning, feature engineering, aggregation
- **Matplotlib / Seaborn** — data visualization (histograms, scatter plots, heatmaps, bar charts)
- **Customer Segmentation** — rule-based segmentation (At Risk, Loyal, Best Customer, Might Churn, etc.)
- **Correlation Analysis** — identifying relationships between spending and risk variables
- **Risk Flagging** — logic-based flag for identifying risky accounts

---

## 📸 Screenshots

### Full Dashboard
![Credit Card Spend Behaviour Dashboard](https://github.com/Saqibaminzargar/-Credit-Card-Spend-Behaviour-Analysis/blob/main/Credit%20Card%20Spend%20Behaviour%20Dashboard.png)

---

## Business Impact & Recommendations

- Tighten monitoring on **Cash Advance-heavy accounts**, which show the strongest link to risk
- Prioritize re-engagement campaigns for the **2,044 inactive customers** before they become lost
- Use the **"At Risk" segment** as the primary target for proactive credit interventions
- Leverage the **Purchases–Payments correlation** to identify healthy repayment behavior as a positive risk signal

---

🔗 [LinkedIn](https://linkedin.com/in/saqib-amin-31b1ba2a1/) 

---

⭐ If you found this project useful, consider giving it a star on GitHub!
