# 🛒 Retail Store Trial Analysis — Data Analytics Project

## 📌 Overview
This project evaluates the impact of a retail store trial conducted in **Store 77**, **Store 86**, and **Store 88** using real retail transaction data.  
The goal is to determine whether the trial significantly improved performance compared to similar non-trial (control) stores.

This analysis is completed using Python in Jupyter Notebooks and follows a structured, professional workflow used in real analytics teams.

---

## 📂 Project Structure

📦 QVI_Store_Trial_Analysis
│
├── data/
│ ├── QVI_data.csv
│ ├── QVI_monthly_aggregated.csv
│ ├── controlstore_correlation_scores_top5.csv
│ ├── controlstore_magnitude_scores_top5.csv
│
├── notebooks/
│ ├── Notebook_1_Data_Preparation.ipynb
│ ├── Notebook_2_Control_Store_Selection.ipynb
│ ├── Notebook_3_Trial_vs_Control_Evaluation.ipynb
│ ├── Notebook_4_Visualizations_and_Insights.ipynb
│ ├── Notebook_5_Final_Report.ipynb
│
├── README.md
└── requirements.txt


---

## 🎯 Project Objectives

- Prepare and clean raw retail transaction data  
- Aggregate store performance at monthly granularity  
- Identify the most similar "control stores" for each trial store  
- Compare trial vs control during the trial period  
- Conduct significance testing to measure trial impact  
- Visualize differences in sales, customers, and transaction patterns  
- Deliver a final data-driven conclusion on trial effectiveness  

---

## 🧪 Analysis Workflow

### **📘 Notebook 1: Data Preparation**
- Loaded raw QVI dataset  
- Cleaned records, removed duplicates, handled missing values  
- Created key features such as `SPEND` and `YearMonth`  
- Aggregated store-level monthly metrics:
  - Total Sales  
  - Total Customers  
  - Average Transactions per Customer  

---

### **📘 Notebook 2: Control Store Selection**
- Computed Pearson correlations to measure trend similarity  
- Calculated magnitude distance to measure metric closeness  
- Ranked candidate control stores for Stores 77, 86, and 88  
- Selected the optimal control store for each trial store  

---

### **📘 Notebook 3 (Upcoming): Trial vs Control Evaluation**
- Defined trial period  
- Compared trial and control store performance across KPIs  
- Conducted t-tests for statistical significance  
- Visualized differences using time-series plots  

---

### **📘 Notebook 4 (Upcoming): Visualizations & Insights**
- Diagnose pre-trial similarity  
- Deep visual analysis: sales, customers, transactions  
- Visual dashboards and charts  

---

### **📘 Notebook 5 (Upcoming): Final Report & PDF Export**
- Executive summary  
- Detailed findings for each trial store  
- Statistical conclusions  
- PDF-ready documentation  

---

## 📊 Key Metrics Explained

- **Total Sales:** Total spending per month  
- **Total Customers:** Number of unique customers  
- **Average Transactions per Customer:** Frequency of purchasing behavior  

---

## 🛠 Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- SciPy  
- Jupyter Notebook  

---

## 📈 Outcome
This project provides a structured, professional approach to measuring trial effectiveness—identifying whether a retail store initiative led to:

- Increased sales  
- Higher customer traffic  
- Changes in purchasing frequency  
- Statistically significant improvements  

---

## 👩🏽‍💻 Author
**Joshua Ikem**  
Data Analyst | Python, Excel & SQL | Retail & Business Analytics  
([https://www.linkedin.com/in/joshua-ikem-998523375/])

---

