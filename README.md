# 🚢 Titanic - Machine Learning from Disaster

### 📌 Project Overview
This project predicts passenger survival on the Titanic using **Logistic Regression**. The goal is to analyze passenger data (age, gender, class, etc.) to build a model that predicts who survived the tragedy.

### 📊 Key Insights (EDA)
- **Gender:** Females had a significantly higher survival rate than males.
- **Class:** First-class passengers were prioritized and had better survival odds.
- **Feature Engineering:** Extracted 'Titles' (Mr, Mrs, Miss, etc.) from names, which proved to be a strong predictor of social status and survival.

### 🛠️ Methodology
1. **Data Cleaning:** Handled missing values in `Age` using Title-based median imputation.
2. **Feature Engineering:** - Created `Family_size` by combining `SibSp` and `Parch`.
   - Extracted `Title` from the `Name` column.
3. **Preprocessing:** - Applied **One-Hot Encoding** for categorical variables (`Sex`, `Embarked`, `Title`).
   - Performed **Standard Scaling** on numerical features (`Age`, `Fare`, `Family_size`).
4. **Model:** Logistic Regression with `random_state=42`.

### 📈 Results
- **Accuracy:** 80.4% on the validation set.
- **ROC-AUC Score:** (.87)
- **Key Predictors:** Gender (Male), Passenger Class (Pclass), and Fare were the most influential features.

### 🚀 How to Run
1. Clone the repo: `git clone https://github.com/Omnia-Elsaka10/Titanic-Survival-Prediction-LogisticRegression.git`
2. Install dependencies: `pip install pandas numpy seaborn matplotlib scikit-learn`
3. Run the notebook `notebooks/Titanic_Analysis_LR.ipynb`.
