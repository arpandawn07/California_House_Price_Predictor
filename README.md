# California_House_Price_Predictor


# House Price Prediction Using Machine Learning

A machine learning regression project that predicts median house values using housing data. This project explores the complete workflow of a typical machine learning task, from exploratory data analysis and preprocessing to model training, evaluation, and prediction.

## Project Overview

The goal of this project is to understand the factors influencing house prices and build regression models that can estimate median house values from housing-related features.

The project uses Python and popular machine learning libraries to explore the dataset, engineer useful features, compare different regression algorithms, and evaluate their performance using standard regression metrics.

## Objectives

- Perform exploratory data analysis (EDA) to understand the dataset.
- Identify relationships between housing features and median house values.
- Handle missing values and preprocess numerical and categorical features.
- Create new features to improve the model's predictive ability.
- Train and compare multiple regression algorithms.
- Evaluate model performance using appropriate regression metrics.
- Build a prediction function and save trained model components for reuse.

## Dataset

The project uses the California housing dataset, containing information about housing districts and demographic characteristics.

The dataset includes features such as:

- `longitude` and `latitude`
- `housing_median_age`
- `total_rooms`
- `total_bedrooms`
- `population`
- `households`
- `median_income`
- `ocean_proximity`

The target variable is `median_house_value`, which represents the median house value for a district.

The notebook works with a dataset containing 20,640 records.

## Exploratory Data Analysis

The following analyses are performed to understand the data:

- Distribution of numerical features using histograms.
- Correlation analysis using a heatmap.
- Geographic visualization of housing data.
- Examination of relationships between housing features and median house values.

These visualizations help identify patterns, understand feature relationships, and guide preprocessing and feature engineering decisions.

## Data Preprocessing and Feature Engineering

The preprocessing workflow includes:

- Handling missing values.
- Separating input features from the target variable.
- Transforming numerical and categorical features.
- Scaling numerical features where appropriate.
- Creating additional features to represent housing characteristics.

### Engineered Features

The project creates the following features:

- `rooms_per_household`: Average number of rooms per household.
- `population_per_household`: Average population per household.
- `bedrooms_per_room`: Proportion of bedrooms relative to total rooms.

These features provide additional information that may help regression models learn useful patterns from the data.

## Machine Learning Models

The notebook explores and compares multiple regression algorithms, including:

- Linear Regression
- Ridge Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost Regressor

The models are evaluated to understand how different algorithms perform on the same prediction task.

## Model Evaluation

The project uses the following metrics to evaluate model performance:

| Metric | Description |
|---|---|
| R² Score | Measures how much variation in the target is explained by the model. |
| MAE | Measures the average absolute difference between actual and predicted values. |
| RMSE | Measures prediction error while penalizing larger errors more heavily. |

### Reported Results

The current notebook reports the following results for the XGBoost model:

| Metric | Reported Value |
|---|---:|
| R² Score | 0.823 |
| Mean Absolute Error (MAE) | $31,950 |
| Root Mean Squared Error (RMSE) | $48,957 |

These are the values recorded in the notebook and should be verified by rerunning the final corrected workflow. They are not a guarantee of performance on new data.

## Technologies Used

- **Python** — Programming language
- **NumPy** — Numerical computations
- **Pandas** — Data manipulation and analysis
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualizations
- **Scikit-learn** — Preprocessing, regression models, and evaluation metrics
- **XGBoost** — Gradient boosting regression
- **Joblib** — Saving and loading model artifacts
- **Jupyter Notebook** — Interactive development and experimentation

## Project Structure

```text
House-Price-Prediction/
│
├── House_Price_Pred.ipynb
├── README.md
├── requirements.txt
└── housing.csv
```

The dataset file should be included only if redistribution is permitted. Otherwise, follow the dataset instructions provided with the notebook.

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/House-Price-Prediction.git
cd House-Price-Prediction
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Create a virtual environment (recommended)

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

Ensure `requirements.txt` contains the packages used by the notebook, including NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, XGBoost, Joblib, and Jupyter.

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `House_Price_Pred.ipynb` and run the cells in order.

Make sure the dataset is available at the file path expected by the notebook.

## Future Improvements

- Improve preprocessing by using pipelines for missing-value imputation and feature transformations.
- Perform hyperparameter tuning to improve model performance.
- Use cross-validation for more reliable model evaluation.
- Compare additional regression algorithms.
- Build a simple web application for interactive house-price predictions.
- Improve prediction input validation and model deployment.

## Learning Outcomes

Through this project, I explored:

- Exploratory data analysis and data visualization.
- Data cleaning and feature engineering.
- Numerical and categorical data preprocessing.
- Regression algorithms and model comparison.
- Model evaluation using R², MAE, and RMSE.
- Building prediction functions and saving trained model components.

## Disclaimer

This project is intended for educational purposes and machine learning practice. The predictions are estimates based on historical housing data and should not be considered professional property valuations or financial advice.

## Author

**Arpan Dawn**
