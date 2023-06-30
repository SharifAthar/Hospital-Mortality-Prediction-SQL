# <p align="center">Hospital Mortality Prediction Project</p>

#### **Tools Used**: Excel, MySQL, Tableau

[Dataset Used](https://www.kaggle.com/datasets/mitishaagarwal/patient)

[Hospital Mortality Dashboard on Tableau](https://public.tableau.com/app/profile/sharif.athar/viz/HospitalMortalityDashboard/Dashboard1)

- **Business Problem:** Healthcare professionals are trying to identify the main causes of in-hospital mortality for admitted patients. By having a clear understanding of the causes early on, healthcare professionals will be in a better position to develop targeted interventions, and implement evidence-based protocols to address the factors that contribute to in-hospital patient deaths. 

- **My Appraoch To Solving The Problem:** To tackle the business problem of identifying the main causes of in-hospital mortality for admitted patients, I wanted to do a comprehensive analysis leveraging SQL and Tableau. My approach involved obtaining the dataset, importing it into Excel, cleaning the data, then importing it to MySQL and conducting insightful queries to extract valuable information. Using my SQL skills, I delved into the dataset, exploring various patient attributes such as age, ethnicity, gender, weight, BMI, heart rate, and comorbidities. After executing the queries with SQL, I uncovered insightful patterns, trends, and correlations within the data. To present my findings in a visually appealing manner, I used Tableau to design an interactive dashboard. The dashboard summarized the key insights derived from my SQL analysis, showcasing patterns and trends related to in-hospital mortality. 

- **Insights I Gathered:** Below I will show the results of the SQL queries I conducted and provide explanations of the patterns and trends I found throughout the analysis.

1: 

![Query1](https://i.ibb.co/SV4r1Rt/Screen-Shot-2023-06-29-at-4-52-19-PM.png)

Out of the 10,000 admitted patients in the hospital, a total of 634 patients died, which translates to 6.34%. This meant that understanding the factors contributing to in-hospital mortality was highly important in improving patient care and reducing preventable deaths.

2:

![Query2](https://i.ibb.co/XC5qXg8/Screen-Shot-2023-06-29-at-7-44-37-PM.png)

This output showed the amount of patients that died and survived in each age group, categorized by 10-year intervals. There were far more admitted patients between the ages of 50-89 compared to patients who were between 0-49. Observing the results more, we can see that patients between ages 0-9 had the highest death percentage and each 10-year age group in the 50-89 range had a slight increase in death percentage. Nearly 1 in every 6 patients between the ages of 70-89 died in the hospital. 

3:

![Query3](https://i.ibb.co/MnB3M5L/Screen-Shot-2023-06-29-at-7-56-52-PM.png)

This output further proves that the death probability of a patient in the hospital rises as they get older.







