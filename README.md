# Restaurant Profitability & Discount Burn Analysis Dashboard

**Power BI | Business Intelligence | Financial Analysis | Profitability Optimization**

An interactive Power BI dashboard designed to evaluate restaurant-level profitability, monitor discount efficiency, identify potential profit leakages, and support data-driven financial decisions in a food-delivery business.

## Project Overview

This project transforms synthetic food-delivery financial data into an interactive business intelligence solution focused on restaurant profitability and financial performance.

The dashboard analyses restaurant commission earnings, platform-funded discounts, SUB, delivery fee revenue, rider earnings, settlement charges, and gross margin to understand how revenue and costs affect business contribution.

Rather than focusing solely on order volume and sales, the project emphasises a more important business question:

**How much financial contribution does the platform retain after funding discounts and covering the costs included in its margin calculation?**

The dashboard is structured around two core analytical areas:

- **SUB & Discount Burn Analysis:** Evaluates commission earnings against platform-funded discounts to identify restaurants with different levels of discount exposure.
- **Gross Margin & Profitability Analysis:** Examines how revenue and cost components affect overall margin and highlights areas requiring further financial investigation.

The objective is to help business stakeholders move beyond performance reporting toward identifying risks, investigating root causes, and evaluating opportunities to improve profitability.

> **Data Disclaimer:** This is an independent portfolio project built using synthetic/generated data. All figures and business scenarios are illustrative and do not represent actual Pathao financial or operational performance. This project is not an official Pathao dashboard and is not affiliated with Pathao.

## Business Problem

A food-delivery platform can generate substantial order volume and commission revenue while experiencing weak profitability due to promotional spending, delivery subsidies, and payment processing costs.

Without a structured financial monitoring system, it can be difficult to determine:

- Which restaurants consume a disproportionately high share of commission earnings through platform-funded discounts.
- Which restaurant segments generate positive or negative SUB.
- Whether high order volume translates into sustainable gross margin.
- Which zones or restaurant chains have relatively weak financial performance.
- How delivery costs and settlement charges affect the platform's contribution per order.
- Where management should prioritise financial investigation and commercial improvements.

This project addresses these challenges by consolidating key financial indicators into interactive dashboards that support restaurant-level comparisons, risk segmentation, margin analysis, and performance monitoring.

## Project Objectives

- Measure commission earnings against platform-funded discount expenditure.
- Calculate SUB to assess commission remaining after platform-funded promotions.
- Classify restaurants according to discount burn levels using a four-tier risk framework.
- Identify restaurants requiring closer review based on discount exposure and financial contribution.
- Analyse gross margin and its underlying revenue and cost components.
- Compare financial performance across restaurant branches, chains, zones, and time periods.
- Investigate potential delivery-cost, discount-efficiency, and settlement-related profit leakages.
- Translate financial analysis into actionable recommendations for business improvement.

# Dashboard 1: SUB & Discount Burn Analysis

## Objective

Evaluate how efficiently restaurant commission earnings cover platform-funded discounts and identify restaurants that may require changes to promotional strategies or commercial arrangements.

## Key Financial Metric: SUB

**SUB = RestaurantCommissionAmount − DiscountByPathao**

Where:

- `RestaurantCommissionAmount` represents commission earned by the platform from restaurants.
- `DiscountByPathao` represents platform-funded promotional and voucher discounts.

SUB measures the commission remaining after deducting platform-funded discounts. It is a contribution indicator, not the final gross margin or net profit.

## Burn% Calculation

**Burn% = (DiscountByPathao ÷ RestaurantCommissionAmount) × 100**

Burn% indicates the proportion of commission earnings consumed by platform-funded discounts.

For example, if commission earnings are ৳100,000 and platform-funded discounts are ৳75,000, the Burn% is 75%, leaving a SUB of ৳25,000.

## Burn% Risk Classification

The dashboard includes an interactive Burn% filter that segments restaurants into four categories to support targeted financial investigation.

