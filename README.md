# Non-Performing Loan Analytics

A Power BI report for **Non-Performing Loan (NPL)** analysis for a microfinance context — built to help finance managers and senior leadership monitor portfolio health, risk, and recovery performance.

## What this solves
Microfinance teams need fast answers to questions like:
- What’s driving NPL growth — product, branch, cohort, or customer segment?
- How is **PAR** trending (PAR30/PAR60/PAR90) and where is it concentrated?
- Are collections improving, or are we just reshuffling risk?
- What’s the impact of restructures, write-offs, and recoveries on the portfolio?

## Key report
1. **Executive Overview**  
   Portfolio KPIs, PAR trends, NPL movement, top risk hotspots.
2. **Portfolio Quality & Risk**  
   PAR buckets, vintage/cohort risk, segment & geography breakdowns.
3. **Delinquency & Roll Rates**  
   Roll-forward / roll-back behavior, early warning signals.
4. **Collections & Recoveries**  
   Recovery rate, cure rate, collections performance by team/strategy.
5. **Restructures, Write-offs & Exposure**  
   Restructures effectiveness, write-off trend, EAD exposure and concentration.

## Data model 
**Fact tables**
- `fact_loans` — loan-level attributes + status snapshots
- `fact_repayments` — repayment transactions / schedules
- `fact_collections` — call/visit outcomes, promises to pay, recovery actions
- `fact_writeoffs` — write-off events and amounts

**Dimensions**
- `dim_customer`, `dim_branch`, `dim_product`, `dim_date`, `dim_loan_status`, `dim_bucket`

## Metrics included
- Portfolio Outstanding / Exposure at Default (EAD)
- NPL Ratio
- PAR30 / PAR60 / PAR90
- Roll rate (bucket-to-bucket movement)
- Cure rate / Recovery rate
- Write-off rate
- Restructure success rate

## 🛠️ Tech stack
- Power BI (data model + visuals)
- Power Query

