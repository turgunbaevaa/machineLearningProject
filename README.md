### Machine Learning Binary Classification Project

This project solves a **binary classification problem** using a dataset of **9,000 rows and 11 features** (numerical and categorical). The goal is to predict a binary target variable (`0` or `1`) through preprocessing, feature engineering, model building, and explainability techniques.

## Data Preprocessing

- Removed outliers in one step using a custom trimming function across all numeric columns.
- Normalized numeric features with **MinMaxScaler** to scale values between 0 and 1.
- Explored feature-target relationships with:
  - **Matrix boxplots** and **scatter plots** (`catplot`)
  - **Correlation matrix**
  - **T-tests** and **Chi-square tests** for feature relevance

---

## Feature Engineering

- Retained key features: `feature_1`, `feature_2`, `feature_3`, `feature_4`
- Removed weak features: `feature_5` to `feature_8`
- Converted `category_1` and `category_2` into numerical values using **Label Encoding**
- Created feature pairs (mean, sum, square, product), and selected the most correlated with the target

---

## Machine Learning Models

Implemented and evaluated the following models:

- **Decision Tree**
- **Random Forest**
- **Gradient Boosting**

Each model was assessed for:
- Accuracy
- Precision / Recall
- Visual performance evaluation

---

## Model Explainability

Used **SHAP** and **LIME** for model interpretability:

- Identified features with the most influence on predictions
- Justified decisions made by complex models
- Reduced model complexity by excluding less impactful features

---

## Business Use Case: Marketing Optimization

Using SHAP and LIME for business alignment (e.g., marketing agency):

- Found top conversion factors (e.g., **page views**, **discounts**)
- Identified the most effective channels (**Instagram** > Google)
- Understood why certain users don’t convert (e.g., **short session**, **no discount**)

**Applications:**
- Optimize marketing budget by removing ineffective channels
- Personalize ads based on feature influence
- Improve UX by targeting pain points

---

## Technologies Used

- `Python`
- `Pandas`, `NumPy`
- `Seaborn`, `Matplotlib`
- `Scikit-learn`
- `SHAP`, `LIME`
- `Jupyter Notebook`

---

## Conclusion

This project demonstrates the complete machine learning pipeline—from data cleaning to feature engineering, model evaluation, and explainability—with direct applications to business decision-making.


