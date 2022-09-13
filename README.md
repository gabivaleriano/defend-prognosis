# defend-prognosis

Generate and explain machine learning models to predict severity in COVID-19.
This repository contains two .csv files and six notebooks:  

## notebooks

### bp_labels and hsl_labels

In the original file tests, there are some cases when the same test have similar but divergent label. 
This cases were resolved with the help of an expert. These notebooks contains all the codes used to correct this issue. 

### bp_preprocessing and sírio_preprocessing

Contains all codes used do preprocessing data from Hospitals Beneficência Portuguesa and Sírio Líbanes.
Data available at https://repositoriodatasharingfapesp.uspdigital.usp.br/

### severity_prognosis 

Contains all codes used to generate machine learning predictive results for five hospitals. 
Data used contain routine attendance parameters collected up to four days after initial attendance.

### SHAP_summaryplot

Contains all codes used to generate summary plots using SHAP library. 

## .csv files

### hosp1 and hosp2

Contains the data resulted from preprocessing described in the notebooks. 
hosp1 refers to the Hospital Sirio Libanês data and hosp2 refers to the Hospital Beneficência Portuguesa data.

If you use these datasets in a scientific publication, we would appreciate citations to the following paper:

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
