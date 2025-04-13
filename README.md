# defend-prognosis

This repository contains code and data to **generate and explain machine learning models** for predicting **COVID-19 severity** using real-world hospital data.

## Contents

- 🧪 **Two `.csv` files**: Preprocessed datasets from two major hospitals in Brazil.
- 📓 **Six Jupyter notebooks** covering:
  - Data labeling corrections
  - Data preprocessing
  - Predictive modeling
  - SHAP explainability analysis

## Notebooks Overview

### 🔧 `bp_labels` and `hsl_labels`

These notebooks address inconsistencies in the original test label assignments.  
In some cases, a test was linked to **divergent or ambiguous severity labels**. With the help of a **domain expert**, these conflicts were carefully resolved.

### 🧼 `bp_preprocessing` and `sírio_preprocessing`

Contain all code used to preprocess raw COVID-19 data from:

- **Hospital Beneficência Portuguesa (BP)**
- **Hospital Sírio-Libanês**

📌 Original raw data is publicly available at:  
https://repositoriodatasharingfapesp.uspdigital.usp.br/

### 📊 `severity_prognosis`

Includes code for training machine learning models to predict **severity outcomes** for patients from five hospitals.  
The prediction is based on routine clinical parameters collected **up to four days after initial hospital attendance**.

### 🧠 `SHAP_summaryplot`

Contains all code to generate SHAP summary plots for model explainability.

## Datasets

### 📁 `.csv` Files

- `hosp1.csv`: Preprocessed data from **Hospital Sírio-Libanês**
- `hosp2.csv`: Preprocessed data from **Hospital Beneficência Portuguesa**

These files are the result of the preprocessing steps described in the notebooks above.

## Looking for a More Refined Version?

A **refined and better-documented version** of the datasets, along with other real-world healthcare datasets from Brazil, is available in the repository:  
👉 [HealthDataBR](https://github.com/YOUR-USERNAME/HealthDataBR) *(replace with actual URL)*

## Citation

If you use these datasets or code in a scientific publication, we kindly ask you to cite the following paper:  
📄 

@inproceedings{Valeriano2022,
  doi = {10.1109/ccgrid54584.2022.00115},
  url = {https://doi.org/10.1109/ccgrid54584.2022.00115},
  year = {2022},
  month = may,
  publisher = {{IEEE}},
  author = {Maria Gabriela Valeriano and Carlos R. V. Kiffer and Giane Higino and Paloma Zanao and Dulce A. Barbosa and Patricia A. Moreira and Paulo Caleb J. L. Santos and Renato Grinbaum and Ana Carolina Lorena},
  title = {Let the data speak: analysing data from multiple health centers of the S{\~{a}}o Paulo metropolitan area for {COVID}-19 clinical deterioration prediction},
  booktitle = {2022 22nd {IEEE} International Symposium on Cluster,  Cloud and Internet Computing ({CCGrid})}
}
