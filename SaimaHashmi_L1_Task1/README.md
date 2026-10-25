# L1 Task 1: Exploratory Data Analysis on Retail Sales Data

**Intern:** Saima Hashmi | **Program:** Oasis Infobyte Internship (OIBSIP) | **Track:** Data Analytics

## Objective
To explore a retail sales dataset and uncover sales trends, customer demographic patterns and category performance, and to turn the findings into business recommendations.

## Dataset
- **Source:** [Retail Sales Dataset on Kaggle](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset) (created by mohammadtalib786)
- **Size:** 1,000 transactions, 9 columns, covering 1 Jan 2023 to 1 Jan 2024
- **Columns:** Transaction ID, Date, Customer ID, Gender, Age, Product Category, Quantity, Price per Unit, Total Amount
- **Note:** This is a synthetic (fictional) dataset made for practice, so the findings show the analysis process and should not be read as real-world business results.

## Tech Stack
Python, pandas, numpy, matplotlib, seaborn, Jupyter Notebook (Google Colab)

## What I Did
- [x] Loaded the data and inspected shape, data types and null values
- [x] Calculated descriptive statistics (mean, median, mode, standard deviation)
- [x] Plotted monthly and quarterly sales trends
- [x] Analysed customer age groups and gender
- [x] Compared product categories by revenue, units sold and transactions
- [x] Built a correlation heatmap of the numerical variables
- [x] Added an extra visualisation: age group vs product category
- [x] Wrote observations after each chart
- [x] Finished with a conclusion and business recommendations

## Key Findings
- The data is clean: no null values and no duplicate rows.
- Monthly sales were uneven. May was the highest month (53,150) and September the lowest (23,620). Q4 was the strongest quarter and Q3 the weakest.
- Customers are split almost equally by gender (51% female, 49% male). The 18-24 group is the smallest age group.
- Electronics (34.4%) and Clothing (34.1%) earn almost the same revenue, with Beauty slightly lower (31.5%).
- Price per Unit is strongly correlated with Total Amount (0.85), while age shows almost no linear correlation with spending.
- Age groups prefer different categories: Clothing is highest among 25-34 year olds and Electronics among 55-64 year olds.

## Limitations
- The dataset is synthetic, so patterns such as seasonality and category preferences may not match a real retail business.
- It has no product names, so categories were ranked instead of making a "top 10 products" list.
- It covers only one year, so seasonality cannot be confirmed.
- Some age group and category cells contain few transactions, so those differences may be due to chance.

## Files
- `SaimaHashmi_L1_Task1.ipynb`: the analysis notebook
- `retail_sales_dataset.csv`: the dataset
