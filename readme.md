# Retail Store Trial Analysis — Data Analytics Project

## Overview
# README (UPDATED AND FINALIZED): Store Trial Performance Analysis Project

## Overview

This project evaluates the effectiveness of a retail trial conducted across three trial stores. The business objective was to determine whether the trial produced a measurable and statistically significant uplift in store performance. The analysis identifies which trial stores experienced meaningful improvement and which did not, based on a structured data-science workflow documented across six Jupyter Notebooks.

The project follows a clear analytical pipeline: data preparation, control store selection, performance comparison, statistical testing, impact interpretation, and executive reporting. All outputs are reproducible, structured, and suitable for production-level analytic workflows.

---

# 1. Project Purpose

Retail trials introduce new strategies, promotions, layouts, or operational changes in selected stores. However, trial results are only actionable if the measured changes can be attributed to the trial and not random variation.

  - The project aims to answer:
  - Did the trial significantly increase store sales?
  - Did customer volume or customer purchasing behavior change?
  - Are the results statistically reliable and repeatable?
  - What should leadership conclude from the trial?

To achieve this, each trial store was matched with a similar control store, allowing accurate comparison of performance before and during the trial period.

---

# 2. Data Sources

The analysis uses a QVI dataset containing transactional information. Key fields include:

* Transaction date and time
* Store ID
* Customer ID
* Product quantity and price
* Transaction value

From these, new aggregated monthly features were engineered:

* Monthly total sales
* Monthly total customers
* Monthly transactions per customer
* Monthly average transaction value
* A consolidated Year-Month field

These transformations created a dataset suited for store-level time-series evaluation.

---

# 3. Analytical Structure (Notebooks 1–6)

The project is divided into six notebooks, each focusing on a specific stage of the workflow.

---

## Notebook 1: Data Cleaning and Monthly Aggregation

This notebook loads the raw data, cleans the fields, removes irrelevant columns, handles missing values, and derives new variables required for analysis.

Key steps:

* Convert transaction dates to datetime
* Generate a Year-Month column
* Aggregate sales, customers, and transaction metrics at the monthly level
* Export the cleaned and aggregated dataset

Output:

* `QVI_monthly_aggregated.csv`

---

## Notebook 2: Control Store Selection

Each trial store must be paired with a control store that behaves similarly before the trial. This ensures that any differences observed during the trial can be attributed to the intervention.

Similarity was measured using:

* Pearson correlation (trend similarity)
* Magnitude distance (performance similarity)

Control stores were ranked, and the best match for each trial store was selected.

Output:

* `control_store_mapping.csv`

---

## Notebook 3: Trial vs. Control Statistical Testing

This notebook compares each trial store with its assigned control store across the trial period.

Steps performed:

* Extract pre-trial and trial windows
* Compare key performance metrics:

  * Total sales
  * Total customers
  * Average transactions per customer
* Conduct statistical tests:

  * Two-sample t-tests
  * Permutation tests

This provides a rigorous method to check whether observed differences are meaningful rather than random.

Output:

* `trial_vs_control_results_YYYY_YY.csv`

---

## Notebook 4: Final Significance Assessment and Results Consolidation

This notebook integrates statistical results and produces final significance labels.

Metrics included:

* Mean performance differences
* Test statistics and p-values
* Permutation-based probability estimates
* Impact classification (significant or not)

Output:

* `notebook4_final_results.csv`

---

## Notebook 5: Drivers of Impact

This stage explains why certain stores showed impact and others did not.

Analysis includes:

* Whether performance uplift was driven by more customers or increased purchasing behavior
* Differences in average basket size and transaction frequency
* Store-specific insights that help the business refine strategy

Output:

* `notebook5_store_impact_summary.csv`

---

## Notebook 6: Executive Summary and Recommendations

This notebook consolidates the results into a clear, business-oriented report. It explains the overall trial outcome, which stores demonstrated significant improvement, and what actions are recommended.

Contents include:

* Statistical conclusions per store
* Interpretation of effect sizes
* High-level business implications
* Suggested next steps for the company

Output:

* `notebook6_executive_summary.txt`

---

# 4. Key Findings

* Some trial stores demonstrated statistically significant uplift in sales and customer behavior.
* Not all stores responded positively to the trial, indicating that the intervention’s effectiveness varies based on store characteristics.
* In successful stores, uplift was caused either by increased customer traffic or by higher spending per customer.
* Statistical testing confirmed which changes were meaningful and which were within expected natural variation.

---

# 5. Methodological Strengths

This project demonstrates the use of:

* Time-series aggregation
* Similarity scoring for experimental design
* Causal inference principles
* Inferential statistics (t-tests, permutation tests)
* Effect size interpretation
* Data-driven story communication

It represents a complete A–Z trial analysis pipeline suitable for real-world retail analytics.

---

# 6. Repository Structure

```
/data
    Raw and processed datasets

/notebooks
    Notebook 1 – Data Cleaning
    Notebook 2 – Control Store Selection
    Notebook 3 – Statistical Testing
    Notebook 4 – Final Results
    Notebook 5 – Drivers of Change
    Notebook 6 – Executive Summary

/outputs
    Aggregated monthly dataset
    Control store mapping
    Trial vs control performance comparisons
    Final significance results
    Impact driver summaries
    Executive summary report

README.md (this file)
```

---

# 7. Project Outcomes

This project provides a reproducible framework that helps leadership:

* Assess trial effectiveness clearly and objectively
* Identify which stores warrant rollout
* Understand why certain stores perform differently
* Improve the design of future retail trials

The analysis supports evidence-based decision-making and reduces uncertainty in strategic initiatives.

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

