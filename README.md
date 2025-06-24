# titanic_survival_prediction
# Titanic Survival Prediction 🚢

This project uses machine learning to predict whether a passenger survived the Titanic shipwreck based on features like age, gender, class, and family information.

## 📌 Project Objective

To analyze the Titanic dataset and build predictive models that can estimate the likelihood of survival for a given passenger using classification algorithms.

## 📁 Dataset

- **Source**: [Kaggle Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic)
- **Features** used:
  - `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
  - `Sex`: Gender of the passenger
  - `Age`: Age in years
  - `SibSp`: Number of siblings / spouses aboard
  - `Parch`: Number of parents / children aboard
  - `Fare`: Passenger fare

## 🧹 Data Preprocessing

- Handled missing values (e.g., in `Age`)
- Encoded categorical variables like `Sex`
- Scaled numerical features for better performance
- Dropped less important columns like `Embarked`, `Cabin`, and `Name` for simplicity

## 🤖 Models Used

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- Support Vector Machine (SVM)

## 🧪 Evaluation Metrics

- Accuracy Score
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)

## ✅ Best Model

- Achieved **~81.56% accuracy** with [insert model name here, e.g., Random Forest].

## 📊 Confusion Matrix & Report

```python
from sklearn.metrics import confusion_matrix, classification_report

# After predicting
confusion_matrix(y_test, predictions)
classification_report(y_test, predictions)
