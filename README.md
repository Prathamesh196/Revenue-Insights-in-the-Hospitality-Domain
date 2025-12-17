# Hospitality Revenue Intelligence Platform  
## End-to-End Data Analytics & Business Intelligence (Power BI • Power Query • DAX)

---

## 🚀 Project Summary
A **production-style Hospitality Revenue Intelligence platform** that transforms raw hotel booking data into **actionable revenue insights**. Built with **Power BI, Power Query, and DAX**, the solution enables data-driven pricing, capacity utilization, and channel optimization.

---

## 🎯 Business Objective
Enable hotel leadership to:
- Standardize revenue KPIs
- Detect revenue leakages (cancellations, no-shows)
- Analyze weekday vs weekend performance
- Drill down by city, property, room type, and channel

---

## 🏗️ Data Architecture (Star Schema)

### Dimension Tables
- **dim_hotels** – Property, city, category, ratings  
- **dim_rooms** – Room types, categories, capacity  
- **dim_date** – Calendar with week number and weekday/weekend logic  

### Fact Tables
- **fact_bookings** – Booking-level transactions (revenue, status, channel)  
- **fact_aggregated_bookings** – Capacity vs successful bookings  

### Reference Tables
- **meta_data_hospitality** – Business rules & mappings  
- **metrics_list** – Centralized KPI definitions  

---

## 📊 KPI & Metrics Engine (DAX)
All metrics are built and validated using **DAX**.

- **Occupancy %** = Successful Bookings / Total Capacity  
- **ADR (Average Daily Rate)** = Revenue from Sold Rooms / Rooms Sold  
- **RevPAR (Revenue per Available Room)** = Total Revenue / Available Rooms  
- **SRN / DSRN (Sellable Room Nights)** = Rooms available for sale per day  
- **DURN (Utilized Room Nights)** = Actual room nights stayed (post check-in)  
- **Realization %** = **DURN / Booked Room Nights**  
- **WoW & MoM Change %** (Time Intelligence)

> **Note:** DURN is used to accurately capture realized stays after cancellations and no-shows, improving revenue realism.

---

## 🔄 Analytics Workflow
1. Requirement analysis with revenue context  
2. Data cleaning & enrichment (Power Query)  
3. Star schema modeling  
4. DAX KPI development & validation  
5. Interactive dashboard build  
6. Stakeholder feedback & iteration  

---

## 📈 Dashboard Capabilities
- Executive KPI snapshot  
- Drill-down: City → Property → Room Type → Channel  
- Weekday vs Weekend comparison  
- WoW & MoM trends (DAX)  
- Conditional formatting for performance monitoring  

---

## 💡 Business Insights
- Flat pricing despite demand variability  
- Revenue loss driven by cancellations/no-shows (captured via **DURN**)  
- Underperforming properties linked to low ratings  
- Channel-level inefficiencies identified  

---

## 🧠 Skills Demonstrated
- Power BI Dashboarding  
- **DAX (KPI & Time Intelligence, incl. DURN)**  
- Power Query (ETL)  
- Star Schema Modeling  
- Business & Revenue Analytics  

---

## 🛠️ Tools & Technologies
- Power BI  
- Power Query  
- **DAX**  
- SQL (conceptual modeling)

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
