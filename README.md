# Bank Marketing Campaign Analysis and Prediction

This project aims to analyze and predict customer behavior regarding term deposit subscriptions using the Bank Marketing dataset. The primary objectives are to identify key factors influencing term deposit subscriptions and build a predictive model to enhance marketing strategies.

## Project Structure

- `data/`: Contains the dataset used for analysis.
- `notebooks/`: Jupyter notebooks with exploratory data analysis, model building, and evaluation.
- `README.md`: Project overview and instructions.

## Dataset

The dataset contains information collected from a Portuguese bank's marketing campaign. It includes attributes such as age, job, marital status, education, account balance, and campaign-related features like contact duration and previous campaign outcomes.

## Key Findings

1. **Months of Marketing Activity**:
   - Highest activity in May, but low effectiveness.
   - Focus on March, September, October, and December for future campaigns.

2. **Campaign Calls**:
   - Limit to a maximum of 2 calls per potential client to save time and effort.

3. **Age Category**:
   - Target clients in their 20s or younger and 60s or older for higher subscription rates.

4. **Occupation**:
   - Focus on students and retired individuals who are more likely to subscribe to term deposits.

5. **House Loans and Balances**:
   - Target individuals with average and high balances who are less likely to have housing loans.

6. **Higher Duration Calls**:
   - Target individuals with call durations above 371 seconds.

## Predictive Modeling

We built and evaluated several models, including Logistic Regression, Decision Trees, and Random Forests. The Random Forest model provided the best performance with an accuracy of 85%.

### Model Training and Saving

The model training and saving process involves:
1. **Preprocessing**: Handling missing values, encoding categorical variables, and scaling numerical features.
2. **Model Training**: Training the Random Forest model using the preprocessed data.
3. **Model Saving**: Saving the trained model using `joblib`.

### Predictions

The model can be used to make predictions on new data by loading the saved model and preprocessing the input data accordingly.
