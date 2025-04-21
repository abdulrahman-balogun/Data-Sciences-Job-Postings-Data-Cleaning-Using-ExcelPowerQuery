# Data-Sciences-Job-Postings-Data-Cleaning-Using-ExcelPowerQuery

![Image](https://github.com/user-attachments/assets/3ed2793c-682f-419a-acf3-3101e1fac6f6)

## Table of Contents

- [Project Description](#project-description)
- [Uncleaned Dataset](#uncleaned-dataset)
- [Objectives](#objectives)
- [Cleaned Dataset Process](#cleaned-dataset-process)
- [Tools](#tools)
- [Key Insight](#key-insight)

## Project Description
README.txt file tailored to help you analyze your cleaned and uncleaned datasets based on the provided job postings data. These datasets contain information about data science job postings, including job titles, salary estimates, descriptions, company details, and required skills. The goal is to assist users in understanding the data, identifying differences between the uncleaned and cleaned versions, and performing meaningful analyses.

 ### Uncleaned Dataset

File Name: uncleaned_job_postings.csv (or similar, depending on your naming)
Source: Raw data extracted from job postings (e.g., as provided in the document).
Format: CSV (Comma-Separated Values)

-	Description: This is the original, unprocessed dataset containing job postings with potential inconsistencies, missing values, and unformatted text (e.g., job descriptions with embedded newlines or special characters).
- Columns:
-	index: Unique identifier for each job posting.
-	Job Title: Title of the job (e.g., “Data Scientist”, “Senior Data Scientist”).
-	Salary Estimate: Estimated salary range (e.g., “$137K-$171K (Glassdoor est.)”).
- Job Description: Detailed text description of the job, including responsibilities and qualifications.
-	Rating: Company rating (e.g., 3.1, -1 if missing).
-	Company Name: Name of the hiring company (may include rating appended in some cases).
-	Location: Job location (e.g., “New York, NY”).
-	Headquarters: Company headquarters location.
-	Size: Company size (e.g., “1001 to 5000 employees”).
-	Founded: Year the company was founded (e.g., 1993, -1 if unknown).
-	Type of ownership: Ownership type (e.g., “Company - Public”).
-	Industry: Industry of the company (e.g., “Insurance Carriers”).
-	Sector: Sector of the company (e.g., “Insurance”).
-	Revenue: Company revenue (e.g., “$1 to $2 billion (USD)”).
-	Competitors: Known competitors (e.g., “EmblemHealth, UnitedHealth Group, Aetna”, -1 if none listed).
-	Additional columns in some versions (e.g., min_salary, max_salary, avg_salary, python, excel, etc.) indicating parsed salary ranges and required skills.

### Objectives

The datasets objective is to be used for:
- Analyze trends in data science job postings (e.g., salary ranges, required skills, industries).
- Compare the uncleaned and cleaned datasets to understand the impact of data cleaning on analysis results.
- Build predictive models (e.g., salary prediction based on location, skills, or company size).
- Explore company demographics (e.g., size, revenue, founding year).


### Cleaned Dataset Process:

-	File Name: cleaned_job_postings.csv (or similar, depending on your naming)
-	Source: Processed version of the uncleaned dataset.
-	Format: CSV (Comma-Separated Values)

-	Description: This dataset has been cleaned to address issues such as missing values, inconsistent formats, and duplicate entries. It is more suitable for analysis and modeling.
-	Cleaning Steps (example, adjust as per your actual process):
-	Removed duplicate entries based on index or identical job postings.
-	Standardized Salary Estimate by extracting min/max values (e.g., “$137K-$171K” → min_salary=137, max_salary=171).
-	Handled missing values (e.g., replaced “-1” or “Unknown / Non-Applicable” with NaN or imputed values).
-	Cleaned Company Name by removing appended ratings (e.g., “Healthfirst 3.1” → “Healthfirst”).
-	Normalized text fields like Job Description (removed extra newlines, special characters).
-	Converted categorical fields (e.g., Size, Type of ownership) to consistent formats.
-	Added binary skill columns (e.g., python, excel) where applicable, based on job description parsing.
-	Columns: Same as the uncleaned dataset, with additional processed columns (e.g., min_salary, max_salary, avg_salary) and cleaned data.

### Tools:

- Excel
- PowerQuery

### Key Insight

- The key insight from this project is that cleaning the job postings dataset significantly improves data quality, revealing clearer salary trends and skill demands. The cleaned data shows Python and Excel as top skills, with average salaries varying by location and industry, enabling more accurate analysis and predictions.
