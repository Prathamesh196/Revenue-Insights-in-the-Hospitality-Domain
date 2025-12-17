# Hospitality Insight in the Hospitality Domain  
## End-to-End Data Analytics & Business Intelligence (Power BI • Power Query • DAX)

---

## 🚀 Project Summary
**Hospitality Insight in the Hospitality Domain** is a production-style analytics project that transforms raw hotel booking and capacity data into **actionable revenue insights**. Built using **Power BI, Power Query, and DAX**, the solution enables data-driven decisions around pricing, occupancy, and channel performance.

---

## 🎯 Business Objective
Enable hotel stakeholders to:
- Track standardized revenue KPIs
- Identify revenue leakages caused by cancellations and no-shows
- Compare weekday vs weekend performance
- Drill down across city, property, room type, and booking channel

---

## 🏗️ Data Architecture (Star Schema)

### Dimension Tables
- **dim_hotels** – Property details including city, category, and ratings  
- **dim_rooms** – Room types, categories, and capacity  
- **dim_date** – Calendar table with week number and weekday/weekend logic  

### Fact Tables
- **fact_bookings** – Booking-level transactional data (revenue, status, channel)  
- **fact_aggregated_bookings** – Aggregated capacity vs successful bookings  

### Reference Tables
- **meta_data_hospitality** – Business rules and domain mappings  
- **metrics_list** – Centralized KPI definitions  

---

## 📊 KPI & Metrics Engine (DAX)
All metrics are built and validated using **DAX**.

- **Occupancy %** = Successful Bookings / Total Capacity  
- **ADR (Average Daily Rate)** = Revenue from Sold Rooms / Rooms Sold  
- **RevPAR (Revenue per Available Room)** = Total Revenue / Available Rooms  
- **SRN / DSRN (Sellable Room Nights)** = Rooms available for sale per day  
- **DURN (Utilized Room Nights)** = Actual room nights stayed (post check-in)  
- **Realization %** = DURN / Booked Room Nights  
- **WoW & MoM Change %** using DAX time intelligence  

---

## 🔄 Analytics Workflow
1. Business requirement analysis with revenue context  
2. Data cleaning and transformation using Power Query  
3. Star schema data modeling  
4. DAX measure development and validation  
5. Interactive dashboard development  
6. Stakeholder feedback and iterative refinement  

---

## 📈 Dashboard Capabilities
- Executive KPI overview  
- Drill-down analysis: City → Property → Room Type → Channel  
- Weekday vs weekend revenue comparison  
- WoW & MoM trend indicators  
- Conditional formatting for performance monitoring  

---

## 💡 Business Insights
- Identified flat pricing despite demand variability  
- Revenue loss quantified through cancellations and no-shows using **DURN**  
- Underperforming hotels linked to lower customer ratings  
- Channel-level revenue inefficiencies highlighted  

---

## 🧠 Skills Demonstrated
- Power BI Dashboard Development  
- **DAX (KPI & Time Intelligence, including DURN)**  
- Power Query (ETL & Data Preparation)  
- Star Schema Data Modeling  
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
│   └── Hospitality_Insight_Dashboard.pbix
├── Screenshots/
│   └── dashboard_views.png
└── README.md
