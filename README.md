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

#### 🔎 Observation

**Observation**

Total hospital billing reached approximately **£3M**, generated from around **4,973 patient visits** during the analysis period. However, although patient volume increased over time, the **average billing per visit (£674.86)** showed a slight downward trend.  

Revenue distribution across departments is also uneven. **Cardiology and Orthopedics contribute the largest share of total hospital billing**, while several other departments generate considerably lower revenue.

**Insight**

This suggests that hospital revenue growth is driven mainly by increasing patient volume rather than higher-value treatments.

Additionally, the strong revenue contribution from only a few departments indicates a **concentration of financial performance in specific specialties**. While this may reflect strong clinical demand in these areas, it also suggests that other departments may be **underutilized or not generating comparable revenue streams**.

**Recommendation**

Hospital management should track **revenue per visit** as a key financial performance indicator alongside total billing. At the same time, leadership should evaluate opportunities to **expand high-value services or procedures in underperforming departments**, helping to diversify revenue sources and reduce dependence on a small number of specialties.

---
### 🔍 Drill-down Analysis – Overview (Department-level)

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Drilldown.png)

**Observation**
Drilling down into department-level data shows that **Cardiology generates the highest total billing**, followed by Orthopedics and General Surgery.  

Within departments, revenue is often driven by a **limited number of diagnoses and procedures**, while many other services contribute relatively smaller shares of department revenue.

**Insight**

This pattern indicates that hospital revenue relies heavily on **specific specialties and procedures**. While these departments demonstrate strong demand, the hospital's financial performance may become **structurally dependent on a few key service lines**.

**Recommendation**

Hospital management should assess whether high-performing departments require **additional operational capacity**, while also identifying opportunities to improve utilization in **lower-performing departments** to build a more balanced revenue structure.

### 👨‍⚕️ Dashboard 2 – Doctors Performance Analysis

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Doctors.png)
#### 🔍 Doctor Performance & Workload Analysis

**Observation**

Doctor workload distribution is uneven across physicians.  
For example, **Dr. Olu Abiola handles a significantly higher number of patient visits compared with other doctors**.

Despite the higher patient volume, **Dr. Olu Abiola also maintains one of the highest patient satisfaction scores**, indicating that a higher workload does not necessarily reduce service quality.

**Insight**

This suggests that high patient volume alone does not lead to lower patient satisfaction.  
Instead, differences in **consultation efficiency, communication skills, and clinical workflow** may explain why some doctors can manage higher workloads while still maintaining strong patient experience.

**Recommendation**

Hospital management should:

- Analyze **best practices from high-performing doctors such as Dr. Olu Abiola**
- Identify consultation or workflow approaches that enable efficient patient handling
- Apply these practices across other physicians to **balance workload while maintaining service quality**


### 🧑‍🤝‍🧑 Dashboard 3 – Patient Profile & Behavior Analysis

**Observation**

Patient demand shows **noticeable seasonal patterns**, with certain months experiencing higher visit volumes than others.  

Demographic analysis also reveals that patient visits are **concentrated among middle-aged and older populations**, which aligns with typical healthcare demand patterns. Additionally, a few insurance providers account for a **significant portion of hospital billing coverage**.

**Insight**

Seasonal fluctuations in patient visits may be associated with **seasonal illnesses, routine health screenings, or ongoing management of chronic conditions**. Understanding these patterns is essential for anticipating demand and planning operational capacity.  

At the same time, reliance on a limited number of insurance providers suggests that hospital revenue may be **financially dependent on a small set of payer channels**, which could expose the organization to financial risk if reimbursement policies change.

**Recommendation**

Hospitals should use patient demand trends to improve **staffing and resource planning**, ensuring that staffing levels align with expected seasonal demand. Additionally, leadership should monitor the distribution of insurance providers to reduce potential financial exposure and maintain a balanced payer mix.

---

<a id="final-conclusion--recommendations"></a>
## 🔎 Final Conclusion & Recommendations  

### Key Findings

The analysis of hospital operations highlights three key operational patterns that influence both efficiency and financial performance.

1. **Revenue concentration across departments**  
Hospital revenue is largely driven by a small number of specialties, particularly **Cardiology and Orthopedics**, indicating strong demand in these areas but also a level of financial dependence on specific service lines.

2. **Uneven doctor workload distribution**  
Patient visits are not evenly distributed among physicians. Some doctors manage significantly higher patient volumes, suggesting opportunities to improve workload allocation and operational balance.

3. **Seasonal and demographic patterns in patient demand**  
Patient visits fluctuate over time and are concentrated among specific demographic groups, indicating that healthcare demand is influenced by recurring medical needs and population characteristics.

Overall, hospital performance is shaped not only by patient volume, but also by how effectively **resources, departments, and medical staff are distributed across the organization**.

### Strategic Recommendations

**1️⃣ Improve workload balance among doctors**

Hospitals should implement workload-balanced scheduling systems that distribute patient demand more evenly across physicians. This can help reduce physician burnout, shorten patient waiting times, and improve overall service capacity.

**2️⃣ Diversify revenue sources across departments**

To reduce financial dependency on a small number of specialties, hospital management should explore opportunities to expand high-value services in underperforming departments and improve utilization across different medical units.

**3️⃣ Monitor revenue per visit alongside patient volume**

Tracking revenue per visit can provide deeper insight into whether growth is driven by higher-value treatments or by lower-cost consultations. This metric can help hospital leadership evaluate the sustainability of revenue growth.

**4️⃣ Use patient demand patterns for operational planning**

Seasonal fluctuations in patient visits should be incorporated into workforce and capacity planning. Aligning staffing levels with expected demand can improve service efficiency and reduce operational pressure during peak periods.

**5️⃣ Maintain a balanced insurance payer mix**

Monitoring the distribution of insurance providers can help hospitals manage financial exposure and reduce potential risks related to reimbursement policy changes.
The framework can be easily extended to support forecasting, performance benchmarking, and continuous improvement initiatives across healthcare organizations.

## 📊 Project Impact

This dashboard helps hospital management:

• Identify revenue concentration across departments  
• Detect workload imbalance among physicians  
• Understand seasonal patient demand patterns  
• Support data-driven operational planning

## 📌 Final Summary

This project analyzes hospital operational performance through a set of Power BI dashboards that examine **revenue distribution, doctor workload, and patient demand patterns**.

The analysis shows that hospital revenue is primarily driven by a small number of departments, indicating a **concentration of financial performance in specific specialties**. While these departments generate strong demand, relying heavily on a limited set of service lines may expose the hospital to financial risk if patient demand shifts.

At the operational level, doctor workload is unevenly distributed. A few physicians manage a significantly higher number of patient visits than their peers. Although some high-volume doctors maintain strong patient satisfaction scores, persistent workload imbalance may lead to **operational pressure and potential burnout risks**.

From the patient perspective, demand fluctuates across time and demographic groups. Seasonal patterns and demographic concentration suggest that healthcare utilization is influenced by recurring medical needs, such as chronic condition management and routine health checkups.

Overall, the findings highlight the importance of **data-driven operational planning**. By balancing doctor workloads, diversifying revenue across departments, and aligning staffing capacity with patient demand patterns, hospital management can improve both **operational efficiency and long-term financial sustainability**.
