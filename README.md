# Medilytics Healthcare Analysis

## **Overview** ##
![alt text](https://i0.wp.com/timoelliott.com/blog/wp-content/uploads/2014/01/predictive-maintenance-health.jpg?ssl=1)
This comprehensive project delves into the intricacies of healthcare data, specifically analyzing de-identified Inpatient Discharge records from diverse New York Hospitals spanning the years 2009 to 2021. The primary objective is to extract valuable insights regarding patient demographics, prevalent diseases, medical procedures, and the financial landscape of the healthcare industry. It involves development of a predictive model for estimating total charges and costs associated with hospital discharges. 

## **Contents** ##

* ### **Data Preparation** ##
The code extracts relevant columns from "Hospital Inpatient Discharges (SPARCS De-Identified) Dataset" provided by the New York State Department of Health from the year 2009 to 2021 listed in https://health.data.ny.gov, which contains a rich and anonymized repository of healthcare information capturing the landscape of inpatient care in the state of New York. The dataset offers priceless insights into patient admissions, diagnoses, medical procedures, and a wide array of healthcare-related variables such as Clinical Classification Software (CCS) and All Patient Refined (APR). 

* ### **Exploratory Data Analysis (EDA)** ### 
In-depth analysis of the data, unraveling insights through exploratory data analysis. This section sheds light on the processing and cleaning tasks necessary for the actual analysis. It delves into the       complexity of the standardization process, including the mapping of alphanumeric codes and the utilization of rapidfuzz logic for description standardization.
  #### **Alphanumeric to Numeric Mapping:** ####
The conversion of alphanumeric codes to numeric codes requires careful consideration of the alphanumeric patterns and their corresponding numeric formats. When analyzing the data, we realized that the CCSR (Clinical Classification Software Refined) Diagnosis and Procedure Codes were alphanumeric for the years 2018 to 2021 while they were simply numeric for the years before 2018. On further researching about these, we realized that the codes were updated universally by the Healthcare Cost and Utilization Project, which is a Federal-State-Industry partnership sponsored by the Agency for Healthcare Research and Quality.
The transition went through several phases in its structure and format in which each transition served specific purposes addressing evolving needs in healthcare data management and standardization. The ICD-9 codes had a finite number of available codes and lacked the specificity needed to represent complex diagnoses and procedures accurately. ICD-10 provided a significantly broader range of alphanumeric codes, allowing for greater precision, specificity, and detailed classification of diseases, injuries, and medical procedures. To make it more granular, the ICD-10 codes were later updated to more structured alphanumeric codes. More than 80,000 ICD-10-PCS procedure codes were converted over 320 clinically meaningful categories. Similarly, around 70,000 diagnosis codes were mapped down to around 300 clinically meaningful categories.

* ### **Data Analysis** ##  
**Question of interest**  
1. Demographic Influence on Disease and Treatment:  
How do population demographics affect disease contraction? We will analyze variables such as age, gender and ethnicity to uncover patterns.  
2. Temporal Shifts in Disease Vulnerability:  
How has the susceptibility of different demographic groups to certain diseases changed over time?  
3. Evolution of Treatment Methods:  
How have the treatments administered for certain diseases evolved through the years? We will track changes in medical procedures and correlate them with advancements in medical technology and guidelines.  
4. Predicting Hospital Discharge Charges:  
Can we develop a model to predict discharge charges more accurately, thereby reducing the gap between estimated and actual charges? This involves analyzing financial data related to patient care and hospital charges.  

**Time Series Analysis**  
An engaging exploration of procedural changes over the years, with a specific focus on the treatment of diseases. This section unravels the consistency and adaptability of medical treatments.  
**Predictive Model**  
A sophisticated approach to building predictive models for forecasting total charges and costs associated with hospital discharges. Detailed insights into the training, evaluation, and assessment of the models are provided.  

## **Future Scope** ##  
A visionary outlook emphasizing the project's evolution, with plans to incorporate more cities, enrich the regression model, and continually refine the analyses for improved healthcare decision-making and outcomes.  
