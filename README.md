# Data Science - Prediction of Risk of Stroke for Individuals
##  Using machine learning to can assess the risk of stroke for individuals based on the data provided. 

**Author**: 
Mikhail Pillay
### Business problem:

**The business problem is to develop a predictive model that can assess the risk of stroke for individuals. Stroke is a critical and life-threatening medical condition, and early identification of individuals at a higher risk of stroke can lead to timely interventions and potentially life-saving measures.**

**Healthcare Providers: Hospitals, clinics, and healthcare professionals who can use the predictive model to identify patients at risk of stroke and provide appropriate medical care and interventions.**

**Individuals: People interested in understanding their own risk of stroke may also benefit from this predictive model.**


### Data:
This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient.
Stroke Dataset: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

For this dataset, there were 5110 rows and 11 columns.
Here is the Data Dictionary for this dataset:

**Attribute Information**
1) id: unique identifier
2) gender: "Male", "Female" or "Other"
3) age: age of the patient
4) hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6) ever_married: "No" or "Yes"
7) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8) Residence_type: "Rural" or "Urban"
9) avg_glucose_level: average glucose level in blood
10) bmi: body mass index
11) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
12) stroke: 1 if the patient had a stroke or 0 if not
*Note: "Unknown" in smoking_status means that the information is unavailable for this patient


## Visualization 1: Gender Distribution of Stroke Cases
![image](https://github.com/Mix1996/Project-2-Classification/assets/53317324/67553e23-ef5e-4454-8988-3d22bb229fa6)

The first visualization provides a clear overview of the distribution of stroke cases by gender. It shows two bars for each gender category: one for individuals who haven't had a stroke (labeled "No") and another for those who have had a stroke (labeled "Yes"). This visualization allows stakeholders to see if there are gender-related trends in stroke occurrence. For instance, it can help identify whether there is a significant difference in the number of stroke cases between genders. According to the data and visualisation, females are less likely to have a stroke compared to males.

## Visualization 2: Average Glucose Level vs. Age Scatter Plot
![image](https://github.com/Mix1996/Project-2-Classification/assets/53317324/e23b2dd5-1e34-4d79-b3ac-8b3c37615862)

The second visualization is a scatter plot that depicts the relationship between age and average glucose level for individuals in the dataset. Each point represents a person, and the colour indicates whether they've had a stroke (blue for "No" and orange for "Yes"). This visualization helps stakeholders understand the distribution of glucose levels across different age groups and whether there is any noticeable trend. According to the data and visualisation people between the age of 60-80 were more likely to have a stroke with an average glucose level above 150.


## Methods
**To prepare this data, the data was cleaned, and the following processes were performed:**
- Drop duplicates and fix inconsistencies in categorical data.
- Identify the features (X) and target (y)
- Perform a train test split
- Create a preprocessing object to prepare the dataset for Machine Learning
- Scale data
- Feature Engineering

**Maching Learning Using the Following Models:**
- Logistic Regression
- Random Forest Regressor Model
- Tuned/Best Random Forest Regressor Model
- Decision Tree Model
- Gradient Boosting
- Support Vector Classifier


## Results

Report the most important metrics

**Random Forest - Best Tuned Model Metrics:**
- Train Accuracy: 0.9711350293542075
- Test Accuracy: 0.9393346379647749
- Precision: 0.0
- Recall: 0.0
- F1 Score: 0.0
- ROC AUC: 0.5

**Gradient Boosting - Best Tuned Model Metrics:**
- Train Accuracy: 0.9542563600782779
- Test Accuracy: 0.9393346379647749
- Precision: 0.0
- Recall: 0.0
- F1 Score: 0.0
- ROC AUC: 0.5

**Support Vector Classifier - Best Tuned Model Metrics:**
- Train Accuracy: 0.9542563600782779
- Test Accuracy: 0.9393346379647749
- Precision: 0.0
- Recall: 0.0
- F1 Score: 0.0
- ROC AUC: 0.5

**Logistic Regression - Best Tuned Model Metrics:**
- Train Accuracy: 0.9545009784735812
- Test Accuracy: 0.9393346379647749
- Precision: 0.0
- Recall: 0.0
- F1 Score: 0.0
- ROC AUC: 0.5

**Decision Tree - Best Tuned Model Metrics:**
- Train Accuracy: 0.9659980430528375
- Test Accuracy: 0.9285714285714286
- Precision: 0.23809523809523808
- Recall: 0.08064516129032258
- F1 Score: 0.12048192771084337
- ROC AUC: 0.531989247311828

The Final Model Chosen was a Decision Tree.


## Recommendations:

Among the models you've evaluated, the Decision Tree model stands out as it shows better performance in terms of precision, recall, and F1 Score compared to the other models. Here's a summary of the Decision Tree's best-tuned model metrics:

**Decision Tree - Best Tuned Model Metrics:**
- Train Accuracy: 0.9659980430528375
- Test Accuracy: 0.9285714285714286
- Precision: 0.23809523809523808
- Recall: 0.08064516129032258
- F1 Score: 0.12048192771084337
- ROC AUC: 0.531989247311828

In conclusion, considering the balance between precision and recall, interpretability, and the potential for further refinement, the Decision Tree model is a reasonable choice as the final model for predicting stroke risk.

## Limitations & Next Steps

As always, it's important to consider factors beyond just the numerical metrics, such as model complexity, interpretability, and any domain-specific considerations that may influence your decision.
Collaboration between data scientists, healthcare professionals, and domain experts is key to the success of such healthcare AI initiatives.


### For further information


For any additional questions, please contact **mikhailpillay83@gmail.com**
