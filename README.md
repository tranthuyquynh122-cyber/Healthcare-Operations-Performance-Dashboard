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

### 📖 What is this project about?

Hospitals generate large volumes of operational and financial data, but turning this data into actionable insights for decision-making remains a challenge.

This project analyzes hospital performance using healthcare data and interactive Power BI dashboards, focusing on how **patient demand, department performance, doctor workload, and treatment costs** impact operational efficiency and revenue.

The analysis aims to identify:
- Revenue concentration across departments  
- Workload imbalances across doctors  
- Demand patterns across patient segments  

These insights support data-driven decisions in **resource allocation, cost optimization, and operational efficiency improvement**.

---

### 👥 Who is this project for?

This project is designed for stakeholders responsible for hospital performance and operational decision-making, including:

- Hospital executives and directors  
- Operations and administrative managers  
- Department heads and medical coordinators  
- Healthcare and business analysts  

The insights enable stakeholders to understand **what is happening, why it is happening, and what actions should be taken** to improve both operational efficiency and patient outcomes.

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

### 📊 Analysis 1 – Hospital Revenue & Operational Performance

#### 🔎 Observation

Total hospital billing reached approximately **£3M**, generated from **4,973 patient visits**.

However, while patient volume increased over time, the **average billing per visit declined to £674.86**, indicating a gap between volume growth and value.

Cost structure is heavily dominated by **treatment costs (£2.63M)**, significantly exceeding medication (£546K) and other cost components.

Revenue is also highly concentrated, with **Cardiology and Orthopedics contributing a disproportionately large share of total billing**, while other departments generate significantly lower revenue.

---

#### 💡 Interpretation

Revenue growth is primarily driven by **higher patient volume rather than higher-value treatments**.

The declining revenue per visit suggests that growth is coming from **lower-value services**, rather than complex procedures.

The concentration of revenue in a few departments indicates a **structural dependency on specific service lines**.

---

#### 📉 Business Impact

If this trend continues, the hospital may experience **increasing workload without proportional revenue growth**, reducing operational efficiency.

Revenue concentration also creates **financial risk**, as performance becomes dependent on a limited number of departments.

---

#### 🎯 Recommendations

- Expand **high-value procedures** within Cardiology and Orthopedics to increase revenue per visit.
- Optimize **service mix and pricing strategy** to reduce reliance on low-margin services.
- Track **revenue per visit** as a key KPI alongside total revenue.
### 🔍 Drill-down Analysis – Overview (Department-level)

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Drilldown.png)

### 🔎 Drill-down Analysis – Department Level

#### 🔎 Observation

Department-level analysis shows significant variation in both revenue contribution and patient volume.

**Cardiology and Orthopedics generate the highest billing**, supported by both high patient demand and higher-value procedures.

In contrast, several departments maintain relatively stable patient volumes but contribute **significantly lower billing**, indicating lower revenue per visit.

---

#### 💡 Interpretation

This pattern suggests that hospital revenue is **not evenly distributed**, but instead concentrated in departments offering more complex and higher-priced services.

Departments with lower billing contribution are likely focused on **routine consultations or lower-cost treatments**.

---

#### 📉 Business Impact

A revenue structure concentrated in a few departments increases **operational and financial concentration risk**.

At the same time, underperforming departments represent opportunities to **optimize service mix or introduce higher-value procedures**.

---

#### 🎯 Recommendations

- Ensure sufficient **staffing, equipment, and capacity** in high-demand departments such as Cardiology and Orthopedics.
- Evaluate opportunities to **introduce higher-value services** in lower-performing departments.
- Track **revenue per patient by department** to identify efficiency gaps.


### 👨‍⚕️ Dashboard 2 – Doctors Performance Analysis

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Doctors.png)

#### 🔍 Doctor Performance & Workload Analysis

#### 🔎 Observation

Patient workload is highly uneven across physicians.

Out of 5 doctors, **the top 2 doctors (Dr. Sade Kikola and Dr. Olu Abiola) handle approximately 65% of total patient visits**, with **1,875 (37.7%) and 1,357 (27.3%) patients respectively**.

In contrast, the remaining 3 doctors each manage less than 20% of total visits, with some handling below 10%.

This indicates a **highly concentrated workload distribution**.

---

#### 💡 Interpretation

The patient distribution follows a **Pareto-like pattern**, where a small number of doctors account for the majority of workload.

This imbalance may be driven by differences in **doctor specialization, availability, scheduling efficiency, or patient preference**.

