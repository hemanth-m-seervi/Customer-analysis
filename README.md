# Telecom Customer Churn Exploratory Data Analysis (EDA)

## 📊 Project Overview
This data analyst project focuses on identifying the driving factors behind customer attrition (churn) in a telecommunications company. By performing an Exploratory Data Analysis (EDA) using Python, this project uncovers critical behavioral patterns and service pain points that lead to customer turnover, providing data-backed recommendations to improve customer retention.

The analysis evaluates a dataset containing **7,043 customer records** with 21 attributes detailing demographic profiles, active services, contract lengths, billing methods, and historical financial metrics[cite: 2].

---

## 🛠️ Tech Stack & Skills Demonstrated
*   **Environment:** Jupyter Notebook (`.ipynb`)[cite: 2]
*   **Data Manipulation:** Python (Pandas, NumPy)[cite: 2]
*   **Data Visualization:** Matplotlib, Seaborn[cite: 2]
*   **Data Cleaning:** Handling missing strings, converting data types, and remapping categorical indicators[cite: 2]

---

## 💾 Dataset Summary
The underlying analysis references the foundational dataset: **"Customer Churn.csv"**[cite: 2].

### **Key Metrics & Base Findings:**
*   **Total Operations Analyzed:** 7,043 unique customer accounts[cite: 2].
*   **Overall Churn Rate:** **26.54%** of the customer base has churned (1,869 customers moved out, while 5,174 stayed)[cite: 2].
*   **Financial & Account Profile:**
    *   **Average Tenure:** ~32.37 months[cite: 2].
    *   **Average Monthly Charges:** \$64.76[cite: 2].
    *   **Max Monthly Charges:** \$118.75[cite: 2].

### **Data Processing & Feature Transformation:**
1.  **Missing Financial Values Fixed:** Empty string records (`" "`) within the `TotalCharges` column (corresponding to new customers with a tenure of `0` months) were replaced with `"0"` and cast to an accurate `float` data type[cite: 2].
2.  **Categorical Enhancement:** Numerical flags (`0` / `1`) for `SeniorCitizen` were transformed into readable categorical strings (`no` / `yes`) to make chart keys instantly interpretable[cite: 2].

---

## 📈 Executive Insights & Visual Discoveries

### **1. Demographics & Age Vulnerabilities**
*   **Gender Neutrality:** Gender plays no role in customer retention[cite: 2]. Churn is distributed almost evenly between male and female cohorts[cite: 2].
*   **Senior Citizen Turnover:** Senior Citizens represent a high-risk group[cite: 2]. While the churn rate for non-seniors sits around 23.61%, it spikes drastically to **41.68%** for Senior Citizens[cite: 2].

### **2. Subscription Lengths & Financial Contracts**
*   **The 1-Month Critical Window:** Customer tenure exhibits an inverse U-shape curve[cite: 2]. A significant cluster of churn happens in the very first or second month of subscription, while customer loyalty sharply solidifies the longer a user stays[cite: 2].
*   **Contract Types:** Customers on a **Month-to-month contract** have a massive **42.71% churn rate**[cite: 2]. This is compared to a low 11.27% churn rate for One-year agreements and a nominal 2.83% for Two-year locked-in plans[cite: 2].

### **3. Operational Services & Product Ecosystems**
*   **High-Value Retention Anchors:** Customers who utilize add-on features—specifically **Online Security, Online Backup, and Tech Support**—show noticeably lower churn volumes[cite: 2]. 
*   **Friction Points:** Attrition drops off significantly when customers use more robust technical ecosystems; non-users or unlinked accounts carry the highest proportional churn[cite: 2].

### **4. Payment Ecosystem Flaws**
*   **Electronic Check Warning:** Payment friction is an obvious driver[cite: 2]. Customers paying via **Electronic Check** represent the highest attrition cohort, accounting for **1,071 churned accounts** (a churn rate approaching 45% within that payment method alone)[cite: 2].
*   **Automatic Peace of Mind:** Customers using automated options (Bank Transfer or Credit Card) exhibit the highest relative stability and retention[cite: 2].

---

## 🚀 How to Run the Analysis

1.  **Prerequisites:** Clone or download the repository ensuring Python, `pandas`, `numpy`, `matplotlib`, and `seaborn` are installed[cite: 2].
2.  **File Placement:** Keep the verbatim data file `"Customer Churn.csv"` in the same working directory as your downloaded copy of the notebook[cite: 2].
3.  **Execution:** Run the blocks sequentially inside a standard Jupyter environment to regenerate all step-by-step transformations, analytical aggregates, and visual graphs[cite: 2].
