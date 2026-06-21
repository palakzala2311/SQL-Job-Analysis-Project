# SQL Job Analysis Project

## Project Overview
This project analyzes job posting data using SQL and SQLite. The dataset contains information about companies, job titles, countries, salaries, and remote work availability.

## Skills Used
- SQL
- SQLite
- Data Analysis
- Data Filtering
- Aggregation Functions

## Queries Performed

### 1. View All Data
```sql
SELECT * FROM job_postings;
```

### 2. Country-wise Jobs
```sql
SELECT job_country, COUNT(*) AS total_jobs
FROM job_postings
GROUP BY job_country;
```

### 3. Average Salary
```sql
SELECT AVG(salary_year_avg) AS avg_salary
FROM job_postings;
```

### 4. Remote Jobs Count
```sql
SELECT COUNT(*) AS remote_jobs
FROM job_postings
WHERE work_from_home = 1;
```

### 5. Highest Salary Job
```sql
SELECT company_name, job_title, salary_year_avg
FROM job_postings
ORDER BY salary_year_avg DESC
LIMIT 1;
```

## Project Output
- Country-wise job analysis
- Salary analysis
- Remote work analysis
- Highest salary job identification

## Author
Palak Zala
Data Analytics Enthusiast | Python & SQL Learner
