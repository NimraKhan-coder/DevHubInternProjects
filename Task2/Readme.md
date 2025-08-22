# Heart Disease Prediction using Logistic Regression

This project uses the **UCI Heart Disease Dataset** to build a machine learning model that predicts the presence of heart disease.  
The implementation is done in **Python** using libraries such as Pandas, Seaborn, Matplotlib, and Scikit-learn.  

---

📂 Project Structure
- **Model.ipynb** → Jupyter Notebook with complete data preprocessing, visualization, and model training steps.
- **heart_disease_uci.csv** → Dataset file (not included in repo, download from UCI repository).

---

🚀 Steps Performed
1. **Data Loading & Exploration**
   - Loaded the UCI heart disease dataset using Pandas.
   - Explored data with `.head()`, `.info()`, `.describe()`.

2. Data Cleaning & Preprocessing
   - Handled missing values with **custom imputation functions** for columns like `thal`, `ca`, `slope`, `fbs`, `exang`.
   - Dropped irrelevant columns such as `id`.
   - Encoded categorical features into numeric form using **One-Hot Encoding**.
   - Converted categorical columns to proper datatypes.

3. Exploratory Data Analysis (EDA)
   - Visualized correlations using **heatmaps**.
   - Checked for missing values with Seaborn heatmaps.
   - Used boxplots to understand feature relationships with the target variable.

   Feature Engineering
   - Created dummy variables for categorical columns (`sex`, `cp`, `thal`, `slope`, etc.).
   - Concatenated them back into the main dataset.

5. Model Training
   - Split data into **training (80%)** and **testing (20%)** sets.
   - Used **Logistic Regression** as the model.
   - Trained the model using `fit()` on training data.

6. Model Evaluation
   - Generated predictions using the test set.
   - Calculated **accuracy score**.
   - Produced a **classification report** for detailed metrics.

---

 📊 Results
- Achieved an accuracy score of around **X%** (replace with your actual result).
- Classification report includes precision, recall, and F1-score.

---

🛠️ Technologies Used
- Python  
- Pandas  
- Numpy  
- Matplotlib  
- Seaborn  
- Scikit-learn  


