# <p align="center">Hospital Mortality Prediction Project</p>

# <p align="center"> ![pic](https://media.istockphoto.com/id/1194838627/vector/patient-in-hospital.jpg?s=612x612&w=0&k=20&c=LqhY8qXr1IgGA0PjGLwqEyVJL-MBTFBU5rf3Dcg4DWo=) </p>

#### **Tools Used**: Excel, MySQL, Tableau

[Dataset Used](https://www.kaggle.com/datasets/mitishaagarwal/patient)

[SQL Analysis (Code)](https://github.com/SharifAthar/Hospital-Mortality-Prediction-SQL/blob/main/Hospital_Mortality_SQL_Analysis.sql)

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

4:

![Q4](https://i.ibb.co/54ZBMBH/Screen-Shot-2023-06-29-at-8-08-53-PM.png)

![Q5](https://i.ibb.co/mJB1cxY/Screen-Shot-2023-06-29-at-8-09-28-PM.png)

These two outputs give more insight to the outcomes of patients in each ICU admit source & type. A vast majority of the patients were admitted to the "Accident & Emergency" ICU admit source and it also experienced the highest number of deaths. However, the ICU admit source with the highest probability of death was "Floor" with a percentage of 11.76. "Other ICU" was ignored because of its very small sample size. 

In the second output where death results are shown for each ICU type, there is a clear outlier: Med-Surg ICU

5:

![Q6](https://i.ibb.co/5cCNgyW/Screen-Shot-2023-06-29-at-8-32-29-PM.png)

Average weight, BMI, and max heart rate among the patients that died. 

The average weight of 67.57 kg (149 in lbs) suggests that, on average, the patients who passed away had a relatively moderate weight. The average BMI of 23.3 indicates that, on average, the patients who died had a BMI within the normal range. This suggests that weight alone may not be the sole determinant of mortality, as individuals with a normal BMI can also face significant health risks and complications leading to hospital death. The average maximum heart rate of 115.1 highlights a potential cardiovascular aspect in the patients' health profiles. Elevated heart rates can be indicative of underlying conditions ([source](https://www.mayoclinic.org/diseases-conditions/tachycardia/symptoms-causes/syc-20355127)), such as cardiac distress or organ failure, which might have contributed to the hospital mortality outcomes observed.

6: 

![Q7](https://i.ibb.co/GHb3dnT/Screen-Shot-2023-06-29-at-8-48-21-PM.png)

There were a total of 8 comorbidities in the dataset, and the 3 shown in the output results above (Diabetes, Immunosuppression, and Solid Tumor) had the highest probability of death with diabetes being the highest, by far. This highlights the importance of managing and monitoring this condition effectively during hospitalization.

7: 

![Q8](https://i.ibb.co/Tkc9RVr/Screen-Shot-2023-07-01-at-2-56-23-PM.png)

Generally speaking, and as shown by this output, prolonged stays in the ICU are associated with higher mortality rates ([source](https://pubmed.ncbi.nlm.nih.gov/26571190/#:~:text=One%2Dyear%20mortality%20was%2026.6,the%20need%20for%20mechanical%20ventilation.)). An increased length of stay in the ICU can be due to a number of reasons, such as cardiovascular system diseases, nervous system diseases, infections, underlying illnesses, and increased exposure to potential complications ([source](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5884409/#:~:text=Our%20study%20showed%20a%20significantly,the%20length%20of%20stay%20increases.)). According to this output, a patient who stayed in the ICU for longer than a day had a higher chance of death compared to someone who spent less than a day in the ICU. 

- **Conclusion:** Age was the first big predictor of in-hospital mortality from this dataset. Consistently, advanced age has been associated with higher rates of medical conditions, complications, and death. According to the dataset, nearly 20% of the patients who were 70 years old or older experienced in-hospital mortality. This finding highlights the significant impact of age on mortality risk among older individuals. Another strong predictor of in-hospital mortality is comorbidities. Diabetes emerged as the most notable comorbidity, with a mortality rate of 24.45% among patients diagnosed with this condition. Heart rate can also be very telling to predict mortality as it reflects the cardiovascular status and overall physiological stability of patients. Abnormalities in heart rate, such as tachycardia (elevated heart rate) or bradycardia (low heart rate), often indicate underlying cardiovascular dysfunction or compromised perfusion ([source](https://www.mayoclinic.org/diseases-conditions/tachycardia/symptoms-causes/syc-20355127)). Research has consistently shown a strong association between abnormal heart rates and increased mortality risk. In this dataset, the average max heart rate for patients that died was 115.1. Generally, a resting heart rate is high if it is over 100 bpm ([source](https://www.healthline.com/health/dangerous-heart-rate)). The length of stay at an ICU was also an important indicator of mortality, showing that patients who stayed for less than a day at the ICU had a much better chance for survival.

- **Next Steps/Recommendations:** While the dataset managed to provide several good predictors for in-hospital mortality, it failed to include other common factors that would have influenced patient mortality. For instance, the dataset did not include information on specific treatments received, such as other vital signs, medications, surgeries, or interventions, which could have played a significant role in patient outcomes. Additionally, the dataset lacked socioeconomic variables, which have been shown to impact healthcare access, quality of care, and ultimately, mortality rates. Furthermore, psychosocial factors, such as mental health conditions, social support, and patient preferences, were not captured in the dataset, despite their known association with mortality. To gain a more comprehensive understanding of in-hospital mortality, future studies should strive to incorporate these additional variables to provide a more nuanced and holistic analysis of the factors influencing patient outcomes. 
