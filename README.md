
# Superstore Business Analytics

## Project Overview

An end-to-end retail business analytics project designed to evaluate sales performance, profitability, customer behavior, discount strategies, and operational efficiency.

This project combines Python, SQL, statistical analysis, DAX, and Power BI to transform retail transaction data into actionable business insights.

## Business Objectives

- Evaluate overall sales and profitability.
- Identify revenue trends and growth opportunities.
- Identify profitable and underperforming product categories.
- Analyze regional and customer segment performance.
- Investigate the relationship between discounts and profitability.
- Evaluate shipping performance.
- Develop an interactive business intelligence dashboard.

## Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Data cleaning and analysis |
| Pandas and NumPy | Data manipulation |
| Matplotlib and Seaborn | Data visualization |
| SciPy | Statistical hypothesis testing |
| Statsmodels | Regression analysis |
| SQL (SQLite) | Business data analysis |
| Power BI | Interactive dashboards |
| DAX | Business performance measures |
| Google Colab | Development environment |

## Dataset

The Superstore dataset contains 9,994 transaction-level records covering the period from 2014 to 2017.

- Original columns: 21
- Processed columns: 27
- Unique orders: 5,009
- Unique customers: 793

Source: [Superstore Dataset - Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

Original data credited to Tableau and its respective creators. This project was developed for educational and portfolio purposes. Redistribution permissions have not been independently verified.

## Data Cleaning and Preprocessing

- Checked missing values and duplicate records.
- Validated transaction values and shipping dates.
- Converted date columns into datetime format.
- Created additional analytical features:
  - Year
  - Month
  - Month Name
  - Quarter
  - Profit Margin
  - Shipping Days

## Key Performance Indicators

| Metric | Result |
|---|---:|
| Total Revenue | $2,297,200.86 |
| Total Profit | $286,397.02 |
| Overall Profit Margin | 12.47% |
| Total Orders | 5,009 |
| Unique Customers | 793 |
| Total Units Sold | 37,873 |
| Average Order Value | $458.61 |
| Revenue per Customer | $2,896.85 |

## Exploratory Data Analysis

The exploratory analysis examined:

- Annual and monthly revenue trends
- Product category performance
- Sub-category profitability
- Regional sales and profitability
- Customer segmentation
- Discount distribution
- Shipping performance

### Annual Revenue Performance

| Year | Revenue | Annual Growth |
|---|---:|---:|
| 2014 | $484,247.50 | N/A |
| 2015 | $470,532.51 | -2.83% |
| 2016 | $609,205.60 | 29.47% |
| 2017 | $733,215.26 | 20.36% |

## Statistical Analysis

### Correlation Analysis

The Pearson correlation coefficient between discount and transaction-level profit margin was approximately -0.8645, indicating a strong negative relationship.

### Hypothesis Testing

An independent-samples comparison was conducted to evaluate differences in profit margins between lower-discount and higher-discount transactions.

- Lower-discount mean profit margin: 26.69%
- Higher-discount mean profit margin: -78.45%
- Test statistic: 59.61

The results indicate a statistically significant difference between the two groups.

### Regression Analysis

An ordinary least squares regression model with cluster-robust standard errors was used to investigate the relationship between discounts and profitability.

- R-squared: 0.756
- Strong negative association between discounts and profit margins

The model explains approximately 75.6% of the observed variation in profit margin.

These findings represent statistical associations rather than proof of causation. Residual diagnostics also indicated limitations related to heteroskedasticity and non-normality.

## SQL Business Analysis

SQL queries were developed to analyze:

- Overall business performance
- Category and sub-category profitability
- Annual revenue growth
- Regional performance
- Top-performing customers
- Discount-based profitability
- Regional product performance

## Power BI Dashboard

The interactive dashboard contains two report pages, six KPI cards, ten analytical charts, and four synchronized slicers.

### Executive Overview

![Executive Overview](images/Executive_Overview.png)

### Detailed Analysis

![Detailed Analysis](images/Detailed_Analysis.png)

### Interactive Features

- Year filter
- Region filter
- Category filter
- Segment filter
- Cross-page slicer synchronization
- Dynamic KPI calculations using DAX

## Key Business Findings

1. Technology generated the highest revenue and profit, with approximately $836,154 in revenue and $145,455 in profit.

2. Furniture recorded a profit margin of only 2.49%, despite generating approximately $742,000 in revenue.

3. Tables, Bookcases, and Supplies were loss-making sub-categories.

4. The West region achieved the highest regional profit margin at 14.94%.

5. The Central region recorded the lowest regional profit margin at 7.92%.

6. Revenue increased by 20.36% in 2017 compared with 2016.

7. Consumer customers contributed approximately 50.56% of total revenue.

8. Extreme-discount transactions recorded an average transaction-level profit margin of approximately -78.82%.

## Business Recommendations

- Review excessive discounting and introduce profitability-based discount limits.
- Prioritize high-performing Technology and Office Supplies products.
- Reevaluate pricing and costs for loss-making Furniture products.
- Investigate discounting and operational inefficiencies in the Central region.
- Develop customer retention strategies for high-value customers.
- Use historical revenue trends to support seasonal inventory planning.
- Evaluate shipping efficiency while balancing delivery speed and operational costs.

## Repository Structure

    superstore-business-analytics/
    ├── data/
    ├── notebooks/
    │   └── Superstore_Analysis.ipynb
    ├── dashboard/
    │   └── Superstore_Business_Analytics.pbix
    ├── images/
    │   ├── Executive_Overview.png
    │   └── Detailed_Analysis.png
    └── README.md

## How to Use This Project

1. Download or clone the repository.
2. Open the Jupyter notebook using Google Colab or Jupyter Notebook.
3. Update dataset paths if necessary.
4. Run the analytical notebook.
5. Open the PBIX file using Power BI Desktop.
6. Explore the dashboard using the interactive filters.

## Conclusion

This project demonstrates an end-to-end business analytics workflow, integrating data preprocessing, exploratory analysis, statistical modeling, SQL, and business intelligence.

The analysis translates retail transaction data into meaningful insights that can support profitability improvement, strategic planning, and data-driven business decisions.

## Author

Niloy Kanti Dhar

Statistics, Data Science and Mathematics

University of Lynchburg | Class of 2027
