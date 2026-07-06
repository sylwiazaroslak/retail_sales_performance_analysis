# Retail Sales Performance Analysis Project

## Project Overview
This repository contains a comprehensive data analytics project designed for a multi-regional retail chain. Taking on the role of a Lead Retail Analyst, the objective is to fulfill a directive from the Chief Financial Officer (CFO): evaluate historical sales performance, analyze profitability drivers, uncover operational inefficiencies, and deliver an executive-ready interactive reporting asset.

The final deliverable is an optimized, multi-tab Excel workbook built from disparate data sources, serving as a single source of truth for strategic decision-making.

---

## 📊 Executive Summary & Key Findings
* **Predictable Cyclical Seasonality:** Time-series tracking from 2014–2017 confirms a repeating seasonal wave pattern. Every fiscal year opens at a sharp cyclical deficit in Q1 (post-holiday market contraction) before reaching an explosive revenue peak in Q4 driven by holiday retail surges and end-of-year procurement cycles.
* **Portfolio Profitability Gaps:** While the **Technology** segment acts as the core driver for high-value revenue and margin expansion, **Furniture** generates significant top-line sales volume but suffers from lower net margin conversion due to high shipping overhead and steep promotional discounting.
* **Statistical Accountability Tie:** A Two-Sample $t$-Test assuming unequal variances was deployed to compare the 2017 Average Order Value (AOV) of the Central Region ($186.62) against the East Region ($223.57). The resulting two-tailed $p$-value of **0.2562** proves that the difference is statistically insignificant and mathematically driven by a few "whale" transactions, establishing a performance tie between the regions.

---

## Data Architecture & Schema
The project consolidates three distinct relational tables contained within the source workbook:
1. **`orders` Table:** The core transactional ledger containing granular item-level records for every sale (Gross Revenue, Product Hierarchy, Segment, Shipping Mode, and Net Profit).
2. **`people` Table:** An organizational lookup mapping regional business territories to human resource leadership.
3. **`returns` Table:** An operational exception ledger tracking post-purchase transaction reversals.

---

## Analytical Workflow
The analytics dashboard is structured into four core functional investigative layers:

### 1. Macro-Level Sales & Seasonality Analysis
- Plotted historical revenue data alongside linear trend lines to prove sustained upward business expansion.
- Established the baseline for seasonal multiplicative smoothing methods to preserve capital efficiency in budgeting.

### 2. Segment Analysis & Profitability Impact
- Profiled product categories to isolate high-frequency transaction drivers (**Office Supplies**) from high-overhead margin diluters (**Furniture**).

### 3. Regional Operational Efficiency
- Formulated an independent two-sample hypothesis test ($t$-test) to compare operational efficiency across regional management structures ($n=406$ for Central vs. $n=470$ for East).

### 4. Financial Simulation & Incentive Optimization
- Constructed a dynamic **Two-Way Data Table** (What-If scenario matrix) to simulate corporate financial exposures across variable salesperson bonus tiers, annual employee turnover rates, and regional sales outputs.

---

## Technical Skills Applied
- **Advanced Statistical Analysis:** Executing Independent Two-Sample $t$-Tests, interpreting two-tailed $p$-values, and modeling variance disparities.
- **Financial Simulation & Modeling:** Building interactive What-If Scenarios and multi-variable Two-Way Data Tables.
- **Data Summarization & Architecture:** Managing relational lookups, advanced calculations, and dynamic pivot architectures inside Excel.

---

## How to Use This Repository
1. **Open the Workbook**: Open `retail_sales_performance_analysis.xlsx` to view the interactive tables and financial calculation models.
2. **Review the Models**: Navigate to the `Calculations` and `Final_report` sheets to inspect the hypothesis test parameters and simulation matrices.
3. **Interact with Filters**: Utilize regional slicers to dynamic filter transaction-level data across human resource hierarchies.
