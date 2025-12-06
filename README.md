# ItDS2025 - Project F4
 AI Impact on job market - Predicting jobs that are at risk (or growing) under the ever rising use of AI
 <br>Team: Nele Taisi Järv, Rico Akiro Kaio, Christen Mägi

## Goal and motivation
Because of the rising popularity of AI use and worry that it might take over many jobs, we decided to base our project off of that to analyse and predict which jobs and industries are or will be at risk of being taken over by AI.

The goal of the project is to perform an analysis of the public Kaggle dataset to find current and projected job trends across industries to then build a predictive model to classify whether a job will be increasing or decreasing by 2030.

## The Dataset
### Dataset Overview
This comprehensive dataset contains detailed information about AI and machine learning job positions, salaries, and market trends across different countries, experience levels, and company sizes. Perfect for data science enthusiasts, career researchers, and market analysts for practice purposes.

#### Dataset Description
What's Inside
It includes detailed salary information, job requirements, company insights, and geographic trends.

#### Key Features:

+ 15,000+ job listings from 50+ countries
+ Salary data in multiple currencies (normalized to USD)
+ Experience level categorization (Entry, Mid, Senior, Executive)
+ Company size impact analysis
+ Remote work trends and patterns
+ Skills demand analysis
+ Geographic salary variations
+ Time-series data showing market evolution

| Column Name | Description | Type |
| :--- | :--- | :--- |
| `job_id` | Unique identifier for each job posting | String |
| `job_title` | Standardized job title | String |
| `salary_usd` | Annual salary in USD | Integer |
| `salary_currency` | Original salary currency | String |
| `salary_local` | Salary in local currency | Float |
| `experience_level` | EN (Entry), MI (Mid), SE (Senior), EX (Executive) | String |
| `employment_type` | FT (Full-time), PT (Part-time), CT (Contract), FL (Freelance) | String |
| `job_category` | ML Engineer, Data Scientist, AI Researcher, etc. | String |
| `company_location` | Country where company is located | String |
| `company_size` | S (Small <50), M (Medium 50-250), L (Large >250) | String |
| `employee_residence` | Country where employee resides | String |
| `remote_ratio` | 0 (No remote), 50 (Hybrid), 100 (Fully remote) | Integer |
| `required_skills` | Top 5 required skills (comma-separated) | String |
| `education_required` | Minimum education requirement | String |
| `years_experience` | Required years of experience | Integer |
| `industry` | Industry sector of the company | String |
| `posting_date` | Date when job was posted | Date |
| `application_deadline` | Application deadline | Date |
| `job_description_length` | Character count of job description | Integer |
| `benefits_score` | Numerical score of benefits package (1-10) | Float |

## TODO
+ Provide a guide to the contents of the repository
+ Explain how to take the code and replicate the same analysis