| Category | Burn% Range | Business Interpretation |
|---|---|---|
| Healthy | Below 50% | Less than half of commission earnings are consumed by platform-funded discounts. |
| Watch | 50% to below 80% | Discount expenditure is consuming a substantial share of commission and warrants monitoring. |
| Risky | 80% to 100%, inclusive | Most or all commission earnings are consumed by discounts, leaving limited or no SUB. |
| Loss Making | Above 100% | Platform-funded discounts exceed commission earnings, resulting in negative SUB for the measured scope. |

**Classification rule:** Burn% below 50% is Healthy; 50% to below 80% is Watch; 80% through 100% is Risky; and above 100% is Loss Making.

These categories describe discount exposure relative to commission, not overall business profitability. A restaurant classified as Healthy can still generate negative gross margin after delivery and other costs. Conversely, a restaurant with high Burn% may have additional revenue or commercial benefits that warrant further analysis.

Orders or restaurants with zero commission require separate handling because their Burn% is undefined or not meaningful. They should not automatically be classified as Healthy.

## Key Metrics

- Total Commission Earned
- Total Platform-Funded Discount Burn
- Total SUB
- Discount Burn Percentage
- SUB Margin Percentage
- SUB per Order
- Restaurant-Level SUB Ranking

## Analytical Approach

### 1. Restaurant-Level Commission vs. Discount Comparison

Compare commission earnings and platform-funded discount expenditure across restaurants and chains to identify segments where discount spending consumes a substantial proportion of commission.

### 2. Burn% Risk Segmentation

Use the four-category Burn% filter to isolate Healthy, Watch, Risky, and Loss Making segments.

This allows stakeholders to move from an overall financial overview to a focused investigation of restaurants with elevated discount exposure.

### 3. Restaurant and Chain Ranking

Rank restaurants by SUB, Burn%, and SUB per order to distinguish high-contribution restaurants from those requiring financial review.

### 4. Monthly SUB Trend Analysis

Monitor how commission earnings, discount expenditure, and SUB change over time to identify deteriorating or improving discount efficiency.

### 5. High-Volume, Low-Contribution Investigation

Identify restaurants that generate substantial order volume but contribute relatively little SUB. These restaurants may warrant further investigation into discount structure, commission arrangements, and order-level economics.

## Business Problems This Dashboard Helps Investigate

- Excessive platform-funded discounts relative to commission earnings.
- Restaurants with negative SUB.
- Restaurant chains with inconsistent discount efficiency across branches.
- High-volume restaurants with weak SUB per order.
- Deteriorating SUB performance over time.
- Potential opportunities to review promotion rules, voucher funding, and commercial agreements.

## Potential Business Actions

The findings can support targeted actions such as reviewing promotion eligibility, evaluating discount-sharing arrangements, setting campaign-level financial limits, and negotiating improved commercial terms.

The objective is not to reduce every discount indiscriminately, but to identify where promotional expenditure may be disproportionate to the financial contribution generated.

# Dashboard 2: Gross Margin & Profitability Analysis

## Objective

Evaluate the contribution remaining after accounting for the revenue and cost components included in the project's gross margin calculation.

## Gross Margin Calculation

**Gross Margin = Restaurant Commission Amount − Discount by Pathao + Delivery Fee + Platform Fee − Rider Earnings − Online Settlement Charges**

The dashboard breaks down these components to explain the financial drivers of overall margin.

This is the project's defined gross margin measure and should not be interpreted as audited accounting gross profit without validation against the company's accounting policies.

## Key Performance Indicators

- Total Gross Margin
- Gross Margin per Order
- Gross Margin Percentage
- Delivery Fee Revenue
- Rider Cost
- Online Settlement Cost
- Delivery Cost Gap
- Negative-Margin Order Count

## Analytical Approach

### 1. Margin Bridge Analysis

Use a waterfall chart to show how commission, discounts, delivery fees, platform fees, rider earnings, and settlement charges contribute to gross margin.

This helps explain which financial components are increasing or reducing contribution.

### 2. Monthly Gross Margin Monitoring

Track gross margin over time to investigate whether changes are associated with increasing discount expenditure, lower commission earnings, higher rider costs, or other changes in the financial mix.

