# 🏡 House Prices Prediction – Advanced Regression

A machine learning project to predict residential house prices in **Ames, Iowa** using advanced regression and ensemble learning techniques.  
This project is based on the popular **Kaggle House Prices** dataset and focuses on proper preprocessing, model evaluation, and ensemble methods.

---

## 📁 Project Structure

- **Data**
  - `train.csv` – Training dataset with **81 features** and **1460 samples**
  - `test.csv` – Test dataset used for Kaggle submission

- **Notebook**
  - `house-prices-advanced-regression-techniques.ipynb`  
    Complete end-to-end workflow including EDA, preprocessing, modeling, and evaluation

---

## 🚀 Project Workflow

### 1️⃣ Data Exploration
- Loaded and explored the dataset
- Analyzed feature distributions and correlations
- Identified missing values and potential outliers
- Studied target variable (`SalePrice`) distribution

---

### 2️⃣ Data Preprocessing
- Handled missing values using appropriate imputation strategies
- Encoded categorical variables:
  - One-Hot Encoding
  - Ordinal Encoding (where applicable)
- Scaled numerical features
- Built reusable **scikit-learn pipelines** to prevent data leakage

---

### 3️⃣ Modeling
Multiple regression models were trained and evaluated:

#### 🔹 Linear Models
- Linear Regression  
- Ridge Regression  
- Lasso Regression  
- ElasticNet  

#### 🌲 Tree-Based Models
- Decision Tree Regressor  
- Random Forest Regressor  

#### ⚡ Ensemble Methods
- Gradient Boosting Regressor  
- AdaBoost Regressor  
- Voting Regressor  
- Stacking Regressor  

✔️ Used **cross-validation** and **hyperparameter tuning**  
✔️ Target variable was **log-transformed** to optimize RMSLE (Kaggle metric)

---

### 4️⃣ Key Insights
- **OverallQual** and **GrLivArea** are the strongest predictors of house prices
- Ensemble models significantly outperform individual models
- Gradient Boosting showed the most consistent performance
- Proper feature engineering and preprocessing greatly improved accuracy

---

## 📊 Results
- **Best Model:** Gradient Boosting Regressor (within ensemble framework)
- Achieved a **competitive RMSLE score** on Kaggle leaderboard
- Feature importance analysis provided meaningful, interpretable insights
- Model generalized well without data leakage

---

## 🛠️ Tech Stack

- **Programming Language:** Python  
- **Libraries:**  
  - pandas, numpy  
  - matplotlib, seaborn  
  - scikit-learn (preprocessing, models, pipelines)
- **Environment:** Jupyter Notebook  

---

## 📈 How to Run the Project

1. Clone the repository
   ```bash
   git clone <repository-url>
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook
   ```bash
   jupyter notebook house-prices-advanced-regression-techniques.ipynb
   ```

4. Run all cells sequentially

---

## 🏁 Kaggle Submission
- Predictions were generated on the Kaggle test dataset
- Final submission followed Kaggle’s required format:
  ```csv
  Id,SalePrice
  ```

---

## 📌 Future Improvements
- Advanced feature interactions
- Bayesian hyperparameter optimization
- LightGBM / CatBoost integration
- Blending multiple stacked models

---

⭐ **If you find this project useful, consider giving it a star!**
