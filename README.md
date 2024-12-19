# DMBI_final_project
Project Overview
This project focuses on analyzing neural response data to identify significant patterns and metrics that differentiate conditions (CONSISTENT, CONTROL, MISLEADING). The analysis uses data collected from various electrodes across multiple time windows and involves the application of statistical and machine learning methods.
Main Goals
Find important electrode readings that are linked to specific conditions.
Identify which features of the data are the most useful for separating the conditions.
Use machine learning models to classify the conditions and check their accuracy.
Reduce the size of the data using PCA (Principal Component Analysis) while keeping important information.
Data Used
Peak Data: Voltage and latency measurements from electrodes.
ALLTRIALS Data: Response values (AUC) measured over different time windows:
150–275ms
150–350ms
250–400ms
300–500ms
550–800ms
Steps in the Project
Load and Clean Data:

Import Peak and ALLTRIALS data from files.
Remove unnecessary columns and restructure the data for easier analysis.
Correlation Analysis:

Check for relationships between electrode readings (Peak Data) and AUC values (ALLTRIALS Data) to find significant features.
Feature Analysis:

Identify the most variable features that can help distinguish between the conditions.
Machine Learning Models:

Train models like Logistic Regression, Random Forest, SVM, Gradient Boosting, and XGBoost.
Test their performance in classifying the conditions.
Dimensionality Reduction:

Use PCA to simplify the data and test its effect on model accuracy.
Results
Important Features:
Key electrode readings: Fp2 and C4.
Key time windows: 250–400ms and 300–500ms.
Best Models:
XGBoost: Accuracy ~35%.
Random Forest: Accuracy ~32%.
Requirements
Make sure you have the following Python libraries installed:

pandas
numpy
scipy
sklearn
seaborn
matplotlib
xgboost

Conclusion
This project helps in understanding how the brain responds under different conditions using neural data. Machine learning models and statistical methods identify the key electrode readings and time windows that are the most relevant for this analysis.
