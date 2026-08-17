# E-commerce Sales & Customer Analysis

**Portfolio Project | Python • SQL • BigQuery • Tableau**

## Business objective

Analyze e-commerce sessions and sales to identify the main revenue drivers, customer behavior patterns, traffic-channel performance, seasonality, and statistically significant relationships that can support business decisions.

## Dataset

- **Period:** 1 November 2020 – 31 January 2021
- **Rows:** 349,545
- **Columns:** 19
- **Main dimensions:** geography, device, browser, operating system, traffic source/channel, customer status and product category
- **Main metric:** product price / sales value

The original analytical dataset was built from a BigQuery training project. The source project is no longer accessible from the current account, so the GitHub version is designed around the saved cleaned dataset rather than requiring the original BigQuery permissions.

## Analysis

### 1. Data preparation
- date conversion;
- missing-value treatment;
- handling of unknown values;
- duplicate checks;
- validation of negative prices;
- dataset profiling.

### 2. Sales and customer analysis
- revenue by continent and country;
- top product categories;
- sales by device;
- traffic channel / medium / source performance;
- email confirmation rate;
- unsubscribe rate;
- customer behavior by subscription status.

### 3. Sales dynamics
- daily sales;
- 7-day rolling trend;
- seasonality;
- sales dynamics by continent;
- sales dynamics by traffic channel;
- sales dynamics by device.

### 4. Statistical analysis
The project includes:
- Pearson correlation;
- correlation matrices;
- ANOVA;
- Mann–Whitney U test;
- Kruskal–Wallis test;
- chi-square test;
- two-proportion z-test.

## Key findings

- **Americas** is the leading region by sales.
- **United States** is the leading country by revenue.
- **Nest** is the largest revenue-generating product category.
- **Desktop** accounts for the largest share of revenue.
- **Direct** and **Organic Search** are the dominant traffic channels.
- Sales show clear **weekly and holiday seasonality**, with a strong increase around the end of November / beginning of December.
- Daily sessions and sales show a strong positive relationship: **Pearson r = 0.791, p = 6.4835e-21**.
- Organic traffic shares in Europe and Americas are statistically similar: **p = 0.7722**.
- Device type and registration status do not show a statistically significant relationship: **p = 0.2318**.
- The project also identifies statistically significant differences in daily sales between registered and unregistered groups and significant differences in daily sessions across traffic channels.

## Business recommendations

1. Continue investing in SEO because Organic Search is one of the main revenue and traffic drivers.
2. Prioritize reliability and performance of the desktop experience because desktop generates the majority of revenue in this dataset.
3. Align promotional activity with the observed seasonal demand pattern.
4. Monitor the Americas market closely because it has the largest impact on total revenue.
5. Investigate conversion and acquisition cost by traffic channel before increasing paid-search investment.
6. Use customer-status analysis to design more relevant retention and communication strategies.

## Tools

**Python:** pandas, NumPy, SciPy, statsmodels, Matplotlib, Seaborn  
**SQL:** Google BigQuery  
**BI:** Tableau Public

## Portfolio links

### Interactive Tableau dashboard
https://public.tableau.com/app/profile/mariia.mykolenko/viz/SalesOverviewCustomerAnalysisPortfolioProgect/Story1?publish=yes

### Notebook
The notebook is available in this repository and can be opened in Google Colab for code review.

## Repository structure

```text
ecommerce-sales-customer-analysis/
│
├── README.md
├── Ecommerce_Sales_Customer_Analysis_Portfolio.ipynb
├── cleaned_project_data.csv
└── images/
    ├── dashboard.png
    └── analysis_preview.png
```

> **Important:** `cleaned_project_data.csv` should be added only if you have the saved cleaned dataset from your original Colab session. The uploaded notebook contains the analysis code and written results, but it does not contain the full underlying dataset itself.
