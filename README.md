# Loan Approval Prediction (Supervised Learning)

Hey there! Welcome to my project. In this repository, I built an end-to-end Machine Learning pipeline to predict whether a loan application will get approved or rejected based on historical customer finance data. 

I built this project completely from scratch to get hands-on experience handling real-world data constraints, missing data imputation, and model pipelines.

## 🚀 Project Overview
When people apply for a loan, financial institutions manually check profiles to evaluate the risk of default. This project automates that process. Using customer background details (like income, credit history, education, and marital status), the model learns patterns to predict loan eligibility (`Loan_Status` - Yes/No).

# Loan Approval Prediction (Supervised Learning)

Hey there! Welcome to my project. In this repository, I built an end-to-end Machine Learning pipeline to predict whether a loan application will get approved or rejected based on historical customer finance data. 

I built this project completely from scratch to get hands-on experience handling real-world data constraints, missing data imputation, and model pipelines.

## 🚀 Project Overview
When people apply for a loan, financial institutions manually check profiles to evaluate the risk of default. This project automates that process. Using customer background details (like income, credit history, education, and marital status), the model learns patterns to predict loan eligibility (`Loan_Status` - Yes/No).

## 🛠️ What's Inside the Code?
Here is the step-by-step workflow I followed in the Jupyter Notebook:
1. Data Gathering: Loaded the dataset (`Finance.csv`) and analyzed missing data points.
2. Data Imputation:
   * Used Mode to fill missing categorical values (Gender, Married, Dependents, Self_Employed, and Credit History).
   * Used Median to fill missing numerical parameters (Loan Amount and Loan Amount Term).
3. Data Preprocessing & Pipelines: Built a robust data pipeline using Scikit-Learn's `ColumnTransformer`.
   * Applied OneHotEncoder to nominal categories.
   * Applied OrdinalEncoder to ordered categories (like Education).
   * Standardized numerical features using StandardScaler.
4. Model Training & Evaluation: Split the data (70% train, 30% test) and compared two different classification algorithms:
   * Logistic Regression
   * Random Forest Classifier

## 📊 Performance & Insights
The models gave me the following test results:
* Logistic Regression achieved a higher testing accuracy of ~65.4% and an incredible recall of ~99.1%.
* Random Forest Classifier landed around ~61% accuracy.

*(Fun fact: I also experimented with Feature Importance for the Random Forest model to see exactly which customer attributes play the biggest role in getting a loan approved!)*

## 📦 Setup & How to Run
If you want to run this notebook locally on your machine, follow these steps:

1. Clone this repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
   cd YOUR_REPO_NAME