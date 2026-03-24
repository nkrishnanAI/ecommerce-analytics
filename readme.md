# 🛒 E-Commerce Customer Analytics Project

## 📌 Overview

This project performs an end-to-end analysis of an e-commerce dataset to extract meaningful insights about customer behavior, revenue patterns, and business performance. It includes data cleaning, exploratory data analysis (EDA), and customer segmentation using RFM methodology.

The project is designed to simulate a real-world business scenario where data is leveraged to improve **customer retention, revenue optimization, and decision-making**.

---

## 📂 Dataset

* Source: Online Retail dataset (transaction-level data)
* Key fields:

  * Invoice
  * StockCode
  * Description
  * Quantity
  * InvoiceDate
  * UnitPrice
  * CustomerID
  * Country

---

## ⚙️ Data Preprocessing

### Steps performed:

* Converted `InvoiceDate` to datetime format
* Standardized column names (removed spaces)
* Renamed `Price` → `UnitPrice`
* Removed missing `CustomerID` values
* Filtered cancelled transactions (Invoice starting with "C")
* Removed invalid records (negative quantity or price)
* Created new feature:

  * `TotalPrice = Quantity × UnitPrice`

---

## 📊 Exploratory Data Analysis (EDA)

### Key analyses performed:

* Revenue trend over time (monthly aggregation)
* Transaction value distribution (identified heavy skewness and outliers)
* Top-selling products (by quantity and revenue)
* Country-wise revenue distribution
* Time-based analysis (day/month trends)

### Key findings:

* Revenue distribution is highly right-skewed
* A small number of transactions contribute disproportionately high revenue
* Certain products dominate sales volume
* Revenue is concentrated in specific geographic regions

---

## 🧠 RFM Customer Segmentation

### Metrics:

* **Recency** → Days since last purchase
* **Frequency** → Number of transactions
* **Monetary** → Total customer spend

### Method:

* Customers scored using quantiles (1–5 scale)
* Segmented into behavioral groups

### Segments identified:

* Champions
* Loyal Customers
* New Customers
* At Risk
* Lost Customers

---

## 📈 Business Insights

* A small percentage of customers contribute a large portion of total revenue
* High-value customers (Champions) are critical for revenue stability
* At-risk customers present an opportunity for retention strategies
* Transaction values show significant variance, indicating mixed customer types (retail vs bulk buyers)

---

## 💡 Recommendations

* Implement loyalty programs for high-value customers
* Target at-risk customers with personalized offers
* Improve onboarding for new customers to increase retention
* Focus marketing efforts on high-performing products and regions

---

## 🛠️ Tools & Technologies

* Python (Pandas, NumPy)
* Data Visualization (Matplotlib, Seaborn)
* Jupyter Notebook

---

## 📁 Project Structure

```id="n3k8cf"
ecommerce-analytics/
│
├── data/
├── notebooks/
├── models/
├── dashboard/
├── README.md
```

---

## 🚀 Future Enhancements

* Customer churn prediction model
* Customer Lifetime Value (CLV) modeling
* Interactive dashboard (Power BI / Tableau)
* Real-time data pipeline integration

---

## 🧠 Key Learnings

* Real-world datasets require extensive cleaning
* Outliers significantly impact analysis and visualization
* Customer segmentation is essential for business strategy
* Data analysis must translate into actionable insights

---

## 📎 How to Run

1. Install dependencies:

   ```
   pip install pandas numpy matplotlib seaborn
   ```
2. Run the notebook:

   ```
   jupyter notebook
   ```
3. Execute cells step-by-step

---

