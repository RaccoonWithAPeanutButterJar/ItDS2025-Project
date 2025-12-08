# ItDS2025 - Project F4
 AI Impact on job market - Predicting jobs that are at risk (or growing) under the ever rising use of AI
 <br>Team: Nele Taisi Järv, Rico Akiro Kaio, Christen Mägi

## Goal and motivation
Because of the rising popularity of AI use and worry that it might take over many jobs, we decided to base our project off of that to analyse and predict which jobs and industries are or will be at risk of being taken over by AI.

The goal of the project is to perform an analysis of the public Kaggle dataset to find current and projected job trends across industries to then build a predictive model to classify whether a job will be increasing or decreasing by 2030.

## The Dataset
The dataset is a public Kaggle dataset with 30,000 rows and 13 valuable columns, generated to reflect realistic labor market patterns based on ongoing research and public data insights (2024-2030)

Here is a description of each column:
+ Job - Title Name of the job/role (e.g., Data Analyst, Cashier, etc.)
+ Industry - Industry sector in which the job is categorized (e.g., IT, Healthcare, Manufacturing)
+ Job Status - Indicates whether the job is Increasing or Decreasing due to AI adoption
+ AI Impact Level - Estimated level of AI impact on the job: Low, Moderate, or High
+ Median Salary (USD) - Median annual salary for the job in USD
+ Required Education - Typical minimum education level required for the job
+ Experience Required (Years) - Average number of years of experience required
+ Job Openings (2024) - Number of current job openings in 2024
+ Projected Openings (2030) - Projected job openings by the year 2030
+ Remote Work Ratio (%) - Estimated percentage of jobs that can be done remotely
+ Automation Risk (%) - Probability of the job being automated or replaced by AI
+ Location Country - where the job data is based (e.g., USA, India, UK, etc.)

## Repository Structure & How to replicate the Analysis

This repository contains the full analysis pipeline, broken down into four key notebooks.

To replicate the analysis and reproduce the findings presented in this project, the code has been structured into four sequential stages. Please execute the Jupyter Notebooks in the following order:

* **`1_Data_Cleaning.ipynb`**
    * **Goal:** Prepare the raw data for analysis.
    * **Process:** Checks for missing values, duplicates, and verifies data types. Since the synthetic dataset is clean, this notebook confirms data integrity before proceeding.

* **`2_Exploratory_Analysis.ipynb`**
    * **Goal:** Understand the current job landscape.
    * **Key Insights:** Visualizes the distribution of jobs across industries, compares median salaries, and analyzes the relationship between automation risk and projected growth.
    * **Highlight:** Discovered that automation risk averages ~50% across most industries, suggesting broad AI applicability rather than sector-specific targeting.

* **`3_Clustering_Analysis.ipynb`** (Unsupervised Learning)
    * **Goal:** Group jobs into distinct categories based on risk and reward.
    * **Method:** Uses **K-Means Clustering** to segment jobs into three types:
        1.  **Fast-growing specialist roles** (High growth, niche skills).
        2.  **High-paying / High-risk roles** (Vulnerable to automation but lucrative).
        3.  **Low-risk core roles** (Stable, resilient jobs).

* **`4_Predictive_Modeling.ipynb`** (Supervised Learning)
    * **Goal:** Predict future job trends.
    * **Models:**
        * **Classification:** Used Random Forest & KNN to predict if a job's status is "Increasing" or "Decreasing".
        * **Regression:** Attempted to forecast the exact number of `Projected Openings` (2030).
    * **Result:** The classification task proved difficult (approx. 50% accuracy), indicating that job status depends on complex factors beyond just salary and automation risk.

---
