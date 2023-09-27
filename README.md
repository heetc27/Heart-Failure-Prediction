# Heart Failure Prediction 

## Introduction: 
Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worldwide. Heart failure is a common event caused by CVDs and this dataset contains 11 features that can be used to predict a possible heart disease. People with cardiovascular disease or who are at high cardiovascular risk need early detection and management wherein a machine learning model can be of great help.

## Problem Statement: 
To predict the chances of heart failure and studying the factors associated with it (such as Cholesterol levels, type of ChestPain, Heart Rate, Blood Pressure)

## Dataset: 
heart.csv imported from our github repository

## Observations:
<li>We observe that the Dataset has 12 Columns, (Age, Sex, ChestPainType, Resting BloodPressure, Cholesterol, Fasting Blood Sugar, Resting ECG. Maximum Heart Rate, Exercise Angina, Old Peak, ST_Slope and Heart Disease(present or absent)</ul>
<li>Resting BP and Cholesterol has zero as minimum which is not possible unless the patient is dead. </ul>
<li>There may be outliers/Missings in Cholesterol and Resting BP being presented as zero. </ul>
<li>The interquartile range of MaxHR suggests that there maybe outliers from Min to 1st quartile. </ul>

We have made use of logistic regression for prediction in our dataset since Logistic regression is a very useful algorithm for modeling a binomial outcome with one or more explanatory variables. In our case our binary variable which needs to be predicted is the presence or absence of Heart Disease (0 or 1) with its dependent variables such as Chest Pain Type, Cholesterol, Heart Rate etc.
Our model predicts the probability of the binary variable Heart Disease based on its predictor variables.

Split the dataset into 80% training and 20% testing using Caret.
We use the glm() function to create the regression model and get its summary for analysis.

## Conclusion
From the Decision Tree above, we can infer that:
<li>The First Criteria for heart diagnosis is ST_Slope, when recorded UP, there is a 18.6% likelihood that there is no heart disease, however there is an 82.3% likelihood that there is presence of heart disease making up for 57.6% of the people in the dataset. 
<li>The next criteria is ChestPainType which is assosciated with criterias OldPeak values and Sex. 
<li>As OldPeak continues to be less than 0.45, there is a 73% likelihood that the person has a heart disease.
