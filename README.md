# Heart-Disease-Predicting-Model
Listen to your heart
## Overview
This Heart Disease Prediction Model is a machine learning tool that utilizes patient data to predict the likelihood of a patient having heart disease. Using logistic regression, a statistical method for analyzing a dataset in which there are one or more independent variables that determine an outcome, this model is trained to identify patterns that lead to heart conditions.
## How the Model Works
The model is built upon a logistic regression algorithm, which is a classification algorithm traditionally used for binary classification problems — in this case, determining whether a patient has heart disease or not.
## Dataset
The dataset used for training the model includes several medical attributes that are known to be risk factors for heart diseases. Below is the description of the dataset attributes:
| Variable Name | Description                                             | Sample Data   |
|---------------|---------------------------------------------------------|---------------|
| Age           | Patient age (in years)                                  | 63; 37; ...   |
| Sex           | Gender of patient (0 = male; 1 = female)                | 1; 0; ...     |
| cp            | Chest pain type (0 = typical angina; 1 = atypical angina; 2 = non-anginal pain; 3 = asymptomatic) | 3; 1; 2; ... |
| trestbps      | Resting blood pressure (in mm Hg)                       | 145; 130; ... |
| chol          | Serum cholesterol (in mg/dl)                            | 233; 250; ... |
| fbs           | Fasting blood sugar > 120 mg/dl (0 = false; 1 = true)   | 1; 0; ...     |
| restecg       | Resting electrocardiographic results (0 = normal; 1 = having ST-T wave abnormality; 2 = showing probable or definite left ventricular hypertrophy by Estes' criteria) | 0; 1; ...   |
| thalach       | Maximum heart rate achieved                             | 150; 187; ... |
| exang         | Exercise induced angina (0 = no; 1 = yes)               | 1; 0; ...     |
| oldpeak       | ST depression induced by exercise relative to rest      | 2.3; 3.5; ... |
| slope         | The slope of the peak exercise ST segment (0 = upsloping; 1 = flat; 2 = downsloping) | 0; 2; ...   |
| ca            | Number of major vessels (0-4) colored by fluoroscopy    | 0; 3; ...     |
| thal          | Thalassemia (3 = normal; 6 = fixed defect; 7 = reversible defect) | 1; 3; ...   |
| Target        | Target column (0 = no heart disease; 1 = have heart disease) | 1; 0; ...   |


## Installation
To run this model, you will need Python installed on your system, along with the following libraries:

pandas
numpy
sklearn
You can install these packages using pip:
 ### pip install pandas numpy scikit-learn

## Usage
The model can be utilized by running the provided Python script or Jupyter notebook. You will need to input the patient data in the form of a feature array to receive a prediction.
# Example of making a prediction
```python
input_data = (63, 1, 3, 145, 233, 1, 0, 150, 0, 2.3, 0, 0, 1)
prediction = model.predict(input_data)
print(f"The prediction for the input data is: {'Heart Disease' if prediction[0] == 1 else 'No Heart Disease'}")


### Model Training and Evaluation
The model was trained on 80% of the provided dataset and evaluated on the remaining 20%. The accuracy on the training data was found to be 85% accurate, and the accuracy on the test data was 81% accurate.