### 3. Restaurant and Chain Profitability

Compare gross margin and gross margin per order across restaurant branches and chains to identify strong contributors and segments requiring further review.

### 4. Zone-Level Delivery Economics

Compare customer delivery fees with rider earnings across zones and rider types to investigate potential delivery subsidy exposure.

### 5. Payment Settlement Cost Analysis

Examine online settlement charges across payment methods to identify differences in transaction costs and investigate potential savings opportunities.

### 6. Negative-Margin Investigation

Identify orders or business segments with negative gross margin and examine the underlying commission, discount, delivery fee, rider earnings, and settlement components.

## Potential Profit Leakages to Investigate

- Platform-funded discounts exceeding commission earnings.
- Delivery fees insufficient to cover rider earnings.
- High order volume accompanied by weak gross margin per order.
- Restaurant branches with consistently weak contribution.
- Settlement costs that materially reduce margin.
- Unexpected discrepancies between calculated gross margin and its underlying financial components.

These are potential investigation areas rather than confirmed financial losses. Any identified issue should be validated against the underlying transactions and financial definitions before action is taken.

# Additional Analytical Opportunities

The dataset provides a foundation for extending the dashboard into a broader profitability monitoring solution.

| Analysis | Business Purpose |
|---|---|
| Restaurant Portfolio Segmentation | Categorise restaurants by order volume, SUB, and gross margin to prioritise investigations. |
| Promotion & Voucher Efficiency | Compare commission, discount burn, SUB, and gross margin by promotion or voucher. |
| Zone-Level Unit Economics | Identify zones with weak delivery fee recovery or low margin per order. |
| Branch Performance Comparison | Compare branches within the same restaurant chain to identify operational or commercial differences. |
| Month-over-Month Margin Decomposition | Explain changes in profitability through changes in revenue and cost components. |
| Payment Cost Analysis | Compare settlement charges and margin across payment methods. |
| Financial Reconciliation Monitoring | Investigate missing, duplicated, or inconsistent financial amounts. |
| Basket Value & Contribution Analysis | Examine the relationship between order value, discount expenditure, and margin per order. |

These extensions can help connect financial reporting with operational investigation and continuous performance improvement.

# Technical Skills Demonstrated

## Power BI & Data Visualization
- Interactive dashboard development
- KPI cards, slicers, and cross-filtering
- Restaurant and chain performance comparisons
- Trend analysis and waterfall visualisation
- Financial risk segmentation

## DAX & Analytical Calculations
- Calculated columns and measures
- SUB and gross margin calculations
- Burn% classification logic
- Ratio and per-order KPI development
- Financial reconciliation measures
- Time-based comparisons, where implemented

## Business & Financial Analysis
- Commission and discount efficiency analysis
- Profitability and contribution analysis
- Cost-driver investigation
- Restaurant and zone performance evaluation
- Financial risk identification
- Data-driven business recommendations

# Project Methodology & Data Quality

Reliable profitability analysis requires more than visualisation. The following validation principles are important to this project:

- Confirm whether each financial record represents an order, order item, or transaction.
- Prevent duplicate aggregation of order-level financial amounts.
- Validate the funding responsibility of each discount component.
- Handle zero or missing commission values appropriately in Burn% calculations.
- Reconcile gross margin against its underlying revenue and cost components.
- Define whether financial performance is analysed by order creation date or delivery date.
- Distinguish observed associations from proven causal effects.

The project uses synthetic/generated data. Its results demonstrate an analytical approach and should not be interpreted as actual company performance.

# Project Outcome

This project demonstrates how financial data can be transformed into an interactive business intelligence solution that supports:

- Structured monitoring of restaurant-level financial performance.
- Identification of high discount-burn and negative-SUB segments.
- Investigation of delivery and settlement cost drivers.
- Comparison of SUB and gross margin to understand broader order economics.
- Prioritisation of financial issues for further investigation.
- More informed decisions around promotional expenditure and profitability improvement.

The central objective is to move beyond descriptive reporting and develop a structured approach to identifying financial risks, investigating their drivers, and evaluating potential
