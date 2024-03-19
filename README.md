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
* Applied custom mapping on these 2 categorical columns: Attrition & BusinessTravel.
  Here is a the Attrition Destribution:
  <img width="540" alt="Attrition Destribution" src="https://github.com/FlammeTik/AI_HR_Attrition/assets/95188070/a2ff2bf4-b46f-4932-9420-7cddf303f12e">

* Used OneHotEncoder on these 3 categorical columns: Department, EducationField & JobRole.
* Filled missing values using mean strategy.
* 

## :desktop_computer:	Machine Learning


## 🎯 Inference demo

## Contributors <img src="https://raw.githubusercontent.com/TheDudeThatCode/TheDudeThatCode/master/Assets/Developer.gif" width=35 height=25>
- Mohammed Reda Guellati
- Zakaria Ali Zouaoui
