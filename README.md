# JPMorgan Chase Quantitative Research
# Job Simulation — Forage

## Overview
Completed the JPMorgan Chase & Co. Quantitative Research Virtual Job Simulation on Forage. The simulation involved four end-to-end quantitative finance tasks spanning commodity price forecasting, derivative contract valuation, credit risk modelling, and FICO score optimization — closely mirroring real-world problems tackled by JPMorgan's Quantitative Research division. An interactive Power BI dashboard was also built from scratch on the loan dataset to visualize credit risk insights across 10,000 borrowers.

## Tasks Completed
- Task 1: **Natural Gas Price Forecasting** — Built a Trend + Seasonality regression model using scipy to estimate natural gas prices at any given date and produce a 12-month forward forecast
- Task 2: **Storage Contract Pricing** — Developed a prototype pricing engine to calculate the net value of a natural gas storage contract given arbitrary injection and withdrawal schedules, yielding a net contract value of $1,081,648.47
- Task 3: **Credit Risk Modelling** — Trained Logistic Regression and Random Forest models (AUC: 1.0000 and 0.9997) to predict Probability of Default and estimate Expected Loss per borrower using the formula EL = PD × Loan Amount × LGD
- Task 4: **FICO Score Quantization** — Implemented a dynamic programming solution to optimally bucket FICO scores (300–850) into 10 discrete rating categories using Log-Likelihood Maximization, identifying key risk frontiers in the credit score distribution

## Dashboard Highlights
- 10,000 loan records analyzed
- 18.51% overall default rate identified
- 3-page interactive Power BI dashboard built from scratch
- 10 custom DAX measures created including Default Rate %, Total Loan Exposure ($41.6M), and Debt-to-Income Ratio
- Cross-segment risk matrix built across FICO Tier × Income Band combinations
- Key risk factors: FICO Score, Tenure, Income

## Tools Used
- Python (Pandas, NumPy, Matplotlib, SciPy)
- Scikit-Learn (Logistic Regression, Random Forest)
- Power BI Desktop
- DAX (Data Analysis Expressions)

## Key Insights
- Tenure-0 customers default at 69% vs near 0% for Tenure 9-10
- FICO Score is the strongest individual default predictor
- Lower income bands show significantly higher default rates
- High debt-to-income ratio and open credit lines increase default risk
- ~$7.7M of the total $41.6M loan portfolio is in defaulted accounts
- Log-Likelihood bucketing outperforms MSE for credit risk segmentation
