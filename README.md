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

This project focuses on analyzing **hospital operational and financial performance** using healthcare data and Power BI dashboards.  
The goal is to help hospital management better understand how patient volume, medical services, doctors, and costs interact — and how these factors impact overall efficiency, revenue, and patient experience.

The dashboard translates complex hospital data into clear, actionable insights that support data-driven decision-making at both operational and strategic levels.

This project helps answer real-world business questions such as:

- How many patients are being served over time, and how does demand fluctuate?
- Which departments generate the highest billing and handle the most patients?
- Which doctors manage the highest workload, and how balanced is doctor performance?
- Are treatment costs and medication costs under control?
- How dependent is revenue on specific departments or insurance providers?
- Are there signs of operational bottlenecks or workload imbalance?
- How does patient satisfaction vary across doctors and departments?
- Where should resources be reallocated to improve efficiency and patient experience?

The analysis transforms raw hospital data into structured insights that support **better planning, cost control, workload balancing, and service optimization**.

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

<details>
<summary><strong>Dashboard 1 – Overview</strong></summary>

**Observations**
- A small number of departments generate most billing  
- Billing fluctuates over time  
- Insurance covers a significant share of costs  

**Recommendations**
- Monitor high-cost departments  
- Reduce dependency on limited services  
- Use trends for financial planning  

</details>

<details>
<summary><strong>Dashboard 2 – Doctors</strong></summary>

**Observations**
- Doctor workload is uneven  
- Some doctors handle disproportionately high patient volumes  
- High workload does not always imply high satisfaction  

**Recommendations**
- Balance workload  
- Improve scheduling  
- Track satisfaction together with productivity  

</details>

<details>
<summary><strong>Dashboard 3 – Patients</strong></summary>

**Observations**
- Patient volume varies by month  
- Middle-aged and elderly groups dominate  
- Emergency visits represent a significant share  

**Recommendations**
- Prepare resources for peak periods  
- Monitor emergency usage  
- Improve follow-up strategies  

</details>

---

## 📊 Key Insights & Visualizations

### 🔍 Dashboard Preview

#### 1️⃣ Dashboard 1 – Hospital Overview (Executive View)

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/overview-helathcare.png)


### 📌 Analysis 1

#### 🔎 Observation

**This dashboard provides a high-level overview of hospital performance, aligned with the North Star metrics: _Total Billing_ and _Total Patients_. It helps management quickly understand overall financial health, patient demand, and operational balance.**

Key observations include:

- **Total Billing Amount reaches ~£3M**, indicating strong overall revenue performance, but distribution is uneven across departments.
- **Total Patients ≈ 4,973**, showing high service demand, with noticeable variation by month and department.
- **Billing concentration by department**:
  - Cardiology and Orthopedics contribute the largest share of total billing.
  - Some departments generate significantly lower revenue, indicating uneven service contribution.
- **Treatment-related costs vs billing**:
  - Treatment cost and medication cost represent a large proportion of total expenses.
  - Certain procedures show high cost but relatively lower billing margins.
- **Insurance dependency is high**:
  - A large portion of billing comes from insurance-covered payments.
  - Out-of-pocket payments account for a smaller share, indicating reliance on insurers.
- **Geographic and departmental drill-down reveals concentration risk**:
  - Revenue and patient volume are concentrated in specific departments and regions.
  - This aligns with the “revenue dependency” risk identified in the empathy map.
- **Monthly trends show seasonality**:
  - Patient volume and billing fluctuate across months, suggesting demand peaks and slow periods.
  - These variations directly affect workload planning and financial stability.

This overview dashboard acts as the **entry point (Page 1)** in the analysis flow, enabling stakeholders to drill down into:
- Department-level performance  
- Doctor-level workload  
- Patient-level behavior  
- Cost structure and insurance exposure  

---

#### 💡 Recommendation

Based on the observations above, the following actions are recommended:

- **Balance revenue concentration risk**
  - Reduce over-reliance on a small number of departments by developing underperforming service lines.
  - Promote high-potential but underutilized departments through operational or service improvements.

