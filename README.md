# Revenue Insights in the Hospitality Domain  
## End-to-End Data Analytics & Business Intelligence (Power BI • Power Query • DAX)

---

## 🚀 Project Summary
**Revenue Insights in the Hospitality Domain** is an end-to-end analytics project that converts raw hotel booking and capacity data into **actionable revenue intelligence**. Built using **Power BI, Power Query, and DAX**, the project mirrors real-world hotel revenue management workflows and supports data-driven pricing and operational decisions.

---

## 🎯 Business Objective
Provide hotel stakeholders with a centralized analytics system to:
- Monitor standardized revenue KPIs
- Detect revenue leakages caused by cancellations and no-shows
- Compare weekday vs weekend performance
- Perform multi-level analysis by city, property, room type, and booking channel

---

## 🏗️ Data Architecture (Star Schema)

### Dimension Tables
- **dim_hotels** – Hotel metadata including city, category, and ratings  
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
All KPIs are developed and validated using **DAX**.

- **Occupancy %** = Successful Bookings / Total Capacity  
- **ADR (Average Daily Rate)** = Revenue from Sold Rooms / Rooms Sold  
- **RevPAR (Revenue per Available Room)** = Total Revenue / Available Rooms  
- **SRN / DSRN (Sellable Room Nights)** = Rooms available for sale per day  
- **DURN (Utilized Room Nights)** = Actual room nights stayed after check-in  
- **Realization %** = DURN / Booked Room Nights  
- **WoW & MoM Change %** using time-intelligence functions  

---

## 🔄 Analytics Workflow
1. Business requirement analysis with revenue context  
2. Data cleaning and transformation using Power Query  
3. Star schema data modeling  
4. DAX measure creation and validation  
5. Interactive dashboard development  
6. Stakeholder feedback and iterative improvements  

---

## 📈 Dashboard Capabilities
- Executive KPI overview  
- Drill-down analysis: City → Property → Room Type → Channel  
- Weekday vs weekend revenue comparison  
- WoW & MoM trend indicators  
- Conditional formatting to highlight performance gaps  

---

## 💡 Business Insights
- Identified flat pricing strategies despite fluctuating demand  
- Quantified revenue loss due to cancellations and no-shows using **DURN**  
- Highlighted underperforming hotels linked to low customer ratings  
- Revealed channel-level revenue inefficiencies  

---

## 🧠 Skills Demonstrated
- Power BI Dashboard Development  
- **DAX (KPI Modeling & Time Intelligence, including DURN)**  
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
│   └── Revenue_Insights_Hospitality.pbix
├── Screenshots/
│   └── dashboard_views.png
└── README.md
