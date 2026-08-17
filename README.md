[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mariia-m-analytics/ecommerce-sales-customer-analysis/blob/main/Ecommerce_Sales_Customer_Analysis_Portfolio%281%29.ipynb)
# E-commerce Sales & Customer Analysis

**Portfolio Project | Python • SQL • BigQuery • Tableau**

## Business objective
Analyze e-commerce sessions and sales to identify the main revenue drivers, customer behavior patterns, traffic-channel performance, seasonality, and statistically significant relationships that can support business decisions.

## Dataset
- **Rows:** 349,545
- **Columns:** 21
- **Period:** 1 November 2020 – 31 January 2021
- **Key dimensions:** geography, device, browser, operating system, traffic source/channel, customer status and product category
- **Main metric:** `price`

The original analytical dataset was created in a BigQuery training project. The portfolio version uses the final cleaned CSV stored in `data/`, so the notebook can be reviewed without access to that training project.

## Analysis
1. Data preparation and quality checks
2. Sales and customer analysis
3. Sales dynamics and seasonality
4. Correlation analysis
5. Statistical tests:
   - Pearson correlation
   - ANOVA
   - Mann–Whitney U
   - Kruskal–Wallis
   - Chi-square
   - two-proportion z-test
6. Business conclusions and recommendations

## Key findings
- Americas is the leading region by sales.
- United States is the leading country by revenue.
- Nest is the largest revenue-generating category in the completed analysis.
- Desktop generates the largest share of revenue.
- Direct and Organic Search are the dominant traffic channels.
- Sales show weekly and holiday seasonality.
- Daily sessions and sales show a strong positive relationship (Pearson r = 0.791 in the completed analysis).
- Organic traffic shares in Europe and Americas were statistically similar (p = 0.7722).
- Device type and registration status were not statistically significantly associated (p = 0.2318).

## Business recommendations
1. Continue investing in SEO.
2. Prioritize the desktop user experience while improving mobile conversion.
3. Align promotions with seasonal demand.
4. Monitor the Americas market closely.
5. Compare traffic-channel revenue with acquisition cost before increasing paid acquisition.
6. Use registered-customer behavior for retention and lifecycle strategies.

## Tools
**Python:** pandas, NumPy, SciPy, statsmodels, Matplotlib, Seaborn  
**SQL:** Google BigQuery  
**BI:** Tableau Public

## Project links
**Tableau Public:**  
https://public.tableau.com/app/profile/mariia.mykolenko/viz/SalesOverviewCustomerAnalysisPortfolioProgect/Story1?publish=yes

## Repository structure
```text
ecommerce-sales-customer-analysis/
├── README.md
├── Ecommerce_Sales_Customer_Analysis_Portfolio.ipynb
├── requirements.txt
└── data/
    └── cleaned_project_data.csv
```
