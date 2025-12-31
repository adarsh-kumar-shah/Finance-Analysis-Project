# Finance-Analysis-Project

# 📌 Executive Overview
This project involved the development of a high-impact Financial Intelligence System designed to provide a 360-degree view of the organization's fiscal health. By synthesizing revenue streams, liquidity metrics, and operational costs, the dashboard serves as a "single source of truth" for stakeholders to evaluate growth trajectories and budget adherence.

# 📈 Financial Scorecard (Key Performance Indicators)

| Metric | Performance | Business Context |
| :--- | :--- | :--- |
| **Gross Margin %** | `45.55%` | Robust baseline profitability; strong cost-of-goods management. |
| **EBITDA Margin** | `24.81%` | Healthy operational efficiency with a focus on core earnings. |
| **Annual Revenue** | `$23.6M` | Total top-line scale for the fiscal period. |
| **Net Cash Position** | `$0.69M` | Solid liquidity buffer after all inflows and expenditures. |
| **Growth Velocity** | `4.18% MoM` | Consistent monthly expansion, peaking in Q4. |

# 🔍 Strategic Insights & Analytical Findings
Revenue & Budget Dynamics
Target Alignment: Using clustered column analysis, the project tracked the variance between Actuals vs. Budgets, revealing high precision in financial forecasting.

Peak Performance: Revenue reached its zenith in December, driven by seasonal product demand and aggressive sales cycles.

Portfolio Strength: Product C and Service X emerged as the primary revenue engines, whereas Product A was identified as a candidate for strategic reassessment.

Liquidity & Working Capital
Cash Flow Narrative: A Waterfall Chart was utilized to visualize the bridge between opening and closing cash, highlighting disciplined expense control.

Collection Efficiency: The Accounts Receivable (AR) Aging remains optimized, with a collection cycle of 26–31 days, ensuring a steady stream of working capital.

# 🛠 Technical Architecture
Data Engineering Stack
Power Query & Excel: Executed complex data ETL (Extract, Transform, Load) to normalize financial records and prepare the schema for modeling.

Power BI: Architected the visual layer, focusing on a balance between high-level KPIs and granular drill-down capabilities.

Advanced DAX Logic
The backbone of the analysis consists of custom Data Analysis Expressions (DAX) to handle time intelligence and ratio calculations:

Profitability Ratios: Dynamic calculation of Gross Margin and EBITDA percentages to assess operational health.

Time Intelligence: Utilized TOTALYTD for cumulative performance tracking and VAR logic to calculate Month-over-Month (MoM) growth shifts.

Liquidity Tracking: Aggregated net cash flows to monitor real-time solvency.

# 💡 Strategic Recommendations
Margin Optimization: Investigate overhead costs to push the 24.81% EBITDA closer to the 30% mark.

Asset Allocation: Redirect surplus cash reserves into the R&D of Product C to capitalize on its high market traction.

Credit Policy Maintenance: Continue the current 30-day collection standard to prevent liquidity bottlenecks.

# 🚧 Challenges Overcome
When presenting these projects, employers love to see how you solved problems. Here are the most common technical hurdles for these specific dashboards and how you addressed them:

1. Handling Granular Time Intelligence
The Challenge: Calculating Week-over-Week (WoW) and Month-over-Month (MoM) growth is difficult when dates are missing or when comparing incomplete current periods to previous ones.

The Solution: I developed a custom Date Table and utilized advanced DAX variables (VAR) to isolate current and previous periods. This ensured that growth percentages remained accurate even when filtering by specific regions or card categories.

2. Data Normalization & Relationship Mapping
The Challenge: Merging transaction-level data with static customer demographics often leads to "Many-to-Many" relationship errors or data inflation.

The Solution: I utilized Power Query to clean and de-duplicate customer records, establishing a clean Star Schema with a 1:Many relationship. This optimized the dashboard's performance, ensuring visuals refreshed instantly even with large datasets.

3. Balancing KPI Density with UI Clarity
The Challenge: Financial dashboards often become cluttered with too many numbers, making it hard for executives to find the "Bottom Line."

The Solution: I implemented a hierarchical design approach. I placed high-level KPIs (Total Revenue, Net Cash) at the top for immediate impact, used Slicers for interactive deep-dives, and employed Waterfall charts to explain the movement of cash rather than just the final balance.

4. Managing Variance Analysis (Budget vs. Actual)
The Challenge: Budget data is often at a monthly level, while Actuals are at a daily level, creating a granularity mismatch.

The Solution: I engineered a common granularity level in the data model, allowing for seamless Variance % calculations that help management pinpoint exactly which months fell short of financial targets.

# 🏁 Final Conclusion
The resulting dashboard empowers the leadership team to move from reactive accounting to proactive financial management. By visualizing the relationship between revenue, profit, and cash, the organization can now make data-backed decisions regarding regional investments and cost-containment strategies.
