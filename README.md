# insurance cost prediction 📊

This repository contains a machine learning project focused on predicting insurance charges based on individual health and demographic data. The project follows a complete pipeline from raw data to a trained predictive model.

## 🚀 Project Overview
The objective is to analyze the `insurance.csv` dataset and build a regression model that estimates insurance costs. This involves understanding data patterns, cleaning inconsistencies, and selecting the most relevant features for prediction.

## 📊 Dataset Features
The model utilizes several key attributes from the dataset:
* **age**: Age of the primary beneficiary.
* **sex**: Gender of the insurance contractor.
* **bmi**: Body Mass Index, used to assess weight relative to height.
* **children**: Number of children or dependents covered.
* **smoker**: Whether the individual is a smoker or not.
* **region**: The residential area in the US (Northeast, Northwest, Southeast, Southwest).
* **charges (Target)**: Individual medical costs billed by the insurance provider.

## 🛠️ Tech Stack
* **Language:** Python
* **Environment:** Google Colab
* **Key Libraries:** `pandas`, `numpy`, `seaborn`, `matplotlib`, `scikit-learn`, `scipy`

## 📈 Workflow
1. **Exploratory Data Analysis (EDA):** Performed distribution analysis using histplots and boxplots to identify outliers and correlations.
2. **Data Cleaning:** Removed duplicate records and handled categorical mapping.
3. **Feature Engineering:** * Created `bmi_category` to group BMI into Underweight, Normal, Overweight, and Obese.
    * Converted categorical variables into numerical values using One-Hot Encoding and Mapping.
4. **Feature Scaling:** Applied `StandardScaler` to normalize numerical features like age and BMI.
5. **Statistical Testing:** Used **Pearson Correlation** and **Chi-Square** tests to validate the relationship between features and the target variable.
6. **Modeling:** Trained a **Linear Regression** model to predict charges.
7. **Evaluation:** Assessed the model using $R^2$ and Adjusted $R^2$ scores.

## 📊 Results and Evaluation
After training the **Linear Regression** model, the performance was evaluated on the test set:
* **R² Score:** ~0.74 (The model explains 74% of the variance in insurance charges).
* **Adjusted R² Score:** ~0.73.

## 📝 How to Use
1. Clone this repository.
2. Upload the `insurance cost prediction.ipynb` file to Google Colab.
3. Ensure the `insurance.csv` dataset is available in your environment.
4. Run the cells sequentially to reproduce the analysis.
