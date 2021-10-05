# defend-prognosis

Generate and explain machine learning models to predict severity in COVID-19.
This repository contains two Jupyter notebooks:  

### models_severity 

Contains all codes used to generate machine learning predictive results for five hospitals. 
Data used contain routine attendance parameters colected up to four days after initial attendance.

##### Inclusion criteria:
- Patients with positive PCR test for COVID, confirmed within a maximum of 15 days after attendance. 

##### Exclusion criteria:
- Patients with no total blood count records;
- Clinical and lab tests that were not done by at least 50\% of critical and 50\% of non-critical patients in that specific hospital. 

### SHAP_summaryplot

Contains all codes used to generate summary of importance with feature effects, plots use SHAP library.