It also suggests that hospital capacity is **not evenly utilized across physicians**.

---

#### 📉 Business Impact

Over-reliance on a small group of doctors creates a risk of **physician fatigue and burnout**, especially for top performers handling a disproportionately high workload.

At the same time, underutilized doctors represent **unused operational capacity**, leading to inefficiencies in resource allocation.

If not addressed, this imbalance may impact both **service quality and operational scalability**.

---

#### 🎯 Recommendations

- Redistribute patient demand by optimizing **appointment scheduling and doctor assignment logic**.
- Reduce dependency on top-performing doctors by **balancing workload across available physicians**.
- Monitor **patient share per doctor (%)** as a key KPI to maintain sustainable workload distribution.
---

### 🧑‍🤝‍🧑 Dashboard 3 – Patient Profile & Behavior Analysis

#### 🔎 Observation

The hospital serves a total of **4,973 patients**, with demand concentrated in specific demographic segments.

Patients aged **55+ account for the largest share (~38.8%)**, followed by the **18–35 group (~28%)**, while other age groups each contribute around 16%.

Insurance coverage is highly concentrated, with **three providers (AXA, Aviva, Allianz) collectively covering nearly 100% of patients**, each contributing approximately one-third.

In addition, **emergency visits account for ~24.7% of total visits**, and **follow-up visits represent 50%**, indicating a significant proportion of recurring patient demand.



#### 💡 Interpretation

Patient demand is **not evenly distributed**, but concentrated in older age groups and a limited number of insurance providers.

The high share of patients aged 55+ suggests that hospital services are heavily utilized by **aging populations with higher healthcare needs**.

The high follow-up rate (50%) indicates **strong patient retention or ongoing treatment cycles**, rather than one-time visits.



#### 📉 Business Impact

Dependence on a specific demographic group (55+) and a limited number of insurance providers creates **concentration risk**, making revenue vulnerable to demographic shifts or policy changes.

At the same time, the high follow-up rate suggests an opportunity to **increase patient lifetime value**, but also implies sustained operational demand.



#### 🎯 Recommendations

- Develop targeted healthcare programs for **older patient segments (55+)**, where demand is highest.
- Strengthen strategic partnerships with **key insurance providers (AXA, Aviva, Allianz)** while exploring diversification opportunities.
- Leverage the high follow-up rate to implement **long-term care programs and patient retention strategies**.
- Monitor **emergency visit trends (~25%)** to optimize resource allocation and capacity planning.
  
---

<a id="final-conclusion--recommendations"></a>
## 🔎 Final Conclusion & Recommendations  

### 📌 Key Findings

The analysis highlights three structural patterns impacting hospital performance:

1. **Revenue concentration across departments**  
Hospital revenue is heavily concentrated in a small number of specialties, particularly **Cardiology and Orthopedics**, which contribute the largest share of total billing. This indicates strong demand but also a dependency on a limited set of service lines.

2. **Uneven doctor workload distribution**  
Out of 5 doctors, **the top 2 account for approximately 65% of total patient visits**, indicating a highly imbalanced workload distribution and suboptimal utilization of available medical capacity.

3. **Concentrated patient demand patterns**  
Patient demand is primarily driven by **older age groups (55+ ~38.8%)** and a small number of insurance providers (**AXA, Aviva, Allianz ~100% combined coverage**), suggesting limited diversification in the patient base.


### 🎯 Strategic Recommendations

Based on the identified workload imbalance and demand concentration patterns, the following targeted actions are recommended:

- **Rebalance physician workloads**, as the top 2 doctors currently handle ~65% of total patient visits, by optimizing scheduling and redistributing patient demand.

- **Expand high-value medical services** in key departments (Cardiology, Orthopedics) to improve revenue per visit and reduce reliance on volume-driven growth.

- **Strengthen capacity planning** in high-demand areas, particularly for patient segments aged 55+ (~38.8%), where healthcare utilization is highest.

- **Leverage the high follow-up rate (50%)** to develop structured long-term care programs and improve patient lifetime value.

- **Reduce concentration risk** by diversifying patient segments and exploring additional insurance partnerships beyond the current core providers.


### 🚀 Project Impact

This analysis shows that hospital performance is currently constrained by workload imbalance and revenue concentration.

By addressing these issues, the hospital can improve resource utilization, reduce operational inefficiencies, and support more sustainable, value-driven healthcare delivery.
