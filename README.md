# Railway Failure Analysis (Power BI Dashboard Project)

## Project Overview
This project analyzes railway system failures to identify patterns, root causes, and operational risks. The goal is to improve system reliability and support proactive maintenance using data-driven insights.

---

## Objectives
- Analyze failure trends across regions and components  
- Identify high-risk failure categories  
- Improve maintenance planning and decision-making  

---

## Key Contributions
- Analyzed failure datasets to identify recurring issues  
- Built interactive dashboards using Power BI  
- Highlighted critical failure patterns and downtime impact  
- Provided insights for improving operational efficiency  

---

## Tools & Technologies
- Power BI  
- SQL  
- Excel  

---

## Dashboard Highlights
- Failure trends over time  
- Region-wise failure distribution  
- Component-level failure analysis  
- Downtime impact analysis  

---

## Sample SQL Queries

```sql
-- Count failures by component
SELECT component, COUNT(*) AS failure_count
FROM failure_data
GROUP BY component
ORDER BY failure_count DESC;

-- Failure trend over time
SELECT DATE(failure_date) AS date, COUNT(*) AS total_failures
FROM failure_data
GROUP BY DATE(failure_date)
ORDER BY date;

-- Identify high-risk components
SELECT component
FROM failure_data
GROUP BY component
HAVING COUNT(*) > 50;

-- Total downtime analysis
SELECT SUM(downtime) AS total_downtime
FROM failure_data;
```

---

## Key Insights
- Identified high-frequency failure components  
- Detected regions with maximum system failures  
- Highlighted peak failure periods  
- Improved visibility into operational risks  

---

## Note
This project demonstrates data analysis and visualization using Power BI along with SQL-based analysis for identifying failure patterns.
