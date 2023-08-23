# Heart Failure: Prediction using its Risk Factors

source: https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction

Cardiovascular diseases (CVDs) are the number 1 cause of death globally, taking an estimated 17.9 million lives each year, which accounts for 31% of all deaths worldwide. Four out of 5 CVD deaths are due to heart attacks and strokes, and one-third of these deaths occur prematurely in people under 70 years of age. Heart failure is a common event caused by CVDs and this dataset contains 11 features that can be used to predict a possible heart disease.

People with cardiovascular disease or who are at high cardiovascular risk (due to the presence of one or more risk factors such as hypertension, diabetes, hyperlipidaemia or already established disease) need early detection and management wherein a machine learning model can be of great help.

![electrocardiogram-36732](https://user-images.githubusercontent.com/125017784/230833923-0714860a-dca3-4971-bed7-eda5e18125ad.png)

## GOAL: 
- To help the stakeholder predict if the patient is likely to have a Heart Failure or not.

![Screenshot 2023-04-21 214624](https://user-images.githubusercontent.com/125017784/235896527-ae16e01c-cfe6-46bb-95af-7e09a8bfe056.png)

## Data cleaning
We have cleaned the data before using it to Machine Learning.
1. Duplicates has been checked
2. Missing values has been managed
3. Categorical values has been validated
4. Numerical Incosistencies has been taken care of

## Feature Engineering
This method was used to see if we can get a better prediction from the defaulted dataset.
1. Age was binned by decades
2. BP values was grouped by Blood Pressure Categories
3. Oldpeak was renamed by the disease it is associate with
   
# Exploratory Data Analysis:

<p align="center">
<img src=https://user-images.githubusercontent.com/125017784/235902485-fa957f24-ecfb-4d77-96f6-114eb5ae8288.png>
</p>

This chart shows the disctribution of patients with heart disease by age. As we can see we don't have a normal distribution on age - Most of our patients are in Late Middle age. We have few patients in Late Adulthood as well as in Early Middle age. According to research Late Adulthood (65 and above) are more at risk that any other age group. However, on this graph we see that the peak is at about age 58.
   
<p align="center">  
<img src=https://user-images.githubusercontent.com/125017784/235902476-000f399a-1f32-44cc-a83f-e9d32e80c3a1.png>
</p>

Typical angina (ATA) or Angina Pectoris is when heart does not get enough oxygenated blood because of blockage. This means that we expect more patients to have this symptom than others. This Bar graph shows the types of chest pain the patients with Heart Disease have. Surprisingly, most of our patients with the disease shows to have an Asymptomatic Chest Pain. Non-Anginal Pain(NAP) comes second. Typical Angina and Atypical Angina have almost the same ratio and there is about 25 patients with this Chest Pain. It seems like most of our patients with Heart Disease doesn't show much Angina than what I expected them to. 
   
<p align="center">   
<img src=https://user-images.githubusercontent.com/125017784/235902587-9321e716-8279-4b0f-851c-ff259d6ab1e3.png>
</p>

Upwards (ST elevation) is associated with Myocardial injury or also known as Heart Attack. Downwards (ST depression) is associated with Myocardial Ischemia, blockage of coronary artery. For this column, we are expecting to have more Up and Down values. Instead the graph shows that the data set has more Flat ST slope(Normal).

# Machine Learning

## Models used
1. Decision Tree
2. Random Forest
3. Light Gradient Boosting
4. Support Vector Machines

## Metrics for Best Model
Defaulted Dataset: 

<p align="center">
<img src=https://user-images.githubusercontent.com/125017784/235902415-a928beb0-0952-47ce-aae5-eff875b78dec.png> </br>
<img src=https://user-images.githubusercontent.com/125017784/236445437-4b8590ab-9162-497f-bf22-fce28563834e.png>
</p>


Engineered Dataset:
<p align="center">
<img src=https://user-images.githubusercontent.com/125017784/235902394-ad3f6ffe-3c60-4ffd-a4fb-049987f9872e.png> </br>
<img src=https://user-images.githubusercontent.com/125017784/236445442-308828d6-08f3-47ce-9e46-e817917cad67.png>
</p>



# Recommendation

Adding more information in our dataset would be appreciate as there are more factors that leads to HF that were not included in this research. Some examples are: 
</br>
<img src= https://github.com/juDEcorous/Heart-Disease-Prediction/assets/125017784/0421a37a-2e35-45aa-9210-b14b9929ee69>

