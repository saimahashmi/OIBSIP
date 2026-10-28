# L1 Task 2: Customer Segmentation using RFM Analysis and K-Means

**Intern:** Saima Hashmi | **Program:** Oasis Infobyte Internship (OIBSIP) | **Track:** Data Analytics

## Objective
To segment an online retailer's customers by purchasing behaviour (Recency, Frequency, Monetary) using K-Means clustering, and to suggest a marketing action for each segment.

## Dataset
- **Source:** [Online Retail II, UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii) (donated by Daqing Chen)
- **License:** CC BY 4.0
- **Content:** real transactions of a UK-based online retailer from 1 Dec 2009 to 9 Dec 2011, 1,067,371 rows and 8 columns across two yearly sheets (Invoice, StockCode, Description, Quantity, InvoiceDate, Price, Customer ID, Country)
- The dataset file (about 45 MB) is not included in this repository. To rerun the notebook, download it from the link above and place `online_retail_II.xlsx` next to the notebook.

## Tech Stack
Python, pandas, numpy, scikit-learn (KMeans, StandardScaler, silhouette score), matplotlib, seaborn, Jupyter Notebook (Google Colab)

## What I Did
- [x] Loaded and combined both sheets, then inspected structure, missing values and duplicates
- [x] Cleaned the data (duplicates, missing Customer ID, cancelled invoices, invalid price/quantity, non-product codes) and documented rows removed at each step
- [x] Calculated descriptive statistics: average purchase value, purchase frequency and historical customer value
- [x] Built RFM features (Recency, Frequency, Monetary) per customer
- [x] Applied a log transform and StandardScaler before clustering
- [x] Chose K using the Elbow Method and silhouette score (K = 4)
- [x] Visualised clusters with scatter plots (3 feature combinations) and a bar chart of customers per cluster
- [x] Profiled each cluster and gave marketing recommendations per segment

## Key Findings
- After cleaning, 776,577 rows and 5,852 customers remained (from 1,067,371 rows).
- Segments found (K = 4):
  - **Champions:** 20.2% of customers, 73.3% of revenue (recent, frequent, highest spend)
  - **Recent / Promising:** 21.3% of customers, 6.1% of revenue (recent but few purchases so far)
  - **At Risk:** 24.9% of customers, 16.9% of revenue (decent past spend, inactive for months)
  - **Lost / Inactive:** 33.6% of customers, 3.7% of revenue (bought about once, not seen for over a year)
- Revenue is highly concentrated in a small group of customers.

## Limitations
- There was no sharp elbow, so K = 4 is a reasonable choice (silhouette about 0.37), not the only correct answer.
- Only RFM features were used; product type, country and order size were not.
- The data covers one UK-based retailer (many wholesale customers), so the results may not apply to other businesses.
- Monetary value is historical spending, not a prediction of future value.

## Files
- `SaimaHashmi_L1_Task2.ipynb`: the analysis notebook
