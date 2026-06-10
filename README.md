# HR-Attrition-Analysis-
HR Attrition Analysis Dashboard using Tableau and SQL
# 👥 HR Attrition Analysis Dashboard

## 📊 Project Overview
An interactive HR dashboard built using Tableau to analyze 
employee attrition patterns across departments, age, gender, 
job roles and marital status.

## 🛠️ Tools Used
- Tableau (Dashboard & Visualization)
- SQL / SQLite (Data Analysis & Querying)

## 📈 Dashboard Features
- Attrition by Department (Bar Chart)
- Attrition by Age (Bar Chart)
- Attrition by Gender (Bar Chart)
- Attrition by Marital Status (Bar Chart)
- Attrition by Job Role (Bar Chart)

## 🔍 Key Insights
- Research & Development has highest attrition (133 employees)
- Employees aged 25-35 have highest attrition rate
- Single employees leave more than married or divorced
- Male employees have higher attrition (150) vs Female (87)
- Managers earn highest average income ($17,181)

## 💻 SQL Queries
### Attrition by Department
SELECT department, attrition, COUNT(*) AS Employee_Count
FROM WA_FnUseC_HREmployeeAttrition
GROUP BY department, attrition
ORDER BY department;

### Average Income by Job Role
SELECT jobrole, ROUND(AVG(monthlyincome), 2) AS Avg_Income
FROM WA_FnUseC_HREmployeeAttrition
GROUP BY jobrole
ORDER BY Avg_Income DESC;

## 📷 Dashboard Screenshot
![Dashboard](hr_dashboard.png)
