# 📊 HR Attendance & Payroll Dashboard – End-to-End BI Project

An enterprise-ready **Business Intelligence (BI)** solution built using:

- 🗂️ **SQL Server (Views)** for backend data modeling  
- 📈 **Power BI (Import Mode)** for interactive dashboards  
- ☁️ **Power BI Service** for deployment with scheduled data refresh
  
--- 

https://github.com/user-attachments/assets/48f75ef1-2730-41af-b4f9-afc5507beec3

--- 


## 📘 Content Flow Table – HR Attendance & Payroll Dashboard

| Section | Content Title | Purpose / Description |
|--------|----------------|------------------------|
| 1️⃣ | 📌 Business Problem | Highlights the challenges faced by HR such as manual attendance tracking, payroll errors, and scattered reporting systems. |
| 2️⃣ | 🎯 Project Overview | Introduces the HR BI Dashboard and explains its goals of automation, accuracy, and centralized analytics. |
| 3️⃣ | 🎯 Objectives | Defines measurable outcomes like attendance monitoring, leave tracking, net pay analysis, and policy transparency. |
| 4️⃣ | 📚 Table of Contents | Page-wise list of report visuals like Attendance Dashboard, Payroll Summary, and Leave Trend. Makes navigation easier. |
| 5️⃣ | 📁 Data Sources | Describes SQL Server Views and custom Power Query tables used for data integration and model building. |
| 6️⃣ | 📊 Data Modeling | Explains the Galaxy Schema with multiple fact tables and shared dimensions used to design a robust HR data model. |
| 7️⃣ | 🔗 Many-to-Many Handling | Showcases the bridge table used to resolve PF contribution date ambiguity using `Month_Year_Bridge`. |
| 8️⃣ | 🖼️ Report Pages with Screenshots & Explanation | Visual tour of every report page with business explanation and why each one matters. |
| 9️⃣ | 🛠️ Key Dashboard Features | Lists interactivity features like drillthrough, slicer sync, conditional formatting, and mobile responsiveness. |
| 🔟 | ⚙️ Tech Stack | Lists all tools used: Power BI, SQL Server, Power Query, DAX, and Gateway. |
| 1️⃣1️⃣ | 🔁 Scheduled Refresh | Explains how the report stays up-to-date using Power BI Service and Gateway auto-refresh. |
| 1️⃣2️⃣ | 🔁 Dashboard Sharing | Describes the process of sharing dashboards securely with role-level access to HR, Finance, and Admins. |
| 1️⃣3️⃣ | 📌 Conclusion | A high-impact summary of project benefits — transforming manual HR tasks into a strategic digital command center. |
| 1️⃣4️⃣ | 👨‍💻 About the Author | Provides your contact, LinkedIn, and Medium profile links for recognition and networking. |


> 🧭 **How to Use This Table:**  
This content flow table acts as a roadmap to the entire HR Attendance & Payroll Dashboard project.  
It provides a section-wise breakdown of every insight, visualization, and feature explained in the README.

- 📂 From identifying the business problem and defining goals,  
- 🧠 To showing data sources, schema modeling, and resolving complex relationships,  
- 📈 To giving a visual walkthrough of each dashboard page,  
- 🛠️ And finally showcasing the technologies, security, automation, and business impact —  

This README captures the **end-to-end journey** of transforming raw HR data into a powerful, interactive BI solution.

➡️ Use this table to **quickly navigate** and **understand each component** of the project.

---

## 🚨 Business Problem

In a rapidly growing organization, the HR department was struggling with multiple challenges that impacted efficiency and accuracy:

- **Attendance Tracking Errors**: Manual attendance registers and outdated systems led to frequent mismatches and inaccuracies in employee presence data.
- **Salary Miscalculations**: Due to inconsistent data sources and lack of automation, payroll processing often resulted in errors — causing employee dissatisfaction and rework.
- **Manual Payroll Processing**: A significant portion of time and effort was spent on preparing monthly salary sheets, calculating deductions, and generating payslips.
- **Lack of Centralized HR Reporting**: With data scattered across Excel files and departmental records, the HR and Finance teams lacked a unified platform to monitor key metrics like attendance trends, leave patterns, and payroll costs.

