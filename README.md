# Heart Disease Health Indicators: Strategic EDA
**Author:** Jyoti Prakash Das  
**Project Objective:** To analyze health and demographic traits to identify the primary drivers leading to Heart Disease.

---

## 📌 Project Overview
This project performs an in-depth **Exploratory Data Analysis (EDA)** on the 2015 BRFSS (Behavioral Risk Factor Surveillance System) dataset. With over **253,000 survey responses**, the goal was to differentiate between modifiable lifestyle factors (like BMI and smoking) and non-modifiable factors (like age) to determine their impact on cardiovascular health.

---

## 🛠️ The Analytical Workflow
To ensure the integrity of the findings, the project followed a structured data science pipeline:

1. **Data Cleaning & Integrity:** * Handled a large-scale dataset with 22 health-related features.
   * Identified and removed **23,899 duplicate records** to prevent statistical bias.
   * Mapped encoded categorical values (Age, Income, Education) to human-readable labels for better interpretability.
   
2. **Univariate Analysis:** * Examined the distribution of the population, identifying a heavy skew toward the 60+ age demographic and a target class imbalance (~10% heart disease prevalence).
   
3. **Bivariate Analysis:** * Compared every feature against the target variable (`HeartDiseaseorAttack`).
   * Quantified the risk increase associated with clinical factors like High Blood Pressure and High Cholesterol.
   
4. **Correlation Study:** * Generated a correlation matrix to rank variables by predictive power.
   * Investigated the "Alcohol Paradox" and identified it as a confounding variable related to age.

---

## 📊 Key Findings & Insights
The analysis yielded four primary conclusions:

* **Top Clinical Drivers:** High Blood Pressure and High Cholesterol are the most significant physiological indicators. Patients with High BP are statistically three times more likely to have experienced a heart attack.
* **The Demographic Peak:** Age is the strongest non-modifiable risk factor, with a clear exponential increase in risk starting at age 50.
* **Socioeconomic Correlation:** There is a distinct "protective shield" provided by education and income; higher socioeconomic status correlates with significantly lower instances of heart disease.
* **Self-Awareness:** Self-reported "General Health" is highly accurate, showing a strong correlation (r=0.25) with actual heart disease history, suggesting patient perception is a powerful diagnostic tool.

---

## 💻 Technologies Used
* **Programming Language:** Python 3.x
* **Libraries:** * **Pandas & NumPy:** For data cleaning and numerical manipulation.
    * **Matplotlib & Seaborn:** For generating professional-grade statistical visualizations.
* **Platform:** Jupyter Notebook / Google Colab

---

## 📜 Conclusion
The project concludes that while lifestyle factors like BMI and smoking are important, **clinical markers (BP/Cholesterol)** and **socioeconomic factors** are the dominant predictors in this dataset. This suggests that public health interventions should prioritize clinical screenings and health equity initiatives for low-income demographics.
