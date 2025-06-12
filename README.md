# Task-1-Predict-Employee-Attrition-

**DATASET:** IBM HR Analytics Dataset

# **Code Explanation:**
**1. Import Libraries & Dataset**
- Uploaded and loaded WA_Fn-UseC_-HR-Employee-Attrition.csv using Pandas.
- Used libraries: pandas, numpy, matplotlib, seaborn, sklearn, shap, lime.

**2. Exploratory Data Analysis (EDA)**
- Converted Attrition to binary (Yes → 1, No → 0).

- Visualized attrition distribution by job roles.

- Created correlation heatmap to identify key influencing features.

**3. Data Preprocessing**
- One-hot encoded categorical features.

- Separated features (X) and target (Attrition_Yes) as y.

- Split into training and testing sets (80/20 split).

- Model Training
  
**4. Trained two models:**
- Random Forest Classifier

- Logistic Regression

- Evaluated using classification report (Precision, Recall, F1-Score).

**5. Model Evaluation:**
1. Random Forest:

- High overall accuracy (88%)

- Low recall for attrition class due to class imbalance

2. Logistic Regression:

- Accuracy: 87%

- Better recall than RF but still impacted by imbalance

**6. Explainability – SHAP & LIME**
1. SHAP: Visualized global feature importance.

2. LIME: Interpreted individual predictions with top 10 influencing features.

**7. Actionable Insights:**
- Top Factors: MonthlyIncome, OverTime, Age, TotalWorkingYears, DistanceFromHome.

**8. HR Recommendations:**

- Reduce overtime workload

- Offer competitive compensation

- Retain younger talent through growth programs

# **How to Run the Code**
**1. Upload CSV File:**

from google.colab import files  
uploaded = files.upload()

**2. Install SHAP & LIME :**

!pip install shap lime

**3. Run the Notebook in Order:**

1. Load and explore the dataset

2. Preprocess data and train models

3. Evaluate and explain predictions

4. Review insights for HR strategy

# **Observation**
1. Attrition prediction is challenging due to class imbalance.

2. Random Forest performs well but needs better recall.

3. SHAP and LIME help build trust and explainability in HR decisions.

4. Actionable insights can guide real-world employee retention strategies.
