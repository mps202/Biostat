# Biostat
Assessing the Impact of Lifestyle Choices on Diabetes Risk

Background:

Diabetes has become a significant public health concern, characterized by elevated blood sugar levels that can lead to serious complications such as heart disease, stroke, and kidney failure. Understanding the factors that contribute to diabetes risk is essential for effective prevention and management strategies. The dataset used in this analysis, sourced from Kaggle (https://www.kaggle.com/datasets/prosperchuks/health-dataset), encompasses a range of health and lifestyle variables, including age, sex, BMI, smoking status, and physical activity levels.

Objectives for Diabetes Risk Analysis Project:
This dataset provides a valuable opportunity to explore how various factors are associated with the likelihood of developing diabetes. By analyzing these variables, we aim to uncover critical patterns and relationships that can inform personalized healthcare strategies and public health interventions. The goal of this project is to leverage data-driven insights to enhance our understanding of diabetes risk factors, support preventive measures, and contribute to better management practices for individuals at risk. 


<class 'pandas.core.frame.DataFrame'>
RangeIndex: 70692 entries, 0 to 70691
Data columns (total 18 columns):
 #   Column                Non-Null Count  Dtype  
---  ------                --------------  -----  
 0   Age                   70692 non-null  float64
 1   Sex                   70692 non-null  float64
 2   HighChol              70692 non-null  float64
 3   CholCheck             70692 non-null  float64
 4   BMI                   70692 non-null  float64
 5   Smoker                70692 non-null  float64
 6   HeartDiseaseorAttack  70692 non-null  float64
 7   PhysActivity          70692 non-null  float64
 8   Fruits                70692 non-null  float64
 9   Veggies               70692 non-null  float64
 10  HvyAlcoholConsump     70692 non-null  float64
 11  GenHlth               70692 non-null  float64
 12  MentHlth              70692 non-null  float64
 13  PhysHlth              70692 non-null  float64
 14  DiffWalk              70692 non-null  float64
 15  Stroke                70692 non-null  float64
 16  HighBP                70692 non-null  float64
 17  Diabetes              70692 non-null  float64
dtypes: float64(18)
memory usage: 9.7 MB
None

Overview of Your Dataset:
Number of Observations (Rows): 70,692
Target Variable: Diabetes
This is the binary variable that indicates whether the individual has diabetes (1) or not (0).
Predictor Variables (Features):
These are the features that will be used to predict the target variable Diabetes. They include:

Age: Continuous variable representing age.
Sex: Binary variable (likely 0 for female and 1 for male).
HighChol: Binary variable indicating high cholesterol (0 for no, 1 for yes).
CholCheck: Binary variable indicating if cholesterol has been checked.
BMI: Continuous variable representing body mass index.
Smoker: Binary variable indicating smoking status (0 for non-smoker, 1 for smoker).
HeartDiseaseorAttack: Binary variable indicating history of heart disease or heart attack.
PhysActivity: Binary variable indicating physical activity.
Fruits: Binary variable indicating fruit consumption.
Veggies: Binary variable indicating vegetable consumption.
HvyAlcoholConsump: Binary variable indicating heavy alcohol consumption.
GenHlth: Ordinal categorical variable (numerical representation) for general health (1-5 scale or another range).
MentHlth: Continuous variable representing days of poor mental health in the last 30 days.
PhysHlth: Continuous variable representing days of poor physical health in the last 30 days.
DiffWalk: Binary variable indicating difficulty walking.
Stroke: Binary variable indicating history of stroke.
HighBP: Binary variable indicating high blood pressure.
