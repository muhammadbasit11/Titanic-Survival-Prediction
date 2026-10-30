# 🚢 Titanic Survival Prediction

## 📌 Project Overview

This project explores the application of Machine Learning classification algorithms to predict whether a passenger survived the Titanic disaster.

Using the Titanic passenger dataset, I performed data exploration, preprocessing, visualization, model training, and performance evaluation.

The primary objective was to compare three tree-based classification algorithms and understand how their predictive performance differs.

## 🎯 Objectives

- Understand and explore the Titanic dataset.
- Perform data cleaning and preprocessing.
- Conduct Exploratory Data Analysis (EDA).
- Visualize survival patterns and passenger characteristics.
- Train multiple classification models.
- Evaluate and compare model performance.

## 📂 Dataset Information

The dataset contains **887 passenger records and 8 columns**.

| Feature | Description |
|---|---|
| Survived | Target variable (0 = No, 1 = Yes) |
| Pclass | Passenger class |
| Name | Passenger name |
| Sex | Passenger gender |
| Age | Passenger age |
| Siblings/Spouses Aboard | Family members aboard |
| Parents/Children Aboard | Family members aboard |
| Fare | Ticket fare |

## 🛠️ Technologies & Libraries

- Python
- Pandas
- Seaborn
- Matplotlib
- Scikit-learn

## 🔍 Project Workflow

### 1. Data Loading and Exploration
- Loaded the dataset using Pandas.
- Examined dataset dimensions and initial observations.
- Inspected column information.
- Checked for missing values.

### 2. Data Preprocessing
- Encoded the `Sex` column:
  - Male → 1
  - Female → 2
- Removed the `Name` column from the predictive features.
- Separated independent variables (X) and the target variable (y).

### 3. Exploratory Data Analysis (EDA)

Created visualizations to investigate:

- Overall survival distribution.
- Survival count by gender.
- Age distribution.
- Fare distribution.

### 4. Train-Test Split

Split the dataset into training and testing subsets:

- Training: 80%
- Testing: 20%
- Random state: 42

### 5. Model Development

Implemented and evaluated three classification algorithms:

**Decision Tree Classifier**
- Used as a baseline classification model.

**Random Forest Classifier**
- Applied an ensemble of decision trees.

**Gradient Boosting Classifier**
- Applied sequential boosting to improve predictive performance.

## 📊 Model Performance Comparison

The following results were obtained from the test dataset:

| Model | Accuracy |
|---|---:|
| Decision Tree | 72% |
| Random Forest | 76% |
| Gradient Boosting | 81% |

### Classification Report Summary

**Gradient Boosting Classifier**

| Metric | Class 0 | Class 1 |
|---|---:|---:|
| Precision | 0.84 | 0.75 |
| Recall | 0.86 | 0.73 |
| F1-score | 0.85 | 0.74 |

Weighted average F1-score: **0.81**

## 🏆 Key Findings

- Decision Tree achieved 72% accuracy.
- Random Forest improved accuracy to 76%.
- Gradient Boosting achieved the highest accuracy at 81%.
- Gradient Boosting also produced the strongest overall weighted F1-score among the three models.

In this experiment, Gradient Boosting performed better than the other two evaluated classifiers.

## 💡 Key Learnings

Through this project, I strengthened my understanding of:

- Data exploration and preprocessing.
- Feature encoding.
- Exploratory Data Analysis.
- Classification algorithms.
- Ensemble learning.
- Model evaluation using precision, recall, F1-score, and accuracy.
- Comparing multiple models on the same dataset.

## 🚀 Future Improvements

Potential next steps include:

- Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
- Confusion matrix visualization.
- Feature importance analysis.
- Cross-validation.
- Exploring additional ensemble algorithms, including AdaBoost.
- Improving feature engineering and evaluating generalization.

## 📁 How to Run the Project

1. Clone this repository:

   ```bash
   git clone YOUR_REPOSITORY_URL
   ```

2. Navigate to the project directory:

   ```bash
   cd titanic-survival-prediction
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Open the notebook:

   ```bash
   jupyter notebook Titanic_Survival_Prediction.ipynb
   ```

5. Ensure `titanic.csv` is in the project directory.

## 👨‍💻 Author

Machine Learning and Data Science enthusiast, continuously learning through hands-on projects and practical implementation.

**Learning by building. Improving through experimentation. Growing one project at a time.** 🚀