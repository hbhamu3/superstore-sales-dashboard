# Superstore Sales & Profitability Dashboard

## The Question
Which parts of the business are actually profitable, and where is revenue being generated without real profit to show for it?

## Data
The Sample Superstore dataset — ~9,994 retail transactions with sales, profit, discount, category, and sub-category data across a multi-year period.

## Approach
- Connected and cleaned the dataset in Tableau
- Built KPI summary cards, a monthly sales trend, and a sub-category-level breakdown of sales, profit, and discount
- Created a Profit Margin % calculated field to isolate margin performance independent of raw discount or sales volume
- Used color encoding and tooltips to compare discount rates against profitability across sub-categories

## Key Findings
- Overall the business generates strong revenue (**$2,297,200.86** in total sales) and healthy profit (**$286,397.02**), with an average order value of **$458.60**.
- **Four sub-categories are unprofitable or barely breaking even: Bookcases, Tables, Supplies, and Fasteners** — but the causes differ:
  - **Bookcases and Tables** carry high average discounts (**21%** and **26%** respectively), directly eroding margin.
  - **Fasteners and Supplies** show much lower average discounts (**7-8%**), meaning their weak profitability points to a structural pricing or cost issue rather than discounting.
- This distinction matters: a single blanket fix (e.g. "cut all discounts") would not solve the full picture, since two different problems are driving the same symptom.

## Recommendation
Apply a tighter discount cap specifically on Bookcases and Tables, where discounting is the clear driver of poor margin. Separately, investigate cost and pricing structure for Fasteners and Supplies, since low discounting rules out discount policy as the cause there — the fix needs to be different.

## Dashboard
🔗 **[View the live interactive dashboard on Tableau Public](https://public.tableau.com/app/profile/harish.bhamu/viz/Book1_17897589447190/Dashboard1?publish=yes
))**

![Dashboard Overview](images/dashboard_overview.png)

## Tools
Tableau (Tableau Public), calculated fields (DAX-equivalent), data cleaning and modeling

## Files
- `dashboard_overview.png` — screenshot of the full dashboard
- Live version available via the Tableau Public link above (interactive, filterable)
