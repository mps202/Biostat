# Biostat

Assessing the Impact of Health and Lifestyle Factors on Hypertension Risk

Background:

Hypertension, commonly known as high blood pressure, is a major public health concern that increases the risk of heart disease, stroke, and other serious conditions. It is often associated with various health and lifestyle factors such as age, cholesterol levels, blood pressure, physical activity, and more. Understanding these factors is crucial for identifying individuals at risk and developing strategies to prevent and manage hypertension effectively. The dataset used in this analysis, sourced from Kaggle (https://www.kaggle.com/datasets/prosperchuks/health-dataset), it contains a variety of health indicators, including age, sex, chest pain type, cholesterol levels, resting blood pressure, and physical activity. 
Categorical Variables
Categorical variables represent discrete categories or groups. In your dataset, these are:

sex: Gender of the individual (binary: typically 0 for female, 1 for male).

cp: Chest pain type (typically categorical with different values representing different types).

fbs: Fasting blood sugar (binary: 0 or 1).

restecg: Resting electrocardiographic results (categorical with discrete values).

exang: Exercise induced angina (binary: 0 or 1).

slope: Slope of the peak exercise ST segment (categorical with discrete values).

ca: Number of major vessels colored by fluoroscopy (categorical with discrete values).

thal: Thalassemia (categorical with discrete values).

Numerical Variables
Numerical variables represent measurable quantities and can be either continuous or discrete. In your dataset, these are:

age: Age of the individual (continuous).

trestbps: Resting blood pressure (continuous).

chol: Serum cholesterol level (continuous).

oldpeak: Depression induced by exercise relative to rest (continuous).

target: Presence or absence of heart disease (binary, but often treated as categorical for classification tasks).




# Key Insights:

Age:

Mean age is 55.66 years with a standard deviation of 15.19, indicating a broad age range in the dataset.
The minimum age is 11 years, and the maximum is 98 years.


Sex:

The average value is 0.5, reflecting an approximately even distribution between males (1) and females (0).

Chest Pain Type (cp):

Mean value of 0.96 indicates most participants likely belong to lower chest pain categories (closer to 0).
Distribution ranges from 0 to 3, covering all chest pain types.


Resting Blood Pressure (trestbps):

Mean resting blood pressure is around 131.59 mm Hg, with values ranging from 94 to 200 mm Hg.

Cholesterol (chol):


The mean cholesterol level is 246.25 mg/dL, which is elevated, considering normal values are usually below 200 mg/dL.

Fasting Blood Sugar (fbs):


Mean is 0.15, showing that about 15% of the participants have fasting blood sugar > 120 mg/dL (coded as 1).


Thalach (Maximum Heart Rate Achieved):


The mean heart rate is 149.66 bpm, with a minimum of 71 bpm and a maximum of 202 bpm.


Exercise-induced Angina (exang):

Around 32.6% of participants experience exercise-induced angina (mean = 0.33).


Oldpeak:

The average ST depression induced by exercise relative to rest is 1.04, with values as high as 6.2, indicating considerable 

variability.


Slope:

Mean slope value is 1.4, which indicates most participants have upsloping ST segments (1).


CA (Number of Major Vessels Colored by Fluoroscopy):

Most participants have 0 major vessels colored by fluoroscopy (mean = 0.72).


Thalassemia (thal):

Mean thalassemia value is 2.32, reflecting that most participants have normal or fixed defect thalassemia (2).


Target:

The target variable has a mean of 0.55, suggesting the dataset is nearly balanced between participants with hypertension (1) and those without (0).



# Metrics Interpretation:

Accuracy: 0.8563

Meaning: Approximately 85.63% of the predictions made by the model are correct. This is a good accuracy rate, indicating that the model is performing well overall in classifying the data.

Precision: 0.8392

Meaning: Of all the instances predicted as having hypertension, approximately 83.92% are actually hypertensive. Precision is particularly important when the cost of false positives is high. In this case, it measures how well the model avoids incorrectly classifying individuals as having hypertension when they do not.

Recall: 0.9167

Meaning: Out of all the actual cases of hypertension, the model correctly identifies 91.67% of them. Recall is crucial when the cost of missing actual cases (false negatives) is high. In this context, a high recall value indicates that the model is good at detecting those who actually have hypertension.

F1-Score: 0.8763

Meaning: The F1-Score is the harmonic mean of precision and recall. It provides a single metric that balances both the precision and recall. An F1-Score of 0.8763 suggests a good balance between precision and recall, meaning the model performs well in both detecting true positives and minimizing false positives.


Contextual Analysis:

High Recall: The model is particularly effective at identifying individuals with hypertension. This is important in a medical context where failing to detect a true case of hypertension (false negative) could have serious health implications.

Good Precision: While the model does a good job of identifying hypertension cases, there's a small chance that some individuals predicted to have hypertension might not actually have it. This trade-off is acceptable in many scenarios where the cost of missing a case is higher than falsely identifying one.

Balanced Performance: The high F1-Score indicates that the model maintains a balance between precision and recall, which is beneficial in ensuring that both false positives and false negatives are kept to a reasonable level.


Overall, the logistic regression model is performing well in predicting hypertension, with a good balance between detecting true cases and minimizing false positives. This performance is especially useful in medical scenarios where detecting true cases is crucial, and we want to minimize the chance of missing those who need treatment.


# 5. Best Model Selection

The model's performance with the selected features from backward selection has slightly improved compared to the previous model

with all the features:

Accuracy increased from 0.8563 to 0.8582.
Precision increased from 0.8392 to 0.8397.
Recall increased from 0.9167 to 0.9202.
F1-Score increased from 0.8763 to 0.8781.

# brief interpretation of the ROC Curve:

An ROC AUC score of 0.91 is excellent! It indicates that the logistic regression model performs very well in distinguishing 

between the positive and negative classes.



ROC AUC Score (0.91): This value suggests that the model has a high level of discriminative ability. An AUC of 0.5 would 

indicate no discrimination (i.e., the model is no better than random guessing), while an AUC of 1.0 indicates perfect 

discrimination. With a score of 0.91, the model is quite effective at predicting the presence or absence of hypertension.

