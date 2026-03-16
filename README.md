# 📊 Healthcare Operations Performance Analysis | Power BI
**Business Operations & Financial Insights | Healthcare Domain | Power BI**
**Author:** Tran Thuy Quynh  
**Date:** 2025-10 
**Tools Used:** Power BI  

## 📑 Table of Contents

1. 📌 [Background & Overview](#-background--overview)
2. 📂 [Dataset Description & Data Structure](#-dataset-description--data-structure)
3. 🧠 [Design Thinking Process](#-design-thinking-process)
4. 📊 [Key Insights & Visualizations](#-key-insights--visualizations)
5. 🔎 [Final Conclusion & Recommendations](#-final-conclusion--recommendations)
---
<a id="background-overview"></a>
## 📌 Background & Overview

### 🎯 Objective

### 📘 What is this project about?

This project analyzes **hospital operational and financial performance** using healthcare data and interactive Power BI dashboards.

The analysis examines how **patient demand, department services, doctor workload, and treatment costs** interact and how these factors influence hospital efficiency, revenue generation, and patient experience.

Through structured dashboards and drill-down analysis, the project helps hospital management identify operational bottlenecks, revenue concentration, and workload imbalances across departments and physicians.

The dashboard helps answer key operational questions such as:

- How does patient demand change over time?
- Which departments generate the highest billing revenue?
- Which doctors manage the largest patient workload?
- How do treatment and medication costs impact overall billing?
- How dependent is hospital revenue on specific departments or insurance providers?
- Are there signs of operational bottlenecks or workload imbalance?
- How does patient satisfaction vary across doctors and departments?
- Where should hospital resources be allocated to improve operational efficiency?

Overall, the analysis transforms raw hospital data into actionable insights that support **resource planning, cost control, workload balancing, and service optimization**.

---

### 👤 Who is this project for?

This project is designed for stakeholders who are responsible for managing hospital operations, performance, and strategy, including:

- ✅ Hospital directors and executive management  
- ✅ Operations and administrative managers  
- ✅ Department heads and medical coordinators  
- ✅ Healthcare analysts and business analysts  
- ✅ Decision-makers involved in budgeting, staffing, and capacity planning  

The insights help these stakeholders **understand what is happening, why it is happening, and what actions should be taken next** to improve both operational efficiency and patient outcomes.

---

<a id="dataset-description--data-structure"></a>
## 📂 Dataset Description & Data Structure  
## 📌 Data Source
- Simulated healthcare operational dataset  
- Format: CSV  
- Used for analytics and Power BI visualization  

---

## 📊 Tables Used in This Project  

| Table | Type | Description |
|------|------|-------------|
| visits | Fact | Patient visit–level transactional data |
| patients | Dimension | Patient demographics |
| providers | Dimension | Doctor information |
| departments | Dimension | Hospital departments |
| diagnoses | Dimension | Diagnosis categories |
| procedures | Dimension | Medical procedures |
| insurance | Dimension | Insurance providers |
| cities | Dimension | Geographic reference |

---

## 🧩 Table Schemas (Click to expand)

<details>
<summary><strong>📘 visits (Fact Table)</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| Visit_ID | INT | Unique visit identifier |
| Visit_Date | DATE | Date of visit |
| Patient_ID | INT | Foreign key → patients |
| Provider_ID | INT | Foreign key → providers |
| Department_ID | INT | Foreign key → departments |
| Diagnosis_ID | INT | Foreign key → diagnoses |
| Procedure_ID | INT | Foreign key → procedures |
| Insurance_ID | INT | Foreign key → insurance |
| Service_Type | TEXT | Emergency / Inpatient / Outpatient |
| Treatment_Cost | FLOAT | Cost of treatment |
| Medication_Cost | FLOAT | Cost of medication |
| Insurance_Coverage | FLOAT | Amount covered by insurance |
| Patient_Satisfaction | FLOAT | Satisfaction score |
| Emergency_Flag | BOOLEAN | Emergency indicator |
| Room_Charge | FLOAT | Room charge |
| Admission_Date | DATE | Admission date |
| Discharge_Date | DATE | Discharge date |
| Followup_Date | DATE | Follow-up date |
| Payment_Status | TEXT | Payment status |

</details>

<details>
<summary><strong>📘 patients</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| Patient_ID | INT | Unique patient identifier |
| Gender | TEXT | Gender |
| Age | INT | Age |
| Race | TEXT | Race |
| City_ID | INT | Foreign key → cities |
| Registration_Date | DATE | Registration date |

</details>

<details>
<summary><strong>📘 providers</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| Provider_ID | INT | Provider identifier |
| Provider_Name | TEXT | Doctor name |
| Gender | TEXT | Gender |
| Nationality | TEXT | Nationality |
| Age | INT | Age |
| Profile_Image | TEXT | Image reference |

</details>

<details>
<summary><strong>📘 departments</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| Department_ID | INT | Department identifier |
| Department_Name | TEXT | Department name |

</details>

<details>
<summary><strong>📘 diagnoses</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| Diagnosis_ID | INT | Diagnosis identifier |
| Diagnosis_Name | TEXT | Diagnosis name |

</details>

<details>
<summary><strong>📘 procedures</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| Procedure_ID | INT | Procedure identifier |
| Procedure_Name | TEXT | Procedure name |

</details>

<details>
<summary><strong>📘 insurance</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| Insurance_ID | INT | Insurance identifier |
| Insurance_Provider | TEXT | Insurance provider name |

</details>

<details>
<summary><strong>📘 cities</strong></summary>

| Column | Data Type | Description |
|------|-----------|-------------|
| City_ID | INT | City identifier |
| City | TEXT | City name |
| State | TEXT | State name |

</details>

---

## 🔗 Data Relationships

<img width="557" height="588" alt="image" src="https://github.com/user-attachments/assets/3198cc48-cf3c-402b-a73e-c6f14f7b2710" />


📌 The model follows a **star schema**, optimized for filtering, aggregation, and drill-down analysis in Power BI.

---

<a id="design-thinking-process"></a>
## 🧠 Design Thinking Process  

This project follows a structured **Design Thinking framework** to ensure that insights are not only data-driven but also aligned with real business needs in a healthcare environment.

The goal is to move step by step from understanding stakeholder problems → defining the right metrics → designing meaningful analytical views → delivering actionable insights.
<img width="1198" height="653" alt="image" src="https://github.com/user-attachments/assets/cc6c33a6-3d62-449c-80d0-2c8dfe007662" />
<img width="1146" height="567" alt="image" src="https://github.com/user-attachments/assets/ca0745e0-d713-456b-9fa0-1d778b21dacf" />
<img width="1098" height="329" alt="image" src="https://github.com/user-attachments/assets/a24d3e6f-778b-479b-a66c-1f22ef02c138" />
<img width="1138" height="637" alt="image" src="https://github.com/user-attachments/assets/14a83164-9470-42f2-a3d4-8b00f86ffae6" />
<img width="1187" height="670" alt="image" src="https://github.com/user-attachments/assets/501e9e51-a077-41a0-ae7d-2991ccd88e73" />
<img width="1139" height="622" alt="image" src="https://github.com/user-attachments/assets/125d158b-67e4-4348-9001-818d2e117e1f" />
<img width="1184" height="654" alt="image" src="https://github.com/user-attachments/assets/0327c637-9713-4d8e-9468-98e95803782c" />

<a id="key-insights--visualizations"></a>
## 📊 Key Insights & Visualizations

### 🔍 Dashboard Preview

#### 1️⃣ Dashboard 1 – Hospital Overview (Executive View)

<img width="1134" height="751" alt="image" src="https://github.com/user-attachments/assets/b0dfdc57-6137-4442-be7d-15ee89816dd7" />

### 📌 Analysis 1

### Observation

Total hospital billing reached approximately **£3M**, generated from **4,973 patient visits** during the analysis period.

While patient volume increased over time, the **average billing per visit (£674.86)** shows a slight declining trend.

Revenue distribution across departments is also uneven. **Cardiology and Orthopedics contribute the largest share of total hospital revenue**, while other departments generate significantly smaller contributions.

In addition, **treatment costs account for the largest share of operational expenses**, significantly higher than medication and room-related charges.

### Interpretation

Revenue growth appears to be driven primarily by **increasing patient volume rather than higher-value medical procedures**.

This suggests that hospital revenue growth may currently rely more on routine consultations or lower-cost services rather than complex procedures that typically generate higher revenue per visit.

The concentration of revenue in a limited number of departments also indicates a **potential structural dependency on specific medical specialties**.

### Business Impact

If patient growth continues to be driven mainly by lower-value visits, the hospital may face limitations in revenue growth despite increasing operational workload.

Heavy reliance on a small number of departments could also introduce financial risk if demand in those specialties declines.

### Recommendations

- Expand high-value medical procedures where appropriate.
- Ensure sufficient staffing and resources for high-demand departments such as Cardiology and Orthopedics.
- Monitor department-level profitability to identify opportunities for service expansion.
---
### 🔍 Drill-down Analysis – Overview (Department-level)

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Drilldown.png)

To better understand the drivers of hospital performance, the dashboard enables a drill-down view that analyzes operational metrics at the **department level**.

#### Observation

Department-level analysis shows clear differences in both **revenue contribution and patient volume** across hospital specialties.

Cardiology and Orthopedics stand out as the **two highest revenue-generating departments**, driven by a combination of higher patient demand and higher-value medical procedures.

In contrast, several other departments contribute a relatively smaller share of hospital billing despite maintaining steady patient visits.

#### Interpretation

This pattern suggests that hospital revenue is **not evenly distributed across departments**. Instead, financial performance is concentrated in specialties that typically involve more complex procedures and specialized treatments.

Departments with lower revenue contribution may focus on routine consultations or services with lower billing values.

#### Business Impact

A revenue structure that relies heavily on a small number of departments can introduce **operational and financial concentration risk**. Any disruption in demand or staffing within these key specialties could significantly impact overall hospital performance.

At the same time, departments with lower revenue contribution may represent **opportunities for service expansion or operational optimization**.

#### Recommendation

- Ensure sufficient staffing and medical resources in high-demand departments such as **Cardiology and Orthopedics**.
- Evaluate opportunities to expand high-value procedures in other departments.
- Monitor department-level performance regularly to maintain balanced operational growth.
\
### 👨‍⚕️ Dashboard 2 – Doctors Performance Analysis

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Doctors.png)
#### 🔍 Doctor Performance & Workload Analysis

### Observation

Doctor-level performance analysis reveals noticeable differences in patient workload across physicians.

Some doctors handle significantly higher patient volumes than others. For example, **Dr. Olu Abiola records one of the highest patient counts**, indicating a strong contribution to overall hospital service capacity.

At the same time, other physicians appear to have comparatively lower patient loads.

### Interpretation

The imbalance in patient distribution may indicate differences in physician specialization, scheduling efficiency, or patient preference.

High patient volumes handled by specific doctors may reflect strong reputation or operational efficiency, but sustained workload concentration could also increase the risk of **physician burnout**.

### Business Impact

Uneven workload distribution can create operational inefficiencies. Over-utilized doctors may experience fatigue, while under-utilized physicians represent unused capacity.

Balanced patient allocation could improve operational efficiency and maintain service quality across the hospital.

### Recommendations

- Review appointment scheduling processes to distribute patient visits more evenly.
- Support high-performing physicians with additional operational resources where necessary.
- Monitor physician workload to reduce burnout risk.

---

### 🧑‍🤝‍🧑 Dashboard 3 – Patient Profile & Behavior Analysis

### Observation

Patient demand shows variations across demographic groups and insurance providers.

Certain age groups represent a larger share of hospital visits, suggesting that healthcare demand may be concentrated among specific patient segments.

Insurance provider distribution also shows concentration among several major providers.

### Interpretation

Understanding demographic demand patterns can help hospitals better align services with patient needs.

Insurance coverage distribution may also influence hospital revenue streams, as reimbursement rates and payment structures vary between providers.

### Business Impact

If patient demand is concentrated within specific demographic segments or insurance providers, the hospital may become financially dependent on a limited set of patient groups.

Understanding these patterns is important for long-term revenue stability and service planning.

### Recommendations

- Monitor demographic demand patterns to support service planning.
- Evaluate partnerships with major insurance providers.
- Develop targeted healthcare programs for high-demand patient groups.
---

<a id="final-conclusion--recommendations"></a>
## 🔎 Final Conclusion & Recommendations  

### Key Findings

The analysis of hospital operations highlights three key operational patterns that influence both efficiency and financial performance.

1️⃣ **Revenue concentration across departments**

Hospital revenue is largely driven by a small number of specialties, particularly **Cardiology and Orthopedics**, indicating strong demand in these areas but also a level of financial dependence on specific service lines.

2️⃣ **Uneven doctor workload distribution**

Patient visits are not evenly distributed among physicians. Some doctors manage significantly higher patient volumes, suggesting opportunities to improve workload allocation and operational balance.

3️⃣ **Seasonal and demographic patterns in patient demand**

Patient visits fluctuate over time and are concentrated among specific demographic groups, indicating that healthcare demand is influenced by recurring medical needs and population characteristics.

### Strategic Recommendations

Based on the analysis, several strategic actions could improve hospital operations:

- Improve operational efficiency by balancing physician workloads.
- Expand high-value medical services to improve revenue sustainability.
- Strengthen capacity planning for high-demand departments.
- Monitor demographic demand patterns to support long-term healthcare planning.

# Project Impact

This dashboard demonstrates how healthcare operational data can be transformed into actionable insights for hospital management.

By integrating financial performance, physician productivity, and patient demand analysis, hospital administrators can better understand operational challenges and identify opportunities to improve both **healthcare quality and financial sustainability**.