- **Improve cost control and margin visibility**
  - Closely monitor treatment and medication costs relative to billing.
  - Identify procedures with high cost but low contribution margin for optimization.

- **Optimize resource allocation**
  - Use department-level billing and patient volume to rebalance staffing and equipment.
  - Allocate resources dynamically based on seasonal demand patterns.

- **Strengthen insurance strategy**
  - Monitor insurer dependency to reduce financial risk.
  - Use insights to negotiate better reimbursement terms or diversify payer mix.

### 🔍 Drill-down Analysis – Overview (Department-level)

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Drilldown.png)

**Focus:** Break down *Total Billing* from the overview level into departments to understand where revenue and cost are actually generated.

#### Observation
- Total billing is highly concentrated in a few departments, with **Cardiology** contributing the largest share.
- Treatment cost accounts for the majority of total cost across departments, while medication and room charges play a smaller role.
- Some departments show **high costs but relatively lower billing**, indicating potential inefficiencies.
- Monthly breakdown reveals noticeable fluctuations, suggesting seasonality in service demand.

#### Insight
- Revenue and cost are not evenly distributed across departments.
- A small number of departments drive most of the hospital’s financial performance.
- Cost structure is heavily driven by treatment-related activities rather than accommodation.
- Variations over time indicate the need for better capacity and workload planning.

#### Recommendation
- Prioritize performance monitoring for high-impact departments (e.g. Cardiology).
- Investigate departments with high costs but weaker billing outcomes.
- Use seasonal trends to plan staffing, budgeting, and resource allocation.
- Apply department-level drill-down as a starting point before analyzing doctors and diagnoses.

### 👨‍⚕️ Dashboard 2 – Doctors Performance Analysis

![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Doctors.png)
#### 🔍 Analysis 2: Doctor-level Drill-down

##### Observation
- A small number of doctors handle a disproportionately high number of patients.
- Some doctors with the highest patient volume show **lower average patient satisfaction scores**, indicating potential workload pressure.
- Billing contribution varies significantly by doctor, even within the same department.
- Certain doctors generate high billing with fewer visits, suggesting higher-value procedures or specialties.
- Workload distribution across doctors is uneven, especially on weekdays.

##### Insight
- High patient volume does not always correlate with high satisfaction or optimal performance.
- Overloaded doctors may face burnout risks, which can negatively affect care quality.
- Revenue concentration at the doctor level mirrors department-level concentration observed in the Overview dashboard.
- There is an imbalance between productivity, quality, and workload across doctors.

##### Recommendation
- Redistribute patient load more evenly among doctors within the same department.
- Use doctor-level KPIs (patients handled, billing, satisfaction score) together rather than in isolation.
- Identify high-performing doctors as benchmarks for best practices.
- Provide support or schedule adjustments for overloaded doctors to prevent burnout.
- Use doctor-level insights as input for workforce planning, incentives, and performance reviews.

### 🧑‍🤝‍🧑 Dashboard 3 – Patient Profile & Behavior Analysis

This dashboard focuses on **patient-level insights**, helping stakeholders understand who the patients are, how they use healthcare services, and how demand changes over time.

It extends the analysis from *departments* and *doctors* to the **end users of the healthcare system**, enabling better demand planning, service design, and patient experience improvement.