These problems not only slowed down operations but also hampered data-driven decision-making. There was a pressing need for a centralized, automated, and interactive BI solution to streamline HR processes, reduce errors, and empower stakeholders with real-time insights.

## 🎯 Project Overview

To address the challenges faced by the HR department, we developed an **end-to-end HR Attendance & Payroll Dashboard** using **Power BI** and **SQL Server**.

This interactive BI solution brings together all critical HR and payroll data into a **centralized, easy-to-navigate dashboard**. It empowers HR managers, finance teams, and leadership to monitor employee attendance, analyze payroll expenses, and ensure compliance — all in real time.

The project integrates multiple data sources, applies robust data modeling using SQL views, and leverages Power BI’s visualization and analytical capabilities to offer a **complete, automated HR reporting ecosystem**.

From high-level KPIs like total net pay and attendance percentage to granular-level insights like individual payslips and department-wise payroll distribution — this dashboard covers it all.

---

## 🎯 Objectives

This project aims to deliver a full-scale HR dashboard that enables stakeholders to:

- 📅 Monitor employee and contractor **attendance trends**, including present, absent, and leave patterns.
- 📈 Track **leave application trends** and **absenteeism** behavior across departments.
- 💵 Analyze **Net Pay** distribution by **role**, **department**, and **contractor type**.
- 🏦 Evaluate **PF contributions** across different roles and departments.
- ⚙️ Provide **admin-level filters** and enable **exporting** for tailored reporting needs.
- 📜 Maintain and display centralized **HR policies** for compliance and transparency.

---

## 📚 Table of Contents

| Report Page | Description |
|-------------|-------------|
| 📌 **Overview** | Summary of key HR KPIs including total employees, contractors, attendance rate, and payroll snapshot. |
| 👥 **Employee & Contractor Directory** | Detailed list of employees and contractors with designations, departments, joining dates, and contact info. |
| 🧩 **Workforce Structure** | Visual breakdown of employee vs contractor count across various departments. |
| 📆 **Shifts & Holidays** | Department-wise shift patterns and categorized holiday schedules (National, Regional, Company-specific). |
| 📊 **Attendance Dashboard** | Day-wise view of Present, Leave, Half Day, and Absent stats with departmental filtering. |
| 👤 **Individual Attendance Insight** | Drilldown into employee-wise attendance behavior including check-in/out time trends. |
| 📉 **Leave & Absentee Trends** | Month-over-month trend analysis for Leave and Absent categories, with department comparison. |
| 📝 **Leave Summary & Application Trend** | Breakdown of leave types availed and trends in employee leave applications over time. |
| 💰 **Payroll Summary** | Net Pay distribution analyzed by department and contractor division; also shows salary component breakdown. |
| 🏦 **PF Contribution** | Visual report on Provident Fund contributions across roles and departments mirroring payroll structure. |
| ⚙️ **Admin Filters & Data Export** | Dynamic filters for role, department, and contractor data export-ready reports. |
| 📜 **HR Policies** | Static documentation page outlining key HR rules and company policy highlights. |

---
## 📁 Data Sources

This dashboard integrates multiple datasets, primarily sourced through **SQL Server Views** and a custom **calendar table** in Power BI. Below is a breakdown of all connected data sources:

### 🗄️ SQL Server – Live Data via Views

The following views are used to model and analyze attendance, payroll, leave records, and workforce distribution:

| View Name | Description |
|-----------|-------------|
| `VIEW_ATTENDANCE_LOG` | Captures employee and contractor attendance logs including check-in/out timestamps and work status. |
| `VIEW_CONTRACTOR_MASTER` | Contains detailed information about contractors and their associated departments. |
| `VIEW_EMPLOYEE_MASTER` | Master data for employees including personal details, roles, departments, and designations. |
| `VIEW_HOLIDAY_CALENDAR` | A structured holiday table covering company-wide, regional, and national holidays. |
| `VIEW_LEAVE_RECORD_TABLE` | Stores leave application data, approval statuses, and categorized leave types. |
| `VIEW_PAYROLL_TABLE` | Monthly payroll summary including gross pay, deductions, and net salary figures. |
| `VIEW_PF_CONTRIBUTION` | Records of Provident Fund contributions split by employee and employer across all departments. |
| `VIEW_SHIFT_MASTER` | Defines shift schedules for different departments and employee categories. |


