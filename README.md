# Restaurant Profitability & Discount Burn Analysis Dashboard

**Power BI | Business Intelligence | Financial Analysis | Profitability Optimization**

An interactive Power BI project designed to evaluate restaurant-level financial performance, analyse discount expenditure, monitor SUB, and investigate gross margin drivers in a food-delivery business.

## Project Overview

This project explores how financial and operational data can be transformed into actionable business insights through an interactive Power BI dashboard.

Using a synthetic food-delivery financial dataset, the analysis focuses on the relationship between restaurant commission earnings, platform-funded discounts, delivery fees, rider earnings, payment settlement charges, and gross margin.

The objective is to identify potentially unprofitable business segments, investigate discount efficiency, understand margin drivers, and support better financial and operational decision-making.

**Data disclaimer:** This is an independent portfolio project built using synthetic/generated data. The figures and business scenarios are illustrative, not actual company financial results. This project is not an official Pathao report and is not affiliated with Pathao.

## Business Problem

High order volume does not necessarily translate into healthy profitability. Commission revenue can be offset by platform-funded promotions, while delivery costs and payment settlement charges can further reduce the contribution earned from each order.

This project addresses the following business questions:

- Are restaurant commission earnings sufficient to cover platform-funded discounts?
- Which restaurants and restaurant groups show relatively high discount burn?
- Which business segments have weak or negative SUB?
- How do rider earnings and delivery fee recovery affect gross margin?
- Which restaurants, zones, or payment methods require further financial investigation?
- How can management identify opportunities to improve profitability without unnecessarily sacrificing order volume?

## Project Objectives

- Measure restaurant-level commission earnings and discount expenditure.
- Calculate SUB to evaluate commission earnings after platform-funded discounts.
- Analyze gross margin and its underlying financial components.
- Compare restaurant, chain, and zone performance.
- Monitor monthly financial trends and changes in profitability.
- Identify potential profit leakages and financial anomalies for further investigation.
- Translate analytical observations into practical business recommendations.

## Dashboard 1: SUB & Discount Efficiency Analysis

### Objective

Evaluate how much commission remains after deducting platform-funded promotions and vouchers, and identify restaurant segments requiring further commercial review.

### Core Calculation

**SUB = Restaurant Commission Amount − Discount Funded by the Platform**

In this project, SUB is a defined analytical measure rather than final business profit.

### Key Metrics

- Total Commission Earned
- Total Platform-Funded Discount Burn
- Total SUB
- Discount Burn Percentage
- SUB Margin Percentage
- SUB per Order

### Analysis Performed

- Compare restaurant commission earnings with discount expenditure.
- Rank restaurants by SUB and discount burn.
- Identify restaurants with high discount burn relative to commission.
- Compare SUB across restaurants, chains, and zones.
- Track monthly SUB trends.
- Investigate high-volume restaurants with weak SUB per order.
- Evaluate promotion and voucher performance using the available financial measures.

### Business Value

This analysis supports the investigation of potentially inefficient discount spending, unfavourable restaurant economics, and opportunities to review promotion structures or commercial arrangements.

High discount burn is treated as a signal for investigation, not automatic evidence that a restaurant or promotion is unprofitable.

## Dashboard 2: Gross Margin & Profit Leakage Analysis

### Objective

Understand how commission revenue, discount expenditure, delivery fees, rider earnings, platform fees, and payment settlement charges contribute to overall gross margin.

### Gross Margin Calculation

Gross Margin = Restaurant Commission Amount − Platform-Funded Discount + Delivery Fee + Platform Fee − Rider Earnings − Online Settlement Charges

### Key Metrics

- Total Gross Margin
- Gross Margin per Order
- Gross Margin Percentage
- Delivery Fee Revenue
- Rider Cost
- Settlement Cost
- Delivery Cost Gap
- Negative-Margin Order Count

### Analysis Performed

- Decompose gross margin using a waterfall chart.
- Compare monthly gross margin trends.
- Analyse profitability across restaurant chains and branches.
- Investigate zones with relatively weak margin per order.
- Compare delivery fee recovery with rider earnings.
- Examine payment settlement costs across payment methods.
- Identify individual orders and business segments with negative gross margin.
- Reconcile the gross margin calculation against its underlying financial components.

### Business Value

This analysis helps explain why a business segment may generate commission revenue but contribute relatively little margin after the costs included in the model.

It supports further investigation of delivery subsidy exposure, discount expenditure, payment costs, and restaurant-level financial performance.

## Additional Analytical Opportunities

The dataset also supports the development of:

- **Restaurant Portfolio Segmentation:** Classify restaurants by order volume, SUB, and gross margin to distinguish strong contributors from segments requiring review.
- **Promotion Efficiency Analysis:** Compare commission, platform-funded discount burn, SUB, and gross margin across available promotion and voucher names.
- **Zone-Level Economics:** Evaluate delivery fee recovery, rider cost per order, and gross margin across zones.
- **Payment Cost Analysis:** Compare settlement charges and margin across customer payment methods.
- **Month-over-Month Performance Analysis:** Identify changes in commission, discount expenditure, delivery costs, and gross margin.
- **Financial Reconciliation Monitoring:** Investigate discrepancies, duplicated amounts, missing values, and inconsistent financial records.
- **Basket Value Analysis:** Examine the relationship between food value, order size, discount burn, and margin per order.

These analyses are intended to generate testable business hypotheses. Any recommendations require validation against reliable financial and operational data.

## Technical Skills Demonstrated

### Power BI & Data Modeling
- Interactive dashboard development
- KPI cards, slicers, drill-downs, and cross-filtering
- Financial performance visualisation
- Data modelling and date-based analysis

### DAX & Analytical Measures
- Calculated columns and measures
- Financial aggregations and ratio calculations
- SUB and gross margin calculations
- Per-order performance metrics
- Time-intelligence calculations, where implemented
- Financial reconciliation measures

### Business & Financial Analysis
- Profitability and contribution analysis
- Discount burn monitoring
- Restaurant and zone performance evaluation
- Cost-driver analysis
- Root-cause investigation
- Data-driven business recommendations

## Repository Contents

- `README.md` — Project overview, methodology, metrics, and business objectives
- `images/dashboard-preview.png` — Dashboard screenshot
- `powerbi/` — Power BI report file, if shared
- `data/` — Synthetic sample dataset, if shared
- `docs/` — KPI definitions and calculation methodology, if included

## Data Quality & Methodology

Before interpreting profitability results, the analysis should establish the financial dataset's grain, verify that order-level amounts are not duplicated, confirm discount funding responsibility, and reconcile gross margin against its components.

The gross margin measure represents the formula defined for this project. It should not be interpreted as audited accounting gross profit without confirmation of the company's accounting policies and financial definitions.

The dataset contains synthetic values, so do not present analytical patterns as verified findings about a real food-delivery business.

## Project Outcome

The project demonstrates how a financial dataset can be structured into an interactive business intelligence solution that connects revenue, discount expenditure, delivery economics, and margin performance.

It highlights how analytical thinking identifies potential business risks, investigates financial drivers, and supports better-informed decisions.

## Author

**Power BI | Business Intelligence | Financial & Business Analysis**

Focused on transforming business data into meaningful insights that support profitability analysis, performance evaluation, and strategic decision-making.
