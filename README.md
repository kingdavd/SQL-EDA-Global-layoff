# SQL Global Layoffs Analysis

## Project Overview
This project analyzes global layoffs across various industries using SQL. The goal is to identify trends in workforce reductions, determine which industries and companies are most affected, and examine how funding stages and company sizes influence layoffs.

Dataset Details
The dataset includes:
- **Compananies Name**: Organizations that reported layoffs.
- **Location**: The geographical location of the companies.
- **Industry**: The sector in which the companies operate.
- **Total Laid Off**: The total number of employees affected- 
- **Percentage Laid Off**: Proportion of layoffs relative to company size.
- **Date**: The date the layoff event occurred- 2020-03-11	2023-03-06
- - **Country**: The nuber of countrries where layoffs occurred- 
- **Funds Raised (in Millions)**: The total funds raised by the companies-

- **Company Size**: The total number of employees.

 Key Insights
- **Industry Trends**: Industries such as logistics, transportation, and travel have high layoff rates.
- **Funding Stage Impact**: Companies in later funding stages (e.g., Post-IPO, Series C) tend to have larger layoffs.
- **Geographical Impact**: The United States has the highest recorded layoffs in the dataset.

SQL Queries Used
Some key SQL queries used for analysis:
- Finding the first and last recorded layoffs:
  ```sql
  SELECT MIN(DATE), MAX(DATE)
  FROM layoffs_staging2;
  ```
- Summarizing total layoffs by industry:
  ```sql
  SELECT industry, SUM(total_laid_off)
  FROM layoffs_staging2
  GROUP BY industry
  ORDER BY 2 DESC;
  ``


 Author
**David**  
Connect with me on GitHub: [kingdavd](https://github.com/kingdavd)

-

