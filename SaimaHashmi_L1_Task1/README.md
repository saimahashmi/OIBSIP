# L1 Task 1: EDA on Retail Sales Data

**Intern:** Saima Hashmi | **Program:** Oasis Infobyte Internship (OIBSIP) | **Track:** Data Analytics

## Objective
Exploratory Data Analysis on a retail sales dataset to find sales trends, customer demographics patterns and business insights.

## Dataset
Retail Sales Dataset from Kaggle (1,000 transactions, 9 columns, 1 Jan 2023 to 1 Jan 2024).
Columns: Transaction ID, Date, Customer ID, Gender, Age, Product Category, Quantity, Price per Unit, Total Amount.

## Tech Stack
Python, pandas, numpy, matplotlib, seaborn, Jupyter Notebook (Google Colab)

## Checklist
- [x] Dataset loading and inspection (shape, dtypes, null check)
- [x] Descriptive statistics (mean, median, mode, std)
- [x] Monthly and quarterly sales trends
- [x] Customer demographics (age groups, gender)
- [x] Product category analysis (revenue, units, transactions)
- [x] Correlation heatmap
- [x] Additional visualisation (age group vs product category)
- [x] Observations after each chart
- [x] Conclusion with business recommendations

## Key Findings
- No null values or duplicates; the dataset is clean.
- Sales peaked in May (53,150) and were lowest in September (23,620); Q4 was the strongest quarter.
- Customers are balanced by gender (51% female, 49% male); the 18-24 group is the smallest.
- Electronics (34.4%) and Clothing (34.1%) earn almost equal revenue; Beauty is lowest (31.5%).
- Price per Unit is strongly correlated with Total Amount (0.85); age shows almost no linear correlation with spending.
- Different age groups prefer different categories (e.g. Clothing peaks at 25-34, Electronics at 55-64).

## Limitations
- The dataset has no product names, so categories were ranked instead of a "top 10 products" list.
- It covers only one year, so seasonality cannot be confirmed.

## Files
- `SaimaHashmi_L1_Task1.ipynb`: the analysis notebook
- `retail_sales_dataset.csv`: the dataset
