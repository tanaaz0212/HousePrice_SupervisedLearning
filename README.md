# House Price Prediction Using Supervised Machine Learning

## Project Overview

This project focuses on predicting house prices using supervised machine learning regression techniques.

The model uses the Ames Housing dataset to estimate the sale price of residential properties based on various features such as living area, neighborhood, building type, overall quality, and other property characteristics.

The main objective is to understand and implement the complete machine learning workflow, including data exploration, preprocessing, model training, evaluation, and model saving.

## Problem Statement

House prices depend on several factors, including property size, location, quality, and construction characteristics.

The goal of this project is to develop a machine learning model that can learn from historical housing data and predict house sale prices based on the available features.

## Dataset

- **Dataset:** Ames Housing Dataset
- **File Name:** `train.csv`
- **Target Variable:** `SalePrice`
- **Problem Type:** Regression

The dataset contains information about residential properties, including numerical and categorical features.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Joblib

## Project Workflow

The project follows these major steps:

1. Data Loading
2. Data Understanding and Exploration
3. Exploratory Data Analysis (EDA)
4. Data Cleaning and Preprocessing
5. Feature Engineering
6. Model Training
7. Model Evaluation
8. Model Comparison
9. Residual Analysis
10. Saving the Trained Model

## Machine Learning Models

The following regression algorithms were explored:

- Linear Regression
- Ridge Regression
- Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor

The models were evaluated and compared using regression performance metrics to identify a suitable model for house price prediction.

## Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the dataset and identify patterns in house prices.

The analysis included:

- Distribution of house sale prices
- Relationship between living area and sale price
- Correlation between numerical features
- Analysis of categorical features such as Neighborhood, BldgType, and HouseStyle
- Identification of important features affecting house prices

## Model Evaluation

The model performance was evaluated using the following regression metrics:

| Evaluation Metric | Result |
|---|---:|
| R² Score | 0.9323 |
| R² Score (Percentage) | 93.23% |
| Mean Absolute Error (MAE) | 15,084.88 |
| Root Mean Squared Error (RMSE) | 22,793.84 |

### Interpretation

The R² score of 0.9323 indicates that the evaluated model explains approximately 93.23% of the variation in house sale prices on the evaluation dataset.

MAE and RMSE measure the difference between actual and predicted house prices.

**Note:** R² is a regression metric and should not be interpreted as classification accuracy.

## Project Files

The repository contains the following files:

- `HousePrice_SupervisedLearning.ipynb` — Jupyter Notebook containing the complete project workflow.
- `train.csv` — Dataset used for analysis and model training.
- `house_price_model.pkl` — Saved trained machine learning model.
- `requirements.txt` — Required Python libraries.
- `summary_report.md` — Summary of the project and evaluation results.
- `README.md` — Project documentation.

## How to Run the Project

### Step 1: Clone the Repository

```bash
git clone <your-github-repository-url>
```

Replace `<your-github-repository-url>` with your actual GitHub repository URL.

### Step 2: Install Required Libraries

```bash
pip install -r requirements.txt
```

### Step 3: Open Jupyter Notebook

```bash
jupyter notebook
```

Open `HousePrice_SupervisedLearning.ipynb` and run the notebook cells in order.

Make sure the dataset file `train.csv` is available at the location specified in the notebook.

## Loading the Saved Model

The trained model can be loaded using Joblib:

```python
import joblib

model = joblib.load("house_price_model.pkl")
```

The loaded model can be used to make predictions when the input features are provided in the format expected by the saved model.

## Conclusion

This project demonstrates the application of supervised machine learning techniques to a real-world regression problem.

The project covers data exploration, preprocessing, feature engineering, model training, model comparison, and evaluation.

The reported R² score of 0.9323 indicates strong predictive performance on the evaluated dataset. The evaluation metrics provide useful information about how closely the predicted house prices match the actual sale prices.

Overall, this project provides practical experience in developing, evaluating, and saving a machine learning model for house price prediction.
