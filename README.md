# Used Bike Price Prediction

An end-to-end Machine Learning project designed to predict the resale price of used bikes using data preprocessing, feature engineering, exploratory data analysis (EDA), and regression models.

The project leverages Python and machine learning techniques to help buyers, sellers, and dealerships estimate fair market prices for used motorcycles based on their characteristics.


## Project Overview

Pricing used bikes accurately is challenging due to various factors such as bike age, mileage, engine power, ownership history, and brand value.

This project aims to build predictive models that estimate the price of a used bike by analyzing historical bike listing data and extracting meaningful insights.

---

## Business Problem

The used bike market often suffers from:

* Inconsistent pricing
* Information asymmetry between buyers and sellers
* Difficulty in estimating fair resale values

This project addresses these challenges by developing a machine learning model capable of predicting used bike prices based on key features.


## Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-Learn**
* **Jupyter Notebook**


## Project Workflow

### 1️ Data Collection

* Loaded used bike dataset from CSV file.
* Explored dataset structure and attributes.

### 2️ Data Cleaning & Preprocessing

* Handled missing values.
* Removed duplicate records.
* Standardized inconsistent data formats.
* Cleaned numerical fields such as:

  * Mileage
  * Power
  * Kilometers Driven

### 3️ Exploratory Data Analysis (EDA)

Performed detailed analysis including:

* Correlation Analysis
* Scatter Plots
* Heatmaps
* Boxplots
* Multivariate Analysis
* Location-wise Price Analysis

### 4️ Outlier Detection & Removal

Used the **Interquartile Range (IQR)** method to remove outliers from:

* Price
* Power
* Mileage
* Kilometers Driven

### 5️ Feature Engineering

Created new features to improve model performance:

* **Brand Extraction** from bike model names
* **Bike Age** derived from model year
* **Engine Capacity (CC)** extraction
* **Power-to-Weight Ratio**
* **Owner Mapping** into numerical categories

### 6️ Feature Transformation

Applied:

* **One-Hot Encoding** for categorical variables
* **Standard Scaling** for numerical features

### 7️ Model Building

Implemented and evaluated multiple regression models:

* Linear Regression
* Lasso Regression
* Gradient Boosting Regressor
* Random Forest Regressor

### 8️ Model Evaluation

Evaluated models using:

* **R² Score**
* **Mean Squared Error (MSE)**
* **Root Mean Squared Error (RMSE)**

Feature importance analysis was also performed to identify the most influential variables affecting bike prices.


##  Key Features

✔ Data Cleaning & Preprocessing
✔ Exploratory Data Analysis
✔ Feature Engineering
✔ Outlier Detection & Removal
✔ Machine Learning Model Training
✔ Feature Importance Analysis
✔ Used Bike Price Prediction


##  Key Insights

* Newer bikes generally command higher prices.
* Mileage and power significantly influence resale value.
* Engine capacity plays a crucial role in pricing.
* Ownership history impacts the market value of used bikes.
* Brand reputation affects resale prices.


## Repository Structure

Used-Bike-Price-Prediction/
│
├── Data/
│   └── raw_data.csv                 # Raw used bike dataset
│
├── Python/
│   └── Used_bike_price_prediction.ipynb
│                                    # Data preprocessing, EDA, feature engineering, and ML models
│
├── Images/
│   ├── eda.png                      # Exploratory Data Analysis visualizations
│   └── model_comparison.png         # Comparison of machine learning models
│
├── requirements.txt                # Project dependencies
└── README.md                       # Project documentation


## How to Run

### Clone the Repository

```bash
git clone https://github.com/aryanpashte42/Used-Bike-Price-Prediction.git
cd Used-Bike-Price-Prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```bash
Used_bike_price_prediction.ipynb
```

## Future Enhancements

* Deploy model using Streamlit or Flask
* Hyperparameter tuning using GridSearchCV
* Incorporate real-time bike listing data
* Experiment with advanced models like XGBoost
* Build an interactive price prediction web application


## Author

**Aryan Pashte**

*MBA Finance | Aspiring Data Analyst | Financial Analyst*

**Skills:** Python | SQL | Power BI | Advanced Excel | Financial Modeling | Machine Learning


⭐ If you found this project useful, feel free to star the repository!


## Model Performance

| Model | R² Score | RMSE |
|---------|---------:|---------:|
| Random Forest | 0.890 | 15,286 |
| Gradient Boosting | 0.886 | 15,536.6 |
| Lasso | 0.818 | 19,684.2 |
| Linear Regression | 0.816 | 19,743.1 |

### Best Performing Model

Random Forest Regressor achieved the highest R² score of 0.890 and the lowest RMSE, making it the most accurate model for predicting used bike prices in this project.
