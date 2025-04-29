![GitHub Banners (2)](https://github.com/user-attachments/assets/f0d821a2-3dc2-4a62-b670-bc5ba7c968c7)

# Customer-Sales-Data-Cohort-Analysis
This project performs a Cohort Analysis on an online retail dataset to analyse customer purchasing behaviour over time, with a focus on retention and monthly sales trends.

---

## Business Insights

### 1. Identify the highest customer retention from the observation
Customers onboarded in the December 2010 cohort show relatively strong retention over 12 months, with 50% returning customers.
- This signifies that these customers have repeated purchase intent during the Christmas/Year-End sales trend to buy from the online store.
- Hence, the brand should focus on what was different that month with respect to ads run, promos, or discounts given.
  
  ![image](https://github.com/user-attachments/assets/c0ccc056-bb91-45e5-84cb-8e97943e89b1)

### 2. Identify the lowest customer retention rate from the observation
Customers onboarded in March 2011 show the highest drop-off, from 100% to 19.09% (approx. 60–75%).
- This might be because the purchases made during the financial year-end were from one-time buyers.
- Also, we observe a stabilized retention of customers acquired from Mar 2011, on the 6th Month at 17.73% increasing to 26.36% in the next Month.
- This suggests possible return behavior or successful re-engagement campaigns.
### 3. Visualize monthly revenue growth or decline from the Monthly Sales chart
- The business has seen a steady growth from Aug 2011 up to Nov 2011 (+114%) and shows a sudden dip in the Sales presumably due to insufficient data.
  ![image](https://github.com/user-attachments/assets/7bf9b0c3-e994-41c3-aa06-c7ba505dfb83)
### 4. Provide business decisions related to marketing and customer retention strategies
- The business should focus on retaining more users after the first month by offering membership programs, promotional follow-ups, or cashback on each purchase.

---

## Dataset

The dataset includes transactional data such as invoice date, customer ID, quantity, and unit price. This dataset contains all purchases made for an online retail company based in the UK during eight months, collected from [Kaggle](https://www.kaggle.com/datasets/vijayuv/onlineretail).

---

## Tools & Technologies

- **Python**: pandas, numpy, matplotlib, seaborn, plotly
- **Google Colab**: notebook development and execution
- **Plotly**: interactive data visualization
- **Seaborn**: statistical data visualization

---

## Workflow Summary

### 1. Data Loading and Preprocessing
- Load the dataset using `pandas`
- Create a `Sales` column as the product of `Quantity` and `UnitPrice`
- Extract the first day of the billing month (`BillMonth`) from the `InvoiceDate`

### 2. Monthly Sales Trend
- Aggregate monthly sales
- Create an interactive line chart showing monthly sales using Plotly

### 3. Cohort Analysis
- Define `CohortMonth` for each customer based on their first purchase
- Calculate `MonthIndex` to track each customer’s behavior over time
- Compute `retention` by counting unique customers in each cohort and month

### 4. Visualization
- Plot an Interactive line chart of monthly sales
- Plot a retention heatmap using Seaborn, showing the percentage of retained customers for each cohort over time
