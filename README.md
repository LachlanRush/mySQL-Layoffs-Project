# mySQL Layoffs Project
A mySQL project to clean and analyse layoff data, showcasing my skills in database management and SQL querying.

## Overview
I built this project to process layoff data through data cleaning and analysis, using mySQL to handle duplicates, standardise data, and extract trends.

## Files
- `layoffs_cleaning.sql`: Removes duplicates, standardises data, and handles nulls.
- `layoffs_analysis.sql`: Analyses layoffs by company, industry, and time.

## Key Skills
- Cleaning: Deduplicated and standardised data with CTEs and joins.
- Analysis: Aggregated data and calculated rolling totals with window functions.
- mySQL: Designed schemas and wrote efficient queries.

## Sample Query
```sql
SELECT SUBSTRING(`date`, 1, 7) AS `MONTH`, SUM(total_laid_off) 
FROM layoffs_staging2 
GROUP BY `MONTH`;
