# Hospitality Revenue Intelligence Platform  
## End-to-End Data Analytics & Business Intelligence Project (Power BI)

---

## 🚀 Project Summary
This project delivers a **production-style Hospitality Revenue Intelligence platform** that mirrors how data analytics is applied in real hotel operations.  
It converts raw booking and capacity data into **business-ready KPIs and insights**, enabling hotel management to optimize pricing, occupancy, and channel strategy.

Designed with **analytics + data engineering best practices**, this project demonstrates strong alignment with **industry workflows, stakeholder-driven design, and scalable data modeling**.

---

## 🎯 Business Objective
Hotels operate in a highly demand-sensitive environment where revenue performance depends on:
- Demand seasonality  
- Booking and cancellation behavior  
- Room capacity utilization  
- Channel-wise sales effectiveness  

The objective of this project is to **build a centralized analytics system** that:
- Standardizes revenue KPIs  
- Identifies revenue leakages  
- Enables multi-level drill-down analysis  
- Supports data-driven pricing and operational decisions  

---

## 🏗️ Data Architecture
The project follows a **Star Schema data model**, ensuring scalability, performance, and analytical flexibility.

### Dimension Tables
- **dim_hotels** – Hotel metadata (property, city, category, ratings)  
- **dim_rooms** – Room types, categories, and capacity  
- **dim_date** – Calendar table with weekday/weekend and week number logic  

### Fact Tables
- **fact_bookings** – Booking-level transactional data (revenue, status, channel)  
- **fact_aggregated_bookings** – Capacity vs successful booking aggregates  

### Reference Tables
- **meta_data_hospitality** – Domain rules and business mappings  
- **metrics_list** – Centralized KPI definitions for consistency  

---

## 📊 Core KPIs & Metrics Engine
All metrics are built using **validated DAX measures** to ensure accuracy and consistency.

- **Occupancy %**  
- **ADR (Average Daily Rate)**  
- **RevPAR (Revenue per Available Room)**  
- **SRN / DSRN (Sellable Room Nights)**  
- **Realization %**  
- **Week-on-Week & Month-on-Month Trends**  

Each KPI is designed to support **diagnostic, not just descriptive, analysis**.

---

## 🔄 Analytics Workflow
1. **Business Requirement Analysis**  
   - Revenue-focused KPIs defined with domain context  

2. **Data Cleaning & Transformation**  
   - Power Query used for standardization and enrichment  

3. **Data Modeling**  
   - Star Schema with optimized relationships  

4. **KPI Engineering**  
   - DAX measures with validation against raw data  

5. **Dashboard Development**  
   - Interactive visuals with drill-down and tooltips  

6. **Stakeholder Feedback Loop**  
   - Iterative enhancements based on business review  

---

## 📈 Dashboard Capabilities
- Executive KPI overview  
- Multi-level drill-down:
  - City → Property → Room Type → Channel  
- Weekday vs Weekend performance comparison  
- WoW & MoM trend indicators  
- Conditional formatting for quick issue detection  

---

## 💡 Business Insights Generated
- Revealed absence of dynamic pricing despite demand variability  
- Identified underperforming hotels driven by cancellations and low ratings  
- Highlighted channel-level revenue inefficiencies  
- Demonstrated correlation between customer ratings and occupancy  

---

## 🧠 Skills Demonstrated
- Data Analytics & BI Development  
- Data Modeling (Star Schema)  
- DAX & KPI Engineering  
- Business & Revenue Analytics  
- Stakeholder Communication  
- Analytical Problem Solving  

---

## 🛠️ Tools & Technologies
- **Power BI**  
- **Power Query**  
- **DAX**  
- **SQL (conceptual & modeling)**  

---

## 📂 Repository Structure
```text
├── Dataset/
│   ├── dim_hotels.csv
│   ├── dim_rooms.csv
│   ├── dim_date.csv
│   ├── fact_bookings.csv
│   ├── fact_aggregated_bookings.csv
│   ├── meta_data_hospitality.csv
│   └── metrics_list.csv
├── PowerBI_Dashboard/
│   └── Hospitality_Revenue_Dashboard.pbix
├── Screenshots/
│   └── dashboard_views.png
└── README.md
