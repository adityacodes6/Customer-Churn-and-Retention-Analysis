# Customer Churn & Retention Analysis

## Project Overview
This project uses Python to analyze customer churn in a telecommunications dataset. It explores churn rates by contract type, customer tenure, monthly charges, and technical support to identify patterns that may help a business improve customer retention.

## Key Results

| Metric | Result |
|---|---:|
| Total customers | 7,043 |
| Customers who churned | 1,869 |
| Customers retained | 5,174 |
| Overall churn rate | **26.54%** |

### Key Business Insights

1. **Contract type:** Month-to-month customers had the highest churn rate at **42.71%**, compared with **11.27%** for one-year contracts and **2.83%** for two-year contracts.
2. **Customer tenure:** Customers with **0–12 months** of tenure had the highest churn rate at **47.44%**. The rate decreased to **28.71%** for 13–24 months, **20.39%** for 25–48 months, and **9.51%** for 49–72 months.
3. **Monthly charges:** Customers who churned had a median monthly charge of **79.65**, compared with **64.43** for retained customers. Their mean monthly charge was **74.44**, compared with **61.27** for retained customers. *(Currency units are not specified in this analysis.)*
4. **Technical support:** Customers without technical support had a churn rate of **41.64%**, while customers with technical support had a churn rate of **15.17%**.
5. **Retention opportunity:** The results suggest that early-tenure customers and month-to-month customers are useful groups for further retention analysis. The relationship between technical support and churn is also worth investigating.

## Project Objectives
- Calculate the overall customer churn rate.
- Compare churn rates across contract types.
- Identify the tenure group with the highest churn rate.
- Compare monthly charges for churned and retained customers.
- Examine the relationship between technical support and churn.
- Summarize the findings in a business-friendly format.

## Tools & Libraries
- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn

## Dataset
The notebook expects the Telco Customer Churn dataset in a CSV file named:

`WA_Fn-UseC_-Telco-Customer-Churn.csv`

Place the CSV file in the same folder as the notebook. The dataset contains customer demographics, subscribed services, billing details, tenure, contract type, and the `Churn` label.

## Analysis Performed
1. **Overall churn:** Counts churned and retained customers and calculates the overall percentage.
2. **Churn by contract:** Calculates and visualizes churn rates for month-to-month, one-year, and two-year contracts.
3. **Churn by tenure:** Groups tenure into 0–12, 13–24, 25–48, and 49–72 months and compares churn rates.
4. **Monthly charges:** Compares mean and median monthly charges by churn status and visualizes their distributions.
5. **Technical support:** Compares churn rates for customers with and without technical support.
6. **Key findings:** Prints a concise summary of the calculated results.

## How to Run
1. Download the dataset and save it as `WA_Fn-UseC_-Telco-Customer-Churn.csv`.
2. Keep the CSV file in the same directory as `customer_churn_and_retention_analysis.ipynb`.
3. Install the required libraries if they are not already installed:

   ```bash
   pip install pandas matplotlib seaborn jupyter
   ```

4. Open the notebook in Jupyter Notebook or JupyterLab.
5. Run all cells from top to bottom.

## Data Preparation
The notebook converts `TotalCharges` to a numeric column. Blank or invalid entries are converted to missing values and then filled with `0`.

## Business Questions
- What percentage of customers churned?
- Which contract type has the highest churn rate?
- How does churn vary with customer tenure?
- Do monthly charges differ between churned and retained customers?
- How does churn differ for customers with and without technical support?

## Conclusion
In this dataset, **26.54% of customers churned**. Churn was highest among month-to-month customers (**42.71%**) and customers with 0–12 months of tenure (**47.44%**). Customers without technical support also had a higher churn rate (**41.64%**) than those with support (**15.17%**). These patterns can help prioritize further retention analysis, but they show associations and do not prove that any one factor causes churn.

## Repository Structure
```text
customer-churn-retention-analysis/
├── customer_churn_and_retention_analysis.ipynb
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
└── README.md
```

## Author
**Aditya Mungekar**

Beginner-friendly data analytics portfolio project focused on exploratory data analysis and business insights.
