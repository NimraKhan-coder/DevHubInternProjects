# 🏡 House Price Prediction using Machine Learning

This project demonstrates how to predict **house prices** using Python and machine learning techniques.  
The notebook includes **data preprocessing, exploratory analysis, feature engineering, and model training**.

---

## 📌 Project Workflow

1. **Importing Libraries**
   - Used `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`.

2. **Loading the Dataset**
   - Imported the housing dataset into a pandas DataFrame.

3. **Exploratory Data Analysis (EDA)**
   - Checked dataset shape, data types, and null values.
   - Visualized correlations between features (heatmap, scatter plots).
   - Used boxplots and histograms to analyze distributions and detect outliers.

4. **Data Cleaning & Preprocessing**
   - Handled missing values by imputation (mean/median/mode).
   - Converted categorical features into numeric using **One-Hot Encoding**.
   - Normalized/standardized numerical features.

5. **Feature Engineering**
   - Selected important predictors of house prices.
   - Removed unnecessary/irrelevant columns.

6. **Model Training**
   - Split dataset into training and testing sets.
   - Trained different regression models:
     - **Linear Regression**
     - **Random Forest Regressor**
     - **Decision Tree Regressor**
     - (optionally XGBoost, if included)

7. **Model Evaluation**
   - Evaluated models using:
     - **R² Score**
     - **Mean Absolute Error (MAE)**
     - **Root Mean Squared Error (RMSE)**
   - Compared performance of models.


```bash
pip install pandas numpy matplotlib seaborn scikit-learn
