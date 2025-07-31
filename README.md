# 🦠 COVID-19 Case Analysis using Python 🧬

This project presents an end-to-end data-driven analysis of COVID-19 patient-level data to extract critical health insights during the pandemic. It identifies key risk factors influencing **hospitalization**, **recovery timelines**, **reinfection trends**, and **long COVID symptoms**. With comprehensive EDA, data cleaning, and feature engineering, this project supports informed public health decisions.


## 📌 Problem Statement

The COVID-19 pandemic showed stark differences in health outcomes based on patient demographics, comorbidities, and vaccination status. The goal is to analyze detailed patient data to:
- Detect factors impacting disease severity and recovery.
- Assess the effectiveness of different vaccine types and doses.
- Understand reinfection trends and long COVID patterns.
- Support targeted interventions for high-risk populations.


## 🗂️ Dataset Highlights

- 🔢 **Records**: 3,000 patients
- 📌 **Features**: 26 columns including:
  - Demographics (Age, Gender, Region)
  - Health Conditions (BMI, Preexisting Conditions)
  - Infection Info (COVID Strain, Symptoms, Severity)
  - Vaccination Status & Doses
  - ICU/Ventilator/Hospitalization Data
  - Reinfection & Long COVID flags


## 🧹 Data Cleaning & Preprocessing

- ✅ Handled missing values using domain logic (e.g., filled `None` for missing preexisting conditions, vaccine type)
- 🔍 Removed columns with >30% nulls (`Date_of_Recovery`, `Date_of_Last_Dose`, etc.)
- 🧾 Treated outliers in **BMI** and **Recovery_Days** using IQR method
- 🧠 Created new features:
  - `Death` (based on recovery status)
  - `Age_Group`, `BMI_Category`
  - `Risk_Score = Age × BMI`

## 📊 Exploratory Data Analysis (EDA)

### 🔢 Numerical Insights
| Metric | Mean | Median | Std Dev |
|--------|------|--------|---------|
| Age | 53.9 | 54 | ±20.9 |
| BMI | 25.1 | 25.1 | ±4.89 |
| Recovery Days | 362.3 | 338 | ±239.4 |

- **Age** and **BMI** are symmetrically distributed
- **Recovery Days** is highly right-skewed

### 🧾 Categorical Trends
- 🧓 Most deaths occurred in **elderly** and **senior** age groups
- ❌ Unvaccinated patients had significantly higher mortality
- 💉 3-dose vaccinated individuals showed better recovery rates
- 🫁 Long COVID symptoms occurred in 7.3% of patients (Fatigue, Brain Fog, Chest Pain)


## 📈 Key Visual Insights

- 📊 **Boxplots & Histograms**: Age, BMI, Recovery Days distributions
- 🧍‍♂️ **CountPlots**:
  - Gender & Vaccination Status distribution
  - Death by Age Group & Vaccination Status
  - Hospitalization by Preexisting Condition
  - ICU Admission vs Ventilator Support
- 🧪 **Severity vs Hospitalized**: Most severe cases were hospitalized
- 📦 **Standard Deviation Analysis** for all numeric variables


## 🧠 Key Insights

- ⚠️ **Obesity**, **Cardiovascular**, and **Hypertension** were leading risk factors for hospitalization.
- 💉 Vaccinated patients (especially those with 2–3 doses) had better outcomes.
- 📉 ICU and Ventilator support was highly correlated with *High Severity*.
- 🧓 Age 65+ (Elderly/Senior) had the **highest death rates**.
- 🔄 Reinfection was rare but present in select vaccinated individuals.


## 🛠️ Tech Stack

- **Language**: Python
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib, SciPy
- **Notebook**: Jupyter
- **Data**: Structured CSV (3000 × 26)


## ✅ Future Enhancements
Integrate ML models to predict hospitalization or recovery duration

Develop an interactive dashboard using Streamlit or Power BI

Time series analysis on infection and recovery trends over time

## 📌 Conclusion
This project provides actionable insights into how COVID-19 severity, vaccination, and preexisting conditions intersect. It offers valuable input for public health policy, resource allocation, and vaccination planning.

## 🙌 Acknowledgements
Thanks to the medical data contributors and open data initiatives that made this project possible.

## 📬 Contact

If you found this project insightful or would like to collaborate on data science, healthcare analytics, or Python-based projects — feel free to reach out:

- 📧 **Email**: bisenpooja441801@gmail.com  
- 💼 **LinkedIn**: www.linkedin.com/in/pooja-bisen-313238263  
- 💻 **GitHub**: https://github.com/Pooja12Bisen

I’m always open to connecting with fellow developers, data enthusiasts, and researchers.  
Let’s build something impactful together! 🚀


