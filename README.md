# Cardiovascular Disease Prediction Analysis
<p align="center">
  <img src="https://github.com/aliaksparkh/Cardiovascular-prediction/blob/main/Coronary-heart-disease.jpg" width="400">
</p>

Welcome to my **[project](https://github.com/aliaksparkh/Cardiovascular-prediction/blob/main/cardiovascular_v2.ipynb)**!

## Project Description
This project focuses on predicting the risk of coronary heart disease (CHD) based on various health metrics. Using logistic regression and other classification techniques, the analysis explores key predictors of heart disease and evaluates the model's performance through various metrics like accuracy, ROC-AUC, precision, and recall. The dataset used contains patient data, including features like age, blood pressure, glucose levels, and smoking habits. Exploratory data analysis, feature engineering, and data cleaning were performed in **Jupyter Notebook**(VSCode). The dataset used for this project was sourced from [Kaggle](https://www.kaggle.com/datasets/christofel04/cardiovascular-study-dataset-predict-heart-disea/data) .

## Project Structure
1. **Data Cleaning and Preprocessing:**  
The dataset was carefully prepared to ensure high-quality inputs for model training, including:  
- Handling outliers and missing values in critical variables like glucose and systolic blood pressure.  
- Encoding categorical variables such as gender and smoking status.  
- Applying logarithmic transformations to normalize skewed distributions in continuous variables, especially glucose levels.

2. **Exploratory Data Analysis:**  
Key factors influencing heart disease risk were identified through:  
- Age: Older individuals had a significantly higher risk.  
- Systolic Blood Pressure: Elevated systolic pressure was strongly linked to higher CHD risk.  
- Smoking: A clear correlation was found between smoking and increased CHD risk.  
- Diabetes: Diabetic patients had a much higher likelihood of developing heart disease.  
- Gender: Males were found to be at greater risk of heart disease compared to females.

3. **Model Training:**  
Key steps in building the logistic regression model included:  
- Selecting important features such as age, sex, systolic blood pressure (sysBP), smoking habits, and diabetes status.  
- Normalizing skewed variables to enhance the model’s predictive power.  
- Training a logistic regression model using a balanced class approach to handle the imbalanced dataset (more non-diseased cases than diseased cases).  
- Threshold Adjustment for Better Sensitivity. 
A key focus of the analysis was on identifying as many true positives (diseased cases) as possible. By lowering the prediction threshold to 0.3 (from the typical 0.5), the model was able to increase its sensitivity (recall), successfully detecting 91% of the diseased individuals. However, this came at the cost of higher false positives, as more non-diseased individuals were misclassified as having heart disease.

4. **Conclusions and Areas for improvement**  

The logistic regression model achieved:  
- **Accuracy:** 66%  
- **ROC-AUC Score:** 0.71  
- **Recall (sensitivity):** 91% for diseased cases, which is critical for minimizing missed heart disease diagnoses.  


### Requirements
- Python 3.x  
- Jupyter Notebook  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Statsmodels  
- Scikit-learn  
