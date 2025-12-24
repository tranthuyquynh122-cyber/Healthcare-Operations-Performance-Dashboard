# 🏥 Healthcare Operations Performance Dashboard

## 📌 Project Description
This project analyzes **healthcare operational data** using Power BI to evaluate hospital performance from both **financial** and **patient volume** perspectives.  
The dashboard is designed to support hospital management in monitoring key metrics, identifying trends, and making data-driven operational decisions.

The solution is built on a **star schema data model**, ensuring scalable analysis and efficient reporting.

---

## 📋 Table of Contents
- Project Description  
- Business Context  
- Data Model  
- Key Metrics & Analysis  
- Dashboard Screenshots  
- Tools & Technologies  
- Dashboard Output  
- Project Structure  
- Contact  

---

## 🧠 Business Context
Hospitals generate large volumes of operational data related to:
- Patient visits and admissions  
- Medical procedures and diagnoses  
- Providers, departments, and insurance coverage  
- Treatment, medication, and room charges  

Without proper analytics, it is difficult to understand:
- Patient demand trends  
- Revenue performance in relation to patient volume  
- Which departments, diagnoses, or services drive cost and billing  

This project transforms raw healthcare data into **clear, actionable insights** through an interactive Power BI dashboard.

---

## 🗂️ Data Model (Star Schema)
The dashboard is built using a **star schema** optimized for analytical reporting.

### ⭐ Fact Table
**Fact_visits**
- Admission & discharge dates  
- Length of stay  
- Emergency & follow-up visit indicators  
- Treatment cost, medication cost, room charges  
- Patient satisfaction score  
- Foreign keys to dimension tables  

### 📐 Dimension Tables
- **Dim_patients** – age, gender, age group, city  
- **Dim_departments** – hospital departments  
- **Dim_providers** – healthcare providers  
- **Dim_diagnoses** – diagnosis information  
- **Dim_procedures** – medical procedures  
- **Dim_insurance** – insurance providers & coverage  
- **Dim_cities** – geographic dimension  
- **Date** – calendar dimension for time-based analysis  

---

## 📊 Key Metrics & Analysis

### ⭐ Key Metrics
- **Total Billing Amount**  
  Total revenue generated from patient services, including treatment cost, medication cost, and room charges.

- **Total Patients**  
  Total number of unique patients served in a selected time period.

### 🔍 Supporting Analysis
- Billing trends over time  
- Patient volume trends  
- Revenue vs patient growth comparison  
- Breakdown by department, provider, diagnosis, and insurance  
- Identification of high-revenue services and patient segments  

---

## 🖥️ Dashboard Screenshots

### 🔹 Overview – Financial & Operational Performance
Provides a high-level view of **Total Billing Amount**, **Total Patients**, cost breakdowns, and department-level revenue contribution.

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/4295f02c089a4a1e1ddeae38972c53b1022a1e81/Screenshot%202025-12-24%20232813.png)

---

### 🔹 Doctors – Provider Performance Analysis
Analyzes doctor performance, including:
- Patients handled per doctor  
- Average patient satisfaction score  
- Procedures performed  
- Average treatment cost
- 
![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/e4215c9950d5889ae9e7ff69ca2ea4487f25c2d5/Screenshot%202025-12-24%20232152.png)

---

### 🔹 Patients – Demographics & Visit Behavior
Explores patient characteristics and behavior, including:
- Patient volume over time  
- Emergency vs non-emergency visits  
- Age group, gender, race distribution  
- Insurance coverage distribution  

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/e273b17bb311550d58fe87e8715602e0e0c14445/Screenshot%202025-12-24%20232200.png)

---

## 🛠️ Tools & Technologies
- **Power BI** – data modeling and dashboard development  
- **DAX** – KPI and calculated measures  
- **Excel / CSV** – data preprocessing and validation  
- **Healthcare domain knowledge** – KPI interpretation and operational context  

---
## 🔍 Final Conclusion & Recommendations

👉 Based on the insights and findings from the Healthcare Operations Performance Dashboard, the following key conclusions and recommendations are proposed for hospital management and operations teams.

### 📌 Key Takeaways
- Patient volume is concentrated in specific age groups, while patient satisfaction varies significantly across departments, indicating uneven service quality.
- High patient load handled by a small number of doctors is associated with lower satisfaction scores, suggesting potential workload imbalance.
- Hospital revenue is highly dependent on insurance coverage and a limited number of high-performing departments and services, increasing financial risk.

### 📌 Recommendations
- **Enhance Patient Experience:**  
  Implement post-visit satisfaction surveys to identify root causes of dissatisfaction and improve service quality across departments.

- **Optimize Doctor Workload & Performance:**  
  Rebalance doctor scheduling to reduce overload and establish KPIs that balance patient volume with satisfaction scores.

- **Reduce Revenue Concentration Risk:**  
  Monitor insurance-related billing closely and promote underutilized services to diversify revenue streams and stabilize financial performance.




