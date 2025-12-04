 
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
| EmployeeID 
| EmployeeName 
| PositionID 
| ManagerID 
| RecruitmentSource 
| Salary
| DateOfHire 
| DateOfTermination 

# *2. Positions Table*
| Column | Description |
|--------|-------------|
| PositionID 
| PositionName 
| Department 

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
- Hiring and Attrition Trend Line Chart
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
- High overall attrition(33.4%) : Investigate top exists reasons,conduct stay interviews and improve retention drivers.

- Production Department has highest attrition : Review workload,supervisor behaviour,shift patterns and provide targeted training
  /support.

 - Technician and production roles show maximum exists : Recheck hiring quality,onboarding,job clarity and provide skill-focused
   development programs.

 - Employees with 1-3 years tenure leave the most : Strengthen early career engagement,mentorshipand structured career pathing 
   during this period.

 - IT/Data analyst and software enginner show lower attrition : Study what works well in these teams and apply those best practices
   across high risk department.

 - Google search recruits show highest attrition : Improve screen quality, revise job ads and evaluate candidate properly.

 - Indeed recruits are more stable and stay longer : Increase hiring percentage from indeed and reinforce partnership with this 
   source.       

---




