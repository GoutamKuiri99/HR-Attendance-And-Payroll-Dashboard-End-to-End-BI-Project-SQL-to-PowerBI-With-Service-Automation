# 📊 HR Attendance & Payroll Dashboard – End-to-End BI Project

An enterprise-ready **Business Intelligence (BI)** solution built using:

- 🗂️ **SQL Server (Views)** for backend data modeling  
- 📈 **Power BI (Import Mode)** for interactive dashboards  
- ☁️ **Power BI Service** for deployment with scheduled data refresh

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





