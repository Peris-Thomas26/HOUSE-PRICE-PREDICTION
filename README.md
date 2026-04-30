# California Housing Price Regression Model

A machine learning project that predicts median house values in California using OLS (Ordinary Least Squares) regression analysis. This project includes comprehensive exploratory data analysis, feature engineering, and statistical modeling to understand the factors that affect housing prices.

## Overview

This project analyzes the California Housing dataset to build a predictive regression model for median house values. The analysis includes data preprocessing, feature engineering, exploratory visualizations, and model evaluation using statistical regression techniques.

## Features

- **Data Preprocessing**: Handles missing values and prepares data for modeling
- **Feature Engineering**: Creates derived features like rooms per household, population per household, and bedrooms per room ratio
- **Exploratory Data Analysis**: Comprehensive visualizations including distributions, correlations, and relationships between variables
- **OLS Regression Model**: Statistical regression analysis with detailed model summary
- **Model Evaluation**: Performance metrics including RMSE and R² score on test data
- **Visualization**: EDA plots and actual vs predicted value comparisons

## Dataset

The project uses the California Housing dataset, containing 20,640 housing records with the following features:

- **longitude**: Longitude coordinate
- **latitude**: Latitude coordinate
- **housing_median_age**: Median age of houses in the area
- **total_rooms**: Total number of rooms
- **total_bedrooms**: Total number of bedrooms
- **population**: Total population
- **households**: Number of households
- **median_income**: Median income in the area
- **median_house_value**: Target variable (median house value in $100,000s)
- **ocean_proximity**: Proximity to ocean (categorical)

## Project Structure

```
.
├── project.ipynb                      # Main Jupyter notebook with full analysis
├── housing.csv                        # Input dataset
├── eda_plots.png                      # Exploratory data analysis visualizations
├── actual_vs_predicted.png            # Model prediction comparison plot
├── prediction_results.csv             # Model predictions and residuals
├── README.md                          # This file
└── requirements.txt                   # Python dependencies
```

## Installation

### Prerequisites

- Python 3.7+
- pip or conda

### Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/california-housing-regression.git
cd california-housing-regression

# Install required packages
pip install -r requirements.txt
```

## Dependencies

```
pandas>=1.0.0
numpy>=1.18.0
matplotlib>=3.1.0
seaborn>=0.10.0
scikit-learn>=0.22.0
statsmodels>=0.11.0
jupyter>=1.0.0
```

## Usage

Open and run the Jupyter notebook to execute the full analysis:

```bash
jupyter notebook project.ipynb
```

The notebook will:
1. Load and explore the housing dataset
2. Perform data preprocessing and feature engineering
3. Generate exploratory data analysis visualizations
4. Train an OLS regression model
5. Evaluate model performance on test data
6. Generate prediction visualizations and export results

## Model Performance

The trained OLS regression model achieves:

- **RMSE**: Model's mean squared error on test data
- **R² Score**: Coefficient of determination measuring model fit quality

See the detailed model summary in the notebook output for coefficient estimates and statistical significance.

## Key Visualizations

1. **Distribution of Median House Value**: Histogram showing the distribution of target variable
2. **Median Income vs House Value**: Scatter plot revealing the relationship between income and price
3. **House Value by Ocean Proximity**: Box plot comparing prices across different ocean proximity categories
4. **Correlation Heatmap**: Shows relationships between all numerical features
5. **Housing Median Age vs House Value**: Scatter plot of age vs price relationship
6. **Actual vs Predicted**: Scatter plot comparing model predictions with actual values

## Results

Model outputs are saved to:

- `eda_plots.png`: Comprehensive exploratory analysis visualizations
- `actual_vs_predicted.png`: Model prediction accuracy visualization
- `prediction_results.csv`: Detailed predictions, actual values, and residuals for the test set

## Methodology

The project follows a structured approach:

1. **Data Loading & Exploration**: Assess data shape, missing values, and basic statistics
2. **Data Cleaning**: Handle missing values using median imputation
3. **Feature Engineering**: Create meaningful derived features
4. **Categorical Encoding**: One-hot encode the ocean_proximity categorical variable
5. **Train-Test Split**: 80-20 split with random_state=42 for reproducibility
6. **Model Training**: Fit OLS regression using statsmodels
7. **Evaluation**: Assess performance using RMSE and R² metrics
8. **Visualization**: Create comprehensive plots for analysis communication

## Insights

The analysis reveals:

- Median income is a strong predictor of house values
- Ocean proximity significantly impacts housing prices
- Housing age shows a relationship with median house value
- Geographic location (latitude/longitude) plays a role in price determination

## Future Improvements

- Explore non-linear relationships and polynomial features
- Implement regularization techniques (Ridge, Lasso)
- Test alternative algorithms (Random Forest, Gradient Boosting)
- Cross-validation for more robust model evaluation
- Spatial analysis of geographic features
- Time-series analysis if temporal data becomes available

#

