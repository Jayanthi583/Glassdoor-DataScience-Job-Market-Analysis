# Glassdoor-DataScience-Job-Market-Analysis
Glassdoor Data Science Jobs Exploratory Data Analysis (EDA)
Problem Statement
This project aims to provide a comprehensive understanding of the Data Science job market by analyzing job postings from Glassdoor. The goal is to identify key trends related to job titles, locations, salary expectations, company types, and the most in-demand technical skills, helping aspiring data scientists and companies navigate the landscape.

Approach & Methodology
This Exploratory Data Analysis (EDA) project involved a systematic approach to uncover insights from the Glassdoor job postings dataset:

Data Acquisition & Initial Setup:
The dataset (Glassdoor_Job_Postings.csv) was loaded into a Pandas DataFrame.
Initial setup included configuring Matplotlib and Seaborn for enhanced visualizations.

Data Cleaning & Preprocessing:
Performed rigorous data cleaning to standardize text fields (location, job_title) by stripping whitespace and normalizing casing.
Salary data (salary_avg_estimate) was meticulously cleaned by removing currency symbols (₹), commas, and handling null values, followed by conversion to a numeric format.
Missing values in critical columns (salary_avg_estimate, job_title, location) were handled by dropping relevant rows to ensure data integrity for analysis.

Job Market Analysis:
Conducted frequency analysis to identify Top 10 Job Titles, Top 10 Job Locations, and Top Hiring Companies, visualized using Seaborn bar plots.
Explored Salary Trends, including salary distribution and average salaries for top job titles and locations, presented with customized bar plots.
Analyzed Company Insights, specifically focusing on Work-Life Balance Ratings for top companies.
Identified prevalent Technical Skill Requirements by extracting and counting mentions of various technical skills (python, sql, machine learning, pytorch, aws, etc.) from job descriptions using regular expressions and Python's collections.Counter.

Company Categorization & Salary Comparison:
Manually mapped and categorized companies into Product MNC, Service MNC, and Startup types.
Calculated and visualized the median salary across these defined company categories, applying data capping to mitigate outlier influence.
Visualization & Interpretation:
Utilized Matplotlib and Seaborn extensively to create clear and informative data visualizations, including bar plots with annotations for easy interpretation.
Transformed average salaries into Lakhs INR for better readability and contextual understanding.

Techniques & Tools Used
Programming Language: Python
Data Manipulation & Analysis: Pandas, NumPy
Data Visualization: Matplotlib, Seaborn
Text Processing: re (Regular Expressions) for skill extraction
Utility: collections.Counter for frequency counting, warnings for suppression
