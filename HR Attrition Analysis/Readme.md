 
 # Project Title
 HR Attrition Analysis Dashboard

---

#  Project Overview
The HR team wants a clear view of the company's workforce: Employee distribution,hiring trends,tenure,attrition patterns and department level insights.

The goal is to help HR identify high risk areas monitor staffing levels, and make data driven decisions.

---

#  Key Objectives
- Identify *attrition patterns* and high-risk areas  
- Monitor *hiring vs termination trends* 
- Understand *workforce distribution*
- Build an interactive Power BI dashboard with drill-downs  

---

# Tools Used
- *Power BI Desktop*
- *Power Query*
- *DAX*
- *Data Modeling*
- *Data Visualization*

---

#  Data Sources
Data was provided in two tables:

# *1. Employees Table*
| Column | Description |
|--------|-------------|
| EmployeeID | Unique employee identifier |
| EmployeeName | Name of employee |
| PositionID | Foreign key for position |
| ManagerID | Reporting manager |
| RecruitmentSource | Employee recruitment source |
| Income | Employee monthly income |
| DateOfHire | Hiring date |
| DateOfTermination | Termination date (blank if active) |

# *2. Positions Table*
| Column | Description |
|--------|-------------|
| PositionID | Unique job position ID |
| PositionName | Role name |
| Department | Department name |

---

# Data Cleaning & Transformations
All cleaning was done in **Power Query**:

#  Changed Data Types  
- Date columns → Date  
- Income → Whole Number  
- IDs → Text  

# Created "Status Column"

If DateOfTermination is null → "Active" Else → "Terminated".

# Created "Manager Level Column"
 Null in ManagerID Created conditional column to label CEO as "Top Level".

# Created "Tenure Column and Tenure Bucket Column"
  To identify tenure of employees and classify that tenure in buckets format.  

# Established Relationships
- *Employees[PositionID] → Positions[PositionID]* (Many-to-One).

---

# Visuals Included in Dashboard
# 1. KPI Cards
- Total Employees  
- Active Employees  
- Attrition 
- Attrition Rate  
- Average Salary  
- Average Tenure

# 2. Charts
- Attrition Trend Line Chart
- Active Employees And Attrition Employees Donut Chart
- Recruitment Wise  Attrition Stacked Column Chart
- Department-Wise Attrition Stacked Bar Chart
- Position-Wise Attrition Clusterd Bar Chart
- Tenure Wise Attrition Stacked Column Chart
 
 

# 3. Filters / Slicers
- Department  
- Recruitment Source  

---



 # Insights Gained
- High overall attrition(33.4%) .

- Production Department has highest attrition.

 - Technician and production roles show maximum exists. 

 - Employees with 1-3 years tenure leave the most.

 - IT/Data analyst and software enginner show lower attrition.

 - Google search recruits show highest attrition.

 - Indeed recruits are more stable and stay longer.       

---





