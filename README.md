
# Telecom Churn Analysis EDA

## Business Understanding & Overview
In the telecom world, customer retention is crucial. When customers leave, it's called churn. Exploratory Data Analysis (EDA) helps in understanding why customers might be leaving. This analysis involves digging into customer data to spot patterns and clues about churn reasons.

## Objectives
1. Data Understanding**: Understand the shape, size, and contents of the dataset.
2. Churn Identification**: Count the number of churned and retained customers.
3. Feature Exploration**: Explore various customer attributes such as usage, tenure, demographics, etc.
4. Visualization and Analysis**: Use charts and graphs to identify patterns and differences between churned and retained customers.
5. Correlation Analysis**: Determine if there are connections between customer attributes and churn.

## Handling Missing Data
By Dropping the column
By imputing the mean() or medoan() values

### Findings
- One column (TotalCharges) has 0.15% missing values; the rest of the columns do not have any missing values.
- TotalCharges has the minimum missing values, so one approach is to handle it by dropping the column. Another approach is to impute the missing values using the mean() or median().

## Dropping Unnecessary Columns


- After analyzing the dataframe, we identified four numerical columns: SeniorCitizen, Tenure, MonthlyCharges, and TotalCharges.
- Although SeniorCitizen appears numerical, it is treated as categorical due to its values being 0 and 1.
- Unnecessary columns such as CustomerID and Tenure will be dropped.
- After removing these columns, all remaining columns are categorical except for MonthlyCharges and TotalCharges.


  ##### Categorical Univariate Analysis

#### 1. Churn with Gender and Senior Citizens
- Plot the churn rate for each gender category.
- Plot the churn rate for senior citizens versus non-senior citizens.

#### 2. Churn VS PhoneService
- Analyze the churn rate based on whether customers have phone service or not.

#### 3. Churn with Partner & without Partner
- Compare the churn rate for customers with and without partners.

#### 4. Dependents vs non-Dependent
- Investigate the churn rate for customers with and without dependents.

#### 5. MultiLines vs Churn and OnlineBackup Vs Churn
- Explore the relationship between having multiple lines and churn.
- Analyze how the availability of online backup services affects churn.

#### 6. Online Security vs Churn and DeviceProtection Vs Churn
- Examine the impact of online security services on churn.
- Investigate how the provision of device protection services affects churn.

#### 7. StreamingTV VS Churn and TechSupport VS Churn
- Analyze the churn rate based on the availability of streaming TV services.
- Explore the relationship between tech support availability and churn.

#### 8. Contract vs Churn and Paperlessbilling VS Churn
- Investigate the churn rate based on different contract types.
- Analyze the churn rate for customers with paperless billing versus traditional billing.

#### 9. PaymentMethod Vs Churn & Tenure_group VS Churn
- Examine how payment method choice impacts churn.
- Explore the churn rate based on tenure groups.

## Numerical Univariate Analysis

### Churn Analysis with MonthlyCharges
- Analyze the distribution of monthly charges for churned and retained customers.
- Plot histograms or kernel density estimates to visualize the distribution of monthly charges for both churned and retained customers.
- Calculate summary statistics such as mean, median, and standard deviation for monthly charges in both groups.

### Churn Analysis with TotalCharges
- Conduct a similar analysis as with MonthlyCharges, but this time focusing on the total charges.
- Visualize the distribution of total charges for churned and retained customers.
- Calculate summary statistics for total charges in both groups.


## Bivariate Analysis

### Distribution of Gender and Partner for Churned and Non-Churned Customers
- Analyze the relationship between gender and partner status for churned and non-churned customers.
- Visualize the distribution of churned and non-churned customers based on their gender and partner status.

### Distribution of Gender and PaymentMethod for Churned and Non-Churned Customers
- Investigate the relationship between gender and payment method for churned and non-churned customers.
- Visualize the distribution of churned and non-churned customers based on their gender and payment method.

### Distribution of Gender and TechSupport for Churned and Non-Churned Customers
- Explore the relationship between gender and tech support availability for churned and non-churned customers.
- Visualize the distribution of churned and non-churned customers based on their gender and tech support status.

### Distribution of Gender and SeniorCitizen for Churned and Non-Churned Customers
- Analyze the distribution of churned and non-churned customers based on their gender and senior citizen status.
- Visualize the relationship between gender and senior citizen status for churned and non-churned customers.

##Next Steps:
Using this Data creating some Machine Learning Models

