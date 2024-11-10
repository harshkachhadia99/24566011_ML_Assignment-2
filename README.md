# 24566011_ML_Assignment-2

# Assignment 2 - DAC-501 Machine Learning Course 

## How to run assignment/project :
Step-1 : Download .ipynb file <br>
Step-2 : Download .csv file <br>
Step-3 : Open .ipynb file using local machine(jupyter notebook) or google colab. <br>
Step-4 : In "df=pd.read_csv()" cell, copy path of .csv file downloaded and paste it to that cell as shown here : <br> 
<div align="center">
df=pd.read_csv("path_to_.csv_file_downloaded")
</div>  <br>
Step-5 : Now you can run code. <br>

## Overview of the assignment
# Predictive Model for Restaurant Tip Estimation

This project develops a predictive model to estimate tip amounts in restaurants based on customer billing and demographic details. Using various regression techniques, the goal is to help restaurants understand tipping behavior better and optimize service and revenue strategies.

## Project Objectives

1. **Identify Key Factors**: Determine which features (e.g., total bill, party size, customer demographics) significantly impact tip amounts.
2. **Build Accurate Models**: Use multiple regression techniques to forecast tip amounts effectively and evaluate prediction accuracy.
3. **Provide Management Insights**: Offer actionable recommendations to improve customer service strategies and revenue management.

The dataset includes customer billing and demographic details such as total bill, tip, size of the party, time of dining (Lunch/Dinner), and other relevant features.

## Analysis & Methodology

### Step 1: Model Selection & Evaluation

The project utilizes several regression techniques to predict tip amounts, including:

1. **Linear Regression**
2. **Ridge Regression**
3. **Lasso Regression**
4. **Decision Tree Regression**
5. **Random Forest Regression** (Ensemble Method)
6. **Support Vector Regression (SVR)**
7. **K-Nearest Neighbors (KNN)**

GridSearchCV is performed on above models for hyperparameter tuning.
Each model is evaluated for prediction accuracy using metrics like **R² score**, **Mean Squared Error (MSE)**, **Root Mean Squared Error (RMSE)**, and **Mean Absolute Error (MAE)**.

### Step 2: Feature Significance & Insights for Management

- **Key Features**: Identify which features have the highest impact on tipping behavior.
- **Management Recommendations**: Provide actionable insights to improve customer service and optimize revenue, such as implementing tipping options in digital payments, upselling popular items, and designing seating arrangements based on party size.

### Step 3: Check if the data follows a linear trend using following methods to analyze the relationship between the target variable(tip) and predictors. 

- **Scatter Plot**: Visualize individual feature relationships with the target variable (tip).
- **Pair Plot**: Explore feature correlations with the target variable across multiple features.
- **Correlation Matrix (Heatmap)**: Identify significant correlations between predictors and the target variable.
- **Statistical Tests (Rainbow Test)**: Check for linearity in relationships between predictors and the target.
- **Residuals Plot**: Analyze the residuals to assess model fit and error distribution.
- **Line Plot (for Time-Series)**: If applicable, check the target variable’s trend over time (e.g., dining time such as Lunch or Dinner).

### Step 4 : Based on above plots, tests and trends in data apply suitable regression method and check model prediction accuracy. 

## Getting Started
## Tools and Libraries Used: 
To run the code, you’ll need the following Python packages:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `statsmodels`

### Numerical variables in .csv file are : total_bill, tip, size.
### Categorical variables in .csv file are : sex, smoker, day, time. These categorical variables are encoded to numerical variables which gives rise to new features.
### 'tip' variable is the target variable.

### Features in the Dataset (after encoding categorical to numerical):
1. **total_bill**: The total amount billed to the customer in dollars, representing the entire cost of the meal, including any additional charges.
2. **size**: The number of people in the dining party, indicating the size of the group.
3. **time_Lunch**: Indicates whether the meal occurred during lunch hours (1 if lunch, 0 if otherwise).
4. **sex_Male**: Encodes the customer's gender (1 if male, 0 if female).
5. **day_Sun, day_Thur, day_Sat**: Binary indicators for the day of the week on which the customer dined (1 if the respective day, 0 if not).
6. **smoker_Yes**: Indicates if the customer is a smoker (1 if yes, 0 if no).

### **Insights for management :**
Based on above steps performed, we acknowleged the importance of features like 'total_bill' and 'size' (number of diners) impacting tip amounts, here are some actionable insights for management to improve customer service strategies and optimize revenue management:

### **1. Suggest More Menu Items**
Since bigger bills lead to better tips, encourage servers to suggest extra items like appetizers, desserts, or special drinks. This makes the meal more enjoyable and can lead to higher spending and tips.

### **2. Assign Experienced Servers to Larger Groups**
Bigger groups usually mean bigger bills and tips, so assign them to experienced servers who can handle larger tables well. This makes service smoother and can increase customer satisfaction.
Consider offering bundled menu options or group discounts to encourage larger groups.

### **3. Offer Group Deals**
Since larger groups contribute positively to tipping, consider promoting discounts or loyalty points for groups dining together. Group discounts for certain days (like weekdays) can attract more diners during slower times, optimizing restaurant capacity and increasing average table size.

### **4. Introduce Digital Payment Options with Suggested Tip Percentages**
Make tipping easier by adding tip suggestions on digital payment screens (like 15%, 18%, or 20%). This makes tipping convenient, transparent and can encourage customers to tip more.

## Conclusion:
### **So, we can conclude that 'total_bill' and 'size' are the most significant features that impacts tip amounts.**

**Author**: Kachhadia Harsh Nagjibhai - 24566011
