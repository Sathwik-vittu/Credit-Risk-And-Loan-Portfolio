# Credit-Risk-And-Loan-Portfolio
## 📌 Project Overview
This project provides a comprehensive analysis of a bank's lending activities to monitor portfolio health and track Key Performance Indicators (KPIs). By processing over 38,000+ loan applications, I developed an end-to-end analytics solution that tracks funding, repayments, and risk metrics (Good vs. Bad Loans) to support data-driven lending strategies.

## 📊 Dashboard Preview
**TABLEAU** : https://public.tableau.com/app/profile/sathwik.reddy.nalla/viz/CreditRiskLoanPortfolio/SUMMARY

## 💼 Business Problem (The "Why")
Lending institutions face significant risk if they cannot monitor their loan portfolio in real-time. This project addresses:
- **Liquidity Tracking:** Monitoring the gap between "Total Funded Amount" and "Total Amount Received."
- **Risk Categorization:** Distinguishing between "Good Loans" (Fully Paid/Current) and "Bad Loans" (Charged Off) to protect the bank's capital.
- **Trend Identification:** Tracking Month-over-Month (MoM) changes in applications and interest rates to adjust to market shifts.

## 🛠️ Technical Implementation
- **Data Source:** 38.5k+ records of anonymized financial loan data.
- **SQL Analysis:** Engineered complex queries to calculate MTD (Month-to-Date) and PMTD (Previous Month-to-Date) metrics. Used DENSE_RANK, GROUP BY, and WINDOW functions to segment data by State, Term, and Purpose.
- **Visualization:** Developed a 3-page interactive dashboard:
  - **Summary:** High-level KPIs (Total Apps, Funded, Received).
  - **Overview:** Visual trends by Grade, Purpose, and Home Ownership.
  - **Details:** Granular drill-down into individual borrower profiles.

  ## 📊 Key Metrics & KRIs (Key Risk Indicators)
- **Good Loan%** = (Fully paid + current)/Total Loans. Measures the overall health of the landing book.
- **Bad Loan%** = Charged off/Total Loans. Tracks the loss rate and capital at risk.
- **DTI Ratio** = Debt-to-Income. Evaluates the borrower's repayment capacity.
- **Average Interest Rate** = Weighted Avg across portfolio. Monitors the bank's primary revenue driver.

## 📈 Insights & Recommendations
- **Regional Concentration:** Identified specific states (e.g., CA, TX, NY) with high application volumes but varying default rates, suggesting a need for region-specific credit tiering.
- **Purpose Analysis:** Debt consolidation and credit card refinancing remain the primary drivers of loan volume; however, smaller categories like "small business" show higher risk volatility.
- **Term Strategy:** 36-month loans show higher repayment stability compared to 60-month terms, providing an opportunity to incentivize shorter-term lending.

## 📂 Repository Structure
- **Bank_finance_dataset.csv**: The raw dataset used for analysis.
- **SQL Queries.doc**: Production-ready SQL scripts for KPI calculation.
- **Domain.doc:** Deep-dive into banking terminology used (LTV, DTI, Amortization).
