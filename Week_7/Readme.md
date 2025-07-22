# 📁 Week 7 Submission – Power BI Project

## 📌 Overview

In Week 7, the focus shifted toward making the Power BI solution **production-ready** by incorporating **automation**, **data refresh scheduling**, and **version management**. This week also covered best practices in organizing report assets and creating scalable deployment workflows.

---

## ✅ Key Activities

### 1. 🔄 Data Refresh Automation

- Configured **Power BI Gateway** to allow scheduled refresh of on-premise datasets
- Set up **scheduled refresh frequency** (daily/weekly) based on stakeholder needs
- Enabled **refresh failure alerts** to notify the data team via email

### 2. 🔗 Data Source Credential Management

- Reviewed and updated **data source credentials** in Power BI Service
- Tested access tokens and privacy level settings to avoid refresh errors
- Verified OAuth2 configurations for external APIs or cloud sources (if applicable)

### 3. 📂 Workspace and Version Management

- Created **version-controlled report files** using naming conventions (`v1.1`, `v2.0`)
- Organized Power BI workspace into logical folders:
  - Dev / QA / Production reports
  - Archived vs. active dashboards
- Documented changes in a **version log** to track enhancements and bug fixes

### 4. 📊 Monitoring & Usage Analytics

- Used **Power BI Admin Portal** and **Usage Metrics Report** to:
  - Track report views and active users
  - Identify underused pages or visuals
  - Analyze performance bottlenecks post-deployment

### 5. 🧹 Dashboard Maintenance & Audit

- Conducted a full **report audit**:
  - Removed unused columns and queries
  - Optimized relationships and indexing
  - Verified consistency across slicers and filters
- Documented all Power BI tables, columns, measures in a **Data Dictionary**

---

## 🧰 Tools & Features Used

- Power BI Service (Workspace, Gateways, Usage Metrics)
- Data Gateway Setup
- Scheduled Refresh Management
- Workspace & App Publishing
- Data Dictionary (Excel/Markdown format)
- Version Control using OneDrive/Git or internal naming standards

---

## 🧠 Key Learnings

- Learned how to **automate data updates** and minimize manual intervention
- Understood key **administration and maintenance** tasks in Power BI
- Established good habits in **version tracking**, **error monitoring**, and **report lifecycle management**
- Saw the impact of **usage analytics** in improving report design and relevance

---

## 🗓️ Course Timeline So Far

| Week | Focus Area                                           |
|------|------------------------------------------------------|
| 1    | Data Extraction, Cleaning, Initial Analysis          |
| 2    | Modeling, DAX, Core Reporting                        |
| 3    | Deployment, Navigation, RLS                         |
| 4    | Testing, Optimization, Final Edits                  |
| 5    | Power BI Service, Sharing, Collaboration            |
| 6    | Advanced DAX, Time Intelligence, Scenario Modeling  |
| 7    | Automation, Gateway Setup, Maintenance              |

---

## 📝 Conclusion

Week 7 equipped the project with the **backend reliability and automation** necessary for real-world use. With scheduled refreshes, centralized versioning, and usage monitoring in place, the Power BI solution is now ready to operate in a **live business environment** with minimal supervision.