---
#### 🔍 Analysis 3: Patients Analysis
![image alt](https://github.com/tranthuyquynh122-cyber/Healthcare-Operations-Performance-Dashboard/blob/abb078c8933119a18dc981bd5a237a77d8b2c0aa/Patients.png)

##### Observation
- Total patient volume shows clear monthly fluctuations, indicating seasonal demand patterns.
- A small number of age groups account for the majority of patient visits.
- Emergency visits represent a significant share of total visits in certain months.
- Follow-up visit rates vary over time, suggesting inconsistent continuity of care.
- Patient distribution differs by insurance provider, showing reliance on a few major insurers.
- Some demographic segments contribute disproportionately to overall service demand.

##### Insight
- Patient demand is not evenly distributed across time or population groups, which can lead to workload imbalance.
- Seasonal spikes increase pressure on hospital capacity if not proactively planned.
- High emergency visit ratios may indicate gaps in preventive or outpatient care.
- Variations in follow-up rates reflect differences in treatment effectiveness and patient engagement.
- Strong dependence on specific insurance providers increases financial and operational risk.

##### Recommendation
- Use monthly and seasonal trends to proactively plan staffing, bed capacity, and appointment schedules.
- Strengthen preventive care and o

<a id="final-conclusion--recommendations"></a>
## 🔎 Final Conclusion & Recommendations  

Based on the overall analysis across the **Overview**, **Doctors**, and **Patients** dashboards, this project provides a holistic view of hospital operational performance, workload distribution, patient behavior, and revenue structure. The insights below synthesize the most critical findings and translate them into clear, actionable recommendations for hospital management.

---

### ✅ Key Takeaways

- Hospital performance is **highly dependent on a small number of departments and services**, especially Cardiology and Orthopedics, creating revenue concentration risk.
- Patient demand is **not evenly distributed across departments or doctors**, leading to workload imbalance and potential burnout.
- Doctors handling the highest patient volumes often show **lower patient satisfaction scores**, indicating service pressure and quality risks.
- Patient demand varies significantly by **age group, time period, and visit type (emergency vs non-emergency)**, revealing predictable behavioral patterns.
- Revenue is strongly influenced by **insurance coverage and reimbursement structure**, making financial performance sensitive to policy changes.
- Clear seasonal and monthly patterns exist in both patient volume and billing, which can be used for better capacity planning.

---

## 🎯Recommendations

### 1️⃣ Strengthen Patient Experience Management
- Introduce **structured post-visit satisfaction surveys** to identify root causes of dissatisfaction by department and doctor.
- Monitor satisfaction trends together with workload indicators to detect early warning signs of service quality decline.
- Use demographic insights (age group, visit type) to tailor patient communication and care pathways.

---

### 2️⃣ Balance Doctor Workload and Improve Performance
- Redistribute patient appointments to reduce overload on high-demand doctors.
- Use doctor-level KPIs combining:
  - patient volume  
  - satisfaction score  
  - procedure complexity  
  - billing contribution  
- Implement targeted coaching or mentoring programs for doctors with low satisfaction scores.
- Apply workload-based scheduling to improve efficiency and reduce burnout risk.

---

### 3️⃣ Reduce Revenue Concentration Risk
- Identify underperforming departments with growth potential and develop service expansion strategies.
- Reduce dependency on a small number of high-revenue services by promoting complementary treatments.
- Monitor revenue contribution by department and diagnosis regularly to detect early concentration risks.

---

### 4️⃣ Improve Financial Planning & Cost Control
- Track treatment, medication, and room costs alongside billing to better understand cost drivers.
- Use monthly and seasonal trends to forecast cash flow more accurately.
- Prepare contingency plans for changes in insurance reimbursement policies.
- Align budgeting decisions with observed demand patterns and service utilization.

---

### 5️⃣ Enable Data-Driven Decision-Making Culture
- Use the dashboard as a **regular management review tool**, not just a reporting artifact.
- Support decisions related to:
  - staffing allocation  
  - scheduling optimization  
  - budgeting and cost control  
  - service portfolio planning  
- Encourage cross-functional discussions using shared KPIs and visual insights.

---

## ✅ Final Summary

This project demonstrates how healthcare operational data can be transformed into **actionable insights** that support both strategic and day-to-day decision-making. By connecting patient behavior, doctor performance, and financial outcomes, the dashboard helps hospital leaders:

- improve service quality,
- balance workload,
- reduce operational risk,
- and strengthen long-term financial sustainability.

The framework can be easily extended to support forecasting, performance benchmarking, and continuous improvement initiatives across healthcare organizations.



