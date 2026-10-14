# Loan Default Risk Analysis

## Project Overview
This project analyzes 255,347 loan records to understand how observed loan default rates vary across borrower characteristics, credit profiles, financial indicators, and loan characteristics.

The goal is to identify segments with relatively higher observed default rates and highlight areas for further credit-risk investigation.

## Business Problem
Banks need to understand how loan default patterns vary across borrower and loan segments to support risk monitoring and informed lending decisions.

## Project Objectives
- Analyze default rates across borrower demographics and employment characteristics.
- Examine associations between credit scores, debt-to-income ratio, and loan defaults.
- Investigate how loan amount, interest rate, loan term, and loan purpose relate to observed default rates.
- Identify segments with relatively higher observed default rates.
- Communicate findings through a Power BI dashboard.

## Tools and Technologies
- Python
- Pandas
- Jupyter Notebook
- Power BI

## Key Performance Indicators (KPIs)
- Total Loans
- Defaulted Loans
- Observed Default Rate
- Average Loan Amount
- Estimated Expected Loss

## Key Findings

### 1. Overall Portfolio
The dataset contains 255,347 loan records, with an overall observed default rate of approximately 11.62%.

### 2. Loan Amount and Interest Rate
The segment with loan amounts of 200K+ and interest rates of 20%–25% had an observed default rate of 23.59%, compared with 4.08% for loans of 0–50K with interest rates of 2%–5%.

### 3. Age and Credit Score
Borrowers aged 18–30 in the Low Credit Score group had an observed default rate of 21.76%. The rate for borrowers aged 61+ in the High Credit Score group was 4.33%.

### 4. Employment and Income
Within the 200K+ loan amount and 20%–25% interest rate segment, unemployed borrowers had an observed default rate of 27.07%. Within this unemployed subgroup, the Low Income group had a rate of 43.49%.

### 5. Deeper Risk Segmentation
Within the Low Income, Unemployed, 200K+ Loan Amount, and 20%–25% Interest Rate segment, borrowers in the Low Credit Score group had an observed default rate of 48.13%.

## Power BI Dashboard
The dashboard contains two pages:

- **Portfolio Overview:** Overall KPIs and default-rate comparisons across income, age, credit score, and employment type.
- **Credit Risk & Risk Segmentation:** Loan amount and interest rate analysis, credit score and DTI comparisons, DTI group analysis, and income segmentation within a higher-risk loan segment.

## Business Implications
The findings highlight segments that may warrant further credit-risk investigation and monitoring. These patterns should not be used as the sole basis for automatically rejecting borrowers.

## Limitations
- The findings are based on the available dataset and may not represent every lending environment.
- Observed associations do not establish causation.
- The Expected Loss estimate uses an assumed Loss Given Default (LGD) of 60%.
- The simplified Expected Loss calculation does not use individual loan-level default probabilities or actual outstanding balances.
- The observed risk patterns require further validation before being used in lending decisions.

## Conclusion
This project demonstrates how Python-based analysis and Power BI visualization can help explore loan default patterns, compare borrower and loan segments, and communicate findings relevant to credit-risk monitoring.