### 📆 Power BI – Custom Date Table (Power Query)

In addition to SQL Server data, a custom **date/calendar table** was created in Power Query using `My_Calendar`, enabling seamless:

- Time intelligence functions (YTD, MTD, QTD)
- Proper join with attendance & payroll dates
- Flexible date-based filtering in slicers

⚠️ **Note**:  
Make sure your Power BI Desktop or Power BI Service is properly authenticated with SQL Server. After publishing to Power BI Service:

- Update your **SQL credentials** in **Data Source Settings**
- Configure your **Personal Gateway** to support automatic **Scheduled Refresh**
- Verify **Data Privacy Levels** to avoid refresh errors

---
## 📊 Data Modeling

The data model used in this project is based on a **Galaxy Schema** (also known as a Fact Constellation Schema), which is well-suited for handling complex HR and Payroll systems involving multiple business processes.

![image](https://github.com/user-attachments/assets/4c5c0b87-7540-4529-90cf-77b9d11370c6)


### 🛰️ Why Galaxy Schema?

This model includes **multiple fact tables**, each focusing on a different HR function:

| Fact Table | Description |
|------------|-------------|
| `VIEW_ATTENDANCE_LOG` | Stores daily check-in/out logs and attendance status |
| `VIEW_LEAVE_RECORD_TABLE` | Captures employee leave requests and approvals |
| `VIEW_PAYROLL_TABLE` | Holds monthly payroll details including earnings and deductions |
| `VIEW_PF_CONTRIBUTION` | Tracks Provident Fund contributions across employees |

These fact tables share a set of common **dimension tables**, such as:

| Dimension Table | Description |
|------------------|-------------|
| `VIEW_EMPLOYEE_MASTER` | Employee demographic and role data |
| `VIEW_CONTRACTOR_MASTER` | Contractor profile data |
| `VIEW_SHIFT_MASTER` | Shift definitions and timings |
| `VIEW_HOLIDAY_CALENDAR` | Calendar of company-wide, regional, and national holidays |
| `My_Calendar` | Custom date dimension for time intelligence functions |

### 🔗 Relationships & Optimization:

- Many-to-one relationships from fact to dimension tables
- Centralized `My_Calendar` enables time-based filters and YTD/MTD/QTD analysis
- DAX measures handle aggregations and KPIs
- Ready for implementing **Row-Level Security (RLS)** via bridge tables if required

## 🔗 Handling Many-to-Many Relationship

In this HR dashboard project, a complex **many-to-many relationship** was resolved using a well-structured **bridge table** with controlled relationship directions and clean time-based joins.

---

### 💡 Problem Scenario

The `VIEW_PF_CONTRIBUTION` table contains multiple entries per employee for each month, and directly linking its `Date` column to the `My_Calendar` table caused ambiguity due to **repeating Month-Year combinations** in both tables.

Both:
- `VIEW_PF_CONTRIBUTION[Month_Year]`
- `My_Calendar[Month_Year]`

had duplicate values, which led to a **many-to-many cardinality conflict** — making DAX measures and time-based visuals unreliable.

---

### 🛠️ Solution: Month-Year Bridge Table

To resolve this, a custom **bridge table** named `Month_Year_Bridge` was created, holding only **unique Month-Year combinations**, and it serves as an intermediary between both tables.

#### 📂 Table: `Month_Year_Bridge`

---

### 📅 My_Calendar Table

The `My_Calendar` table is a **custom date dimension table** created using Power Query. It includes:

- `Date`
- `Month`
- `Month_Num`
- `Quarter`
- `Year`
- `Month_Year` (formatted as "MMM-YYYY")

This allows advanced **time intelligence** (YTD, MTD, QTD) across the dashboard.

---

### 🔗 Relationship Structure

![image](https://github.com/user-attachments/assets/b9d13971-757e-410f-a4ad-d1e7e3b6406b)

- `My_Calendar[Month_Year]` → `Month_Year_Bridge[Month_Year]`: **Many-to-One**
- `Month_Year_Bridge[Month_Year]` → `VIEW_PF_CONTRIBUTION[Month_Year]`: **One-to-Many**
- Cross-filter direction: **Both**

### 🛠️ Why This Works

- The bridge table acts as a mediator, preventing ambiguity in filtering between two datasets having repeated `Month_Year` values.
- With **bi-directional filters**, any selection in `My_Calendar` will propagate through the bridge and correctly filter `PF Contribution` data.
- This maintains full compatibility with other date-based measures like **Monthly PF Totals**, **YTD**, and **Monthly Comparison**.

### ✅ Result

- Seamless time intelligence for PF-related visuals.
- Cleaner and scalable data model.
- Accurate monthly aggregation across all date-synced tables.

## 🖼️ Report Pages with Screenshots & Explanation

Below is a walkthrough of the key report pages in the HR Attendance & Payroll Dashboard. Each page is designed to answer a specific business question using clean, interactive visuals and impactful metrics.

---

### 📌 1. HR Overview

**What it Shows:**  
Key HR KPIs such as:
- **Total Employees:** 100
- **Active Employees:** 80
- **Resigned Employees:** 20
- **Contractors:** 10 (Active: 8)
- **Overall Attendance Rate:** 83.34%

**Why it Matters:**  
Gives stakeholders a one-glance health check of the overall workforce and hiring-retention trend.

![image](https://github.com/user-attachments/assets/467fab9f-7bab-4e13-9d70-51d386e2feb3)

---

### 👥 2. Employee & Contractor Directory

**What it Shows:**  
- Department-wise Employee Listing
- Detailed employee profiles: Name, DOJ, Department, Designation
- All 10 contractors listed with contact persons and phone numbers

**Why it Matters:**  
Acts as a live reference directory, eliminating manual lookup from HR spreadsheets.

![image](https://github.com/user-attachments/assets/61be96ae-7f92-482b-870a-485004cc61d7)

---

### 🧩 3. Workforce Composition

**What it Shows:**  
- Department-wise employee distribution
- Donut chart for contractor spread (uniformly distributed)

**Why it Matters:**  
Helps identify over- or under-staffing across business units.

![image](https://github.com/user-attachments/assets/8864bb7c-67ff-4eed-9cd5-f1baf79600ec)

---

### 🕒 4. Shift & Holiday Analysis

**What it Shows:**  
- Total shifts defined: 7  
- Next upcoming holiday: **15 August**
- Holiday classification: National (10), Regional (6), Company (4)
- Detailed shift timings per role/division

**Why it Matters:**  
Crucial for workforce scheduling and planning long weekends or business closures.

![image](https://github.com/user-attachments/assets/a595bea5-031b-4fb2-9fbe-83f1a85ba207)


---

### 📅 5. Attendance Analysis

**What it Shows:**  
- Daily status summary: Present, Leave, Half-Day, Absent  
- Actual in-time and out-time stamps  
- Sample drilldown for employees like **Aarti Tiwari**:
  - Avg In-Time: 09:15
  - Avg Out-Time: 18:15–19:00
  - Avg Working Hours: ~9 hrs/day

**Why it Matters:**  
Enables micro-level analysis of employee punctuality and attendance discipline.

![image](https://github.com/user-attachments/assets/b9df279d-53b3-4bcc-a70f-a6cdaa582bb3)

---

### 👤 6. Employee Attendance Behavior

**What it Shows:**  
- Trend visuals for each employee:
  - In-Time Pattern
  - Out-Time Pattern
  - Working Hours Trend

**Why it Matters:**  
Helpful for HR to identify overworking or underworking staff and enforce work-life balance.

![image](https://github.com/user-attachments/assets/f9ac4177-9f1d-4632-81f9-7f0043b20a88)


---

### 📈 7. Attendance Trends Over Time

**What it Shows:**  
- Month-wise attendance breakdown including:
  - ✅ Present
  - 🚫 Absent
  - 💤 Leave
  - 🌓 Half-Day
- Department-wise monthly attendance performance
  - 📊 Average across all departments: **83.90%**

**Why it Matters:**  
This report helps HR identify **seasonal patterns**, spot **departments with low attendance**, and enforce better workforce planning. It also supports policy reviews by highlighting **absenteeism spikes** and **monthly behavioral trends**.

![image](https://github.com/user-attachments/assets/98bb2605-0ecf-4010-85be-1d5d5e76155a)

---
### 💡 8. Attendance Health Score Analysis

**What it Shows:**  
- Visualizes **Attendance Health Score** — the percentage of employees present across each **month** and **department**
- Tracks attendance trends and highlights overall engagement levels
- Example stats:
  - 📈 Highest Attendance %: **November – 101.92%**
  - 📉 Lowest Attendance %: **February – 69.64%**
  - 🧾 Department-Wise Average: **83.90%**

**Why it Matters:**  
This section helps HR monitor presence patterns across months and departments, identify problem areas, and take corrective actions to maintain workforce productivity.

![image](https://github.com/user-attachments/assets/03b0ae75-d159-4917-ba25-cbd0fece5a17)

---

### 📉 8. Leave & Absence Trends

**What it Shows:**  
- Separate trends for:
  - Leave Application Count (Type-wise)
  - Absence Rate (with department filter)

**Why it Matters:**  
Highlights patterns in voluntary vs. unplanned absenteeism and helps refine leave policies.

### **Leave**
![image](https://github.com/user-attachments/assets/86e0ea09-dd40-4816-a444-5cef056b1f83)

#### **Absence Rate**
![image](https://github.com/user-attachments/assets/aabcbbb1-726b-4885-bf21-c105dcc2a962)

#### **Leave Application Count (Type-wise)**
![image](https://github.com/user-attachments/assets/7c16d99c-cb61-4918-8c92-e4c855042527)

---

### 💰 9. Payroll Summary

**What it Shows:**  
- Net Pay distribution:
  - **By Role**
  - **By Department**
  - **By Contractor Status**
- Salary component breakdown (Basic, HRA, Allowances, Deductions, Net Pay)

**Why it Matters:**  
Helps HR/Finance review salary alignment and fairness across designations and teams.

![image](https://github.com/user-attachments/assets/c1a21956-196b-487e-bea4-7cb95f617f37)

![image](https://github.com/user-attachments/assets/80022c7f-8cbd-4b6e-8b0b-efe17ec7acf2)

![image](https://github.com/user-attachments/assets/dcb296aa-6c47-4321-b515-a4cc9f2834b8)


---

### 🏦 10. PF Contribution Analysis

**What it Shows:**  
- Monthly PF contributions for employees
- Split: Employee Share vs. Employer Share
- Breakdown by Department and Role

**Why it Matters:**  
Ensures transparency and audit compliance for statutory contributions.

![image](https://github.com/user-attachments/assets/6480f778-1ef7-4ab0-bc20-ab3a631450e2)

![image](https://github.com/user-attachments/assets/2959e6bd-6441-4322-9550-73ff88760596)


---

### ⚙️ 11. Admin Filters & Export

**What it Shows:**  
- Filters to slice by:
  - Contractor
  - Department
  - Designation
- Direct export to Excel button for customized datasets

**Why it Matters:**  
Empowers HR/Admin to generate quick department-wise reports and perform ad hoc analysis.

![image](https://github.com/user-attachments/assets/162e049a-d49c-4c85-ad32-0f6196042897)

---

### 📜 12. HR Policies

**What it Shows:**  
Summarized HR policies such as:
- Leave eligibility
- Shift policies
- Working hour structure
- Rules for overtime and weekly offs

**Why it Matters:**  
Brings clarity and promotes consistency in internal communication.

![image](https://github.com/user-attachments/assets/ddd2aff1-a244-4b35-8b1f-f5690fb0ab43)

---

## 🛠️ Key Dashboard Features

🎯 **Drillthrough to Employee Profile:**  
Clicking on any employee or contractor in summary charts opens a dedicated page showing their full attendance log, salary breakdown, and leave history.

🔄 **Sync Slicers Across Pages:**  
Filters like **Department**, **Month-Year**, or **Employee Status** stay consistent across all report pages — helping HRs explore data seamlessly.

📁 **Dynamic Role-Based Filtering:**  
Separate views for **Employees** and **Contractors**, with department-level slicing, using DAX-based role segmentation.

🕵️ **Conditional Formatting for Attendance & Pay Health:**  
Highlights abnormal behavior like high absenteeism, zero working hours, or large net pay deductions using intuitive color schemes.

🧠 **Time Intelligence with DAX:**  
Enables **MoM (Month-over-Month)**, **YTD**, and **Monthly Comparison** of attendance % and salary components.

📂 **Drillable Leave Trends:**  
Clicking on leave type charts shows individual employee leave logs and department-level leave patterns.

📱 **Mobile-Responsive Layout:**  
Dashboard layout adapts well to mobile and tablet screens on Power BI Service — handy for HRs on the move.

🔐 **Security via Row-Level Filters:**  
Each manager or department head sees only their team's data via Row-Level Security (RLS), ensuring privacy and compliance.

📤 **Export-Ready Reports:**  
Admin filters allow slicing and exporting employee-specific datasets directly into Excel — perfect for audits or MIS reporting.

---

## ⚙️ Tech Stack

- 💻 **Power BI Desktop** – Dashboard design, data modeling, and DAX calculations  
- 🧩 **SQL Server (Views)** – Source system with multiple view tables for HR data  
- 📅 **Power Query** – Used for custom `My_Calendar` table creation and multiple data transformations:  
  - Added columns like Month-Year, Financial Year, Week Number, IsWeekday, etc.  
  - Cleaned and reshaped data from SQL views before loading to model  
  - Shifted calculated columns to Power Query to avoid heavy DAX and improve performance  
- 🔢 **DAX** – Calculations for Net Pay, Attendance %, PF, and time-based metrics  
- ☁️ **Power BI Service** – Dashboard published and shared with HR/Admin teams  
- 🔁 **Power BI Gateway** – Enables scheduled refresh from SQL Server
  
---

## 🔁 Scheduled Data Refresh

The dashboard is deployed on **Power BI Service** with a configured **Personal Gateway** to enable automated data refresh.

- 🔗 Connected directly to **SQL Server Views**
- ⏰ **Scheduled Refresh** set up to run daily for up-to-date insights
- ✅ Ensures that HR and Payroll reports reflect the **latest attendance logs**, **leave records**, and **salary updates**
- 🔒 Refresh setup is secured and monitored via Gateway Status in Power BI Service

![image](https://github.com/user-attachments/assets/51cedf0a-4794-40dc-91ae-618b4d3695a4)

----

## 🔁 Sharing the Dashboard

Once the scheduled refresh is enabled, the dashboard is shared with HR, Admin, and Finance stakeholders using the following approach:

1. 📤 **Published to Power BI Service**  
   The final report is deployed to the Power BI workspace for centralized access.

2. 🔗 **Shared via Dashboard Link or Embedded in HR Portal**  
   Direct sharing through Power BI link or embedded within the company’s internal tools like SharePoint or intranet portals.

3. 🔐 **Role-Based Permissions for Secure Access**  
   - **HR Managers** see department-wise employee data  
   - **Finance Users** access payroll and PF components  
   - **Admins** can export and manage full employee datasets  
   Row-Level Security (RLS) ensures that each user sees only the data relevant to their role.

--- 

## 📌 Conclusion

This HR Attendance & Payroll Dashboard is not just a report — it's a **strategic command center** for the entire HR ecosystem.

It transforms scattered SQL data into a **visually-rich, centralized, and interactive platform** that empowers HR teams, streamlines payroll operations, and gives leadership **real-time insights** into the most valuable asset: the workforce.

🚀 **Impact Delivered:**
- Reduced payroll processing time from hours to minutes
- Eliminated manual tracking errors in attendance & leave records
- Enabled department heads to drill down into performance and absenteeism trends
- Provided finance with accurate, role-wise salary distribution & PF compliance
- Established a scalable system ready for multi-location HR expansion

🔐 With row-level security, dynamic DAX intelligence, and automated refreshes, this dashboard isn’t just a project — it’s a **future-ready HR solution** that adapts, informs, and delivers value every single day.

> 💬 _"From gut-feeling to data-backed decision-making — this dashboard changes the game for HR."_

✨ Whether it’s optimizing shift schedules, auditing pay structures, or tracking attendance anomalies — **everything is now just a click away.**

--- 

## 👨‍💻 About the Author
- **Name**: Goutam Kuiri
- **Contact**: gkuiri26@gmail.com
- **LinkedIn**: [Goutam Kuiri](https://www.linkedin.com/in/goutam-kuiri-949b632a6)
- **Medium**: [Goutam Kuiri](https://medium.com/@goutamkuiri)




