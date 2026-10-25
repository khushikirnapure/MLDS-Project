# ATM Cash Demand Prediction Using Machine Learning

## Project Overview

ATM Cash Demand Prediction is a Machine Learning and Data Science project that predicts the amount of cash required by an ATM for the next day. It uses historical ATM transaction data and other relevant factors to estimate future cash demand.

The project aims to help banks plan ATM cash replenishment more efficiently, reduce cash shortages, and avoid unnecessary cash loading.

## Objectives

- Predict next-day ATM cash demand.
- Analyze factors affecting ATM cash requirements.
- Perform data preprocessing and exploratory data analysis.
- Apply and compare different Machine Learning algorithms.
- Evaluate model performance using appropriate metrics.
- Explore clustering techniques to identify patterns in ATM cash demand.

## Dataset

**Dataset file:** `atm_cash_management_dataset.csv`

The notebook expects the dataset to contain the following columns:

- `Total_Withdrawals`
- `Total_Deposits`
- `Holiday_Flag`
- `Special_Event_Flag`
- `Previous_Day_Cash_Level`
- `Nearby_Competitor_ATMs`
- `Cash_Demand_Next_Day` — target variable

The target variable represents the next day's required cash demand.

*Note: The dataset must be added separately to the repository if sharing is permitted. Confirm that its column names match the notebook.*

## Technologies Used

- **Programming Language:** Python
- **Environment:** Google Colab / Jupyter Notebook
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Model Saving:** Joblib

## Project Workflow

1. Load the ATM cash management dataset.
2. Explore dataset structure, column types, and summary statistics.
3. Handle missing values using median and mode imputation.
4. Convert categorical variables into numerical features using one-hot encoding.
5. Split the dataset into training and testing sets.
6. Train and evaluate different Machine Learning models.
7. Compare model performance using evaluation metrics.
8. Apply clustering techniques to explore patterns in ATM activity.
9. Perform cross-validation and hyperparameter tuning.

## Algorithms Implemented

### Regression
- Simple Linear Regression
- Multiple Linear Regression
- Decision Tree Regression
- Bagging Regression
- Random Forest Regression

### Classification
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes

### Clustering
- K-Means Clustering
- Gaussian Mixture Model (GMM)

### Model Optimization
- 5-fold cross-validation
- GridSearchCV for hyperparameter tuning

## Evaluation Metrics

The regression models are evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score
- Mean Absolute Percentage Error (MAPE)

The classification models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

## How to Run the Project

### Option 1: Google Colab

1. Open the notebook `MLDS_PROJECT_.ipynb` in Google Colab.
2. Upload `atm_cash_management_dataset.csv` when prompted.
3. Run the notebook cells sequentially.
4. View the model evaluation results and visualizations.

### Option 2: Run Locally

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

Place the notebook and dataset in the same folder. Open the notebook in Jupyter Notebook and run the cells sequentially.

## Expected Outcome

The project compares different Machine Learning approaches for estimating next-day ATM cash demand. The evaluation metrics help identify promising regression models, while clustering techniques provide additional insights into ATM activity patterns.

The predictions can support better cash replenishment planning. Actual replenishment timing would require additional information such as current cash balance, ATM capacity, delivery lead time, and replenishment schedules.

## Future Scope

- Integrate real-time ATM transaction data.
- Predict the date and time when cash replenishment will be required.
- Include bank-specific and location-specific demand patterns.
- Develop a dashboard for visualizing cash demand predictions.
- Deploy the best-performing model through a web application.

## Project Structure

```text
MLDS-Project/
├── MLDS_PROJECT_.ipynb
├── atm_cash_management_dataset.csv
└── README.md
```

## Contributors

Add the names of all project team members here.

- Khushi Kirnapure
- Gauri Gadewar
- Palak Kharabe

## Conclusion

This project demonstrates the use of Machine Learning and Data Science techniques to analyze ATM cash management data and predict next-day cash requirements. It provides a foundation for improving cash availability and making ATM replenishment planning more data-driven.


