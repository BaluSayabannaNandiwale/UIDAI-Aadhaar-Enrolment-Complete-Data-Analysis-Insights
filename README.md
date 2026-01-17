# UIDAI Aadhaar Enrolment – Complete Data Analysis & Insights

## 🏛️ Hackathon Details
**Event:** Online Hackathon on Data-Driven Innovation for Aadhaar  
**Organised by:** Unique Identification Authority of India (UIDAI)  
**In association with:** National Informatics Centre (NIC) & MeitY  
**Mode:** Online (Final presentation – In-person for shortlisted teams)

---

## 🎯 Problem Statement
Unlocking societal trends in Aadhaar enrolment and updates by identifying
meaningful patterns, trends, anomalies, and predictive indicators that can
support informed decision-making and system-level improvements.

---

## 📌 Project Objective
The objective of this project is to analyse anonymised Aadhaar enrolment datasets
released by UIDAI to:
- Understand age-wise enrolment patterns
- Identify regional disparities across states and districts
- Analyse temporal enrolment trends
- Detect anomalies or unusual enrolment behaviour
- Build a predictive model to estimate future enrolment trends

---

## 📂 Datasets Used
### Aadhaar Enrolment Dataset (Aggregated & Anonymised)

The dataset provides aggregated information on Aadhaar enrolments across
various demographic and geographic levels.

**Files Used:**
- `api_data_aadhar_enrolment_0_500000.csv`
- `api_data_aadhar_enrolment_500000_1000000.csv`
- `api_data_aadhar_enrolment_1000000_1006029.csv`

**Key Attributes:**
- Date of enrolment
- State
- District
- PIN Code
- Age-wise categories:
  - 0–5 years
  - 5–17 years
  - 18 years and above

All datasets were consolidated to ensure complete coverage and avoid sampling bias.

---

## 🧪 Methodology
The analysis follows a structured and reproducible workflow:

1. **Data Loading & Consolidation**
   - Combined multiple CSV files into a single dataset

2. **Data Cleaning & Preprocessing**
   - Standardised column names
   - Handled missing values
   - Converted date fields
   - Extracted year and month features

3. **Feature Engineering**
   - Created `total_enrolment` from age-wise columns
   - Derived time-based features for trend analysis

4. **Exploratory Data Analysis**
   - Univariate analysis (age-wise enrolment)
   - Bivariate analysis (state-wise, district-wise)
   - Trivariate analysis (state × year × age group)

5. **Data Visualisation**
   - Bar charts, line plots, histograms
   - Heatmaps for multi-dimensional analysis
   - All plots saved automatically for reporting

6. **Anomaly Detection**
   - Applied Z-score method to detect extreme enrolment spikes

7. **Predictive Modelling**
   - Built a Linear Regression model to analyse enrolment trends over time

---

## 📊 Key Analyses & Visualisations
All visualisations are programmatically saved in the `outputs/` folder.

- Age-wise Aadhaar enrolment distribution
- Top 10 states by total enrolment
- Monthly enrolment trend analysis
- District-level enrolment distribution
- State × Year adult enrolment heatmap
- Anomaly detection scatter plot
- Actual vs predicted enrolment trend

---

## 📈 Key Insights
- Aadhaar enrolments are predominantly driven by the adult population (18+)
- Significant enrolment disparities exist across states and districts
- Temporal analysis shows a steady long-term growth trend
- Certain districts exhibit abnormal enrolment spikes, possibly due to special drives
- Predictive modelling indicates sustained future demand for Aadhaar services

---

## 🛠️ Technology Stack
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy
- **Environment:** Jupyter Notebook
- **Version Control:** Git & GitHub

---

## ▶️ How to Run the Project
1. Clone the repository:
```bash
git clone https://github.com/your-username/uidai-aadhaar-enrolment-analysis.git
