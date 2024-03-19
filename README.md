## 📝 Description
HumanForYou, a pharmaceutical company based in India with a workforce of approximately 4000 employees, has an issue where its annual empolyees turnover rate is about 15%, causing delays in projects, HR resource strain and inefficiencies in onboarding.

Project goal:
- Objective: Analyze data to identify influencing employee turnover.
- Task: Propose machine learning models to uncover insights and suggest improvements to motivate employees to stay.

## ⏳ Dataset
- Download the dataset files from this link: https://github.com/FlammeTik/AI_HR_Attrition/tree/d1f1f5312798d7126a1066c1f0494d3ed5b44d7d/Dataset

## :hammer_and_wrench: Requirements
* Python 3.5+
* Jupyter Notebook

## :mag: Data Pre-processing
* Created a feature called AVG_Work_Time.
* Removed non-related columns for my study like: EmployeeCount, EmployeeID, Gender, MaritalStatus, Over18 (all had the same value "Yes") & StandardHours (all had the same value "8").
* Applied custom mapping on these 2 categorical columns: Attrition & BusinessTravel. Here is the Attrition Destribution:

  <img width="540" alt="Attrition Destribution" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/a2ff2bf4-b46f-4932-9420-7cddf303f12e">
  
* Used OneHotEncoder on these 3 categorical columns: Department, EducationField & JobRole.
* Filled missing values using mean strategy.
* Created boxplots for each column to check for outliers. Here is a box plot for Monthly Income column:

  <img width="546" alt="Box Plot for MonthlyIncome" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/7bc043eb-844e-4150-8319-db0c205e451a">

* Ploted histograms for each column to see if the data is balanced or not:

  <img width="736" alt="Histograms" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/4149b177-dd7c-4291-b23c-7d48accd7d83">

* Ploted heat map for correlation matrix:

  <img width="671" alt="Correlation Matrix" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/82b16f3b-4271-4d30-bebf-f8c476194267">

* Applied the standard scaler since there were outliers within the data.
* Created the data pipeline encompassing all transformation steps for later use in machine learning.

## :desktop_computer:	Machine Learning
* I applied the previous data pipeline.
* Utilizing StratifiedShuffleSplit, I partitioned the data into two sets: 80% designated for training and 20% allocated for testing, ensuring representative stratification across the dataset.
* Employed five distinct classification models, systematically assessing for overfitting through cross-validation techniques. Subsequently, I computed various evaluation metrics for each model and discerned the optimal choice based on the precision score.

  <img width="644" alt="ROC Curve" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/536c5bff-bb91-4389-bbda-5cb151aa9a1f">
  
  <img width="513" alt="Evaluation Metrics" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/892beb76-47db-45d1-a642-87b8a850b0f3">

* Conducted hyper-parameter tuning for Random Forest Classifier, meticulously exploring various settings to ascertain the most effective combination for optimal performance.

  <img width="372" alt="Best parameters" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/a7b3c1a1-606e-4375-a535-6161d27173da">

* Tested the final model on the test set and got excellent results:

  <img width="168" alt="Evaluation Metrics - Test Set" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/f0e808c7-c073-45cb-8337-d9200e22a8ce">

## chart_with_upwards_trend: Feature Importance
* Here is a chart showing the sorted contribution of each column to the target column "Attrition":

  <img width="548" alt="Feature Importance" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/1fda86e7-1578-49ee-8ee8-634514d97791">

## 🎯 Recommendations


## Conclusion

## Contributors <img src="https://raw.githubusercontent.com/TheDudeThatCode/TheDudeThatCode/master/Assets/Developer.gif" width=35 height=25>
- Mohammed Reda Guellati
- Zakaria Ali Zouaoui
