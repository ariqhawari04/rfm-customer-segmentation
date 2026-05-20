# 👥 Customer Segmentation with RFM & K-Means

A quick and scalable data analytics workflow to segment an online retail dataset containing **25,000+ transaction logs**. By combining the **RFM (Recency, Frequency, Monetary)** framework with **K-Means Clustering**, this project simulates how commercial teams optimize user retention and marketing spend.

*Note: This repository serves as an analytics playbook inspired by real-world B2B and retail-centric use cases.*

---

### 💼 The Business Problem
Using a single marketing approach for all customers is inefficient. To maximize revenue growth and prevent user churn, cross-functional teams need to identify:
1. Who are our high-value **Champions**?
2. Which users are **At-Risk / Sleeping** and need a win-back campaign?
3. How can we target campaigns without wasting budget?

---

### 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn (K-Means), Matplotlib, Seaborn

---

### 🚀 Quick Steps to Execute
1. **Data Preprocessing (Pandas):** Load the `.csv` file, handle missing IDs, drop transaction anomalies (negative quantities/returns), and engineer a `TotalAmount` feature ($Quantity \times UnitPrice$).
2. **RFM Metrics:** Calculate Recency (days since last purchase), Frequency (total unique invoices), and Monetary (total spend) per customer using Pandas aggregations.
3. **Clustering (Scikit-Learn):** Scale data using `StandardScaler` and apply K-Means clustering to discover distinct user behaviors.

---

### 📊 Anticipated Insights
* **Champions:** Reward with exclusive loyalty perks.
* **High Spenders:** Cross-sell premium high-margin bundles.
* **At Risk / Sleeping:** Trigger re-engagement discount emails.