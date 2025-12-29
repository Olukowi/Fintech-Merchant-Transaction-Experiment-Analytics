# Fintech-Merchant-Transaction-Experiment-Analytics
This project is a product analytics case study simulating a fintech payments platform.   The objective was to analyze merchant transaction behavior and evaluate the impact of a transaction fee reduction using SQL and Python.

[generate_payment_datav3.ipynb](https://github.com/user-attachments/files/24374708/generate_payment_datav3.ipynb)


The project focuses on:
- Merchant transaction growth
- Revenue trade-offs
- Experiment (A/B test) design and analysis

---

## Business Context
Merchants were split into two groups:
- **Control group**: standard transaction fee (1.5%)
- **Variant group**: reduced transaction fee (1.0%)

The key business question:
> *Does reducing transaction fees increase merchant activity enough to justify the revenue impact?*

---

## Data Generation
- Synthetic merchant and transaction data was generated using Python (Pandas, NumPy).
- The dataset includes:
  - Merchant onboarding information
  - Transaction amounts, dates, and payment channels
  - Experiment group assignment (control vs variant)
- Merchant behavior was designed to reflect real-world patterns such as:
  - Different merchant sizes
  - Churn and inactivity
  - Increased activity for variant merchants

---

## SQL Analysis
SQL was used to answer core product and business questions, including:
- Monthly transaction and revenue trends
- Control vs variant transaction activity
- Pre- and post-experiment performance comparison

Key SQL concepts demonstrated:
- Joins
- Aggregations
- Common Table Expressions (CTEs)
- CASE logic for time-based analysis

---

## Experiment & Statistical Testing (Python)
To validate experiment outcomes:
- Merchant-level metrics were calculated using Pandas
- Independent t-tests (SciPy) were applied to compare control and variant groups
- Metrics tested included:
  - Transactions per merchant
  - Revenue per merchant

This approach avoids transaction-level bias and reflects user-level impact.

---

## Key Findings
- Merchants in the reduced-fee variant showed higher transaction activity.
- Average revenue per transaction declined due to lower fees.
- Statistical testing confirmed that observed differences were statistically significant.
- The experiment highlights a trade-off between engagement growth and revenue optimization.

---

## Tools Used
- SQL (SQLite)
- Python (Pandas, SciPy)
- Jupyter Notebook
- Power BI (dashboard visualization)

---

## Dashboard
An executive-facing Power BI dashboard was created to summarize insights and experiment outcomes.

