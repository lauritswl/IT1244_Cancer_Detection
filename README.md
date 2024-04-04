# IT1244 Cancer Detection Project: XGBoost on multiclass identification
Project for NUS IT1244 by Team 43 - Laurits Lyngbaek & Tan Century

## How to run the project
The project contains outputs from three files: 
 - 'Code/PCA_XGboost.ipynb'
    - This files produces the PCA-analysis and shows the failed model that was discarded. It also produces the cumsum plot used in the report.
 - 'Code/Binary_Classification_XGBoost.ipynb'
    - This files produces the binary cancer-healthy classification model. It should run as is, and produce correlation heatmap, binary confusion matrix and numric results.
 - 'Code/Multicalss_predict_XGBoost.ipynb'
    - This files produces the multiclass classification model. It should run as is, confusion matrix from the report and the numric results. The randomsearch is saved in DATA, to avoid running the search again, as it took 7 hours.

### Needed libraries:
The libraries needed to run the code is noted down in the requirements.txt file


# Data Description:
- classification dataset
- around 2100 training samples and around 1000 test samples
- first 350 columns (length_51, length_52, ..., length_400) are features: "length_51" denotes the max normalized frequency of DNA fragment length 51
- last column (class_label) is the sample class: healthy/screening stage/early stage/mid stage/late stage cancer
- It's a class imbalanced dataset

# Task:
- need to classify cancer vs healthy
- need to try and do well for (1) screening stage cancer vs healthy and (2) early stage cancer vs healthy
- need to use appropriate metrics (not accuracy) to account for positive class accuracy and negative class accuracy

