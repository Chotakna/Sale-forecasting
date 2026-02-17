# Cinema Sales Forecasting Project

This repository contains a comprehensive machine learning project for forecasting cinema ticket sales using multiple quantitative forecasting models. The analysis was conducted using real cinema transaction data to predict future revenues and optimize business operations.

## Project Overview

This project analyzes cinema sales data to predict future ticket revenues using advanced machine learning techniques. The dataset includes detailed information about ticket sales, movie performances, cinema locations, and temporal patterns.

## Key Features

- **Multi-model Approach**: Implements 4 different forecasting models with detailed performance comparison
- **Comprehensive EDA**: Extensive exploratory data analysis with visualizations
- **Advanced Feature Engineering**: Creation of lag features, seasonal indicators, and interaction variables
- **Business-Focused Insights**: Actionable recommendations for cinema operations and management

## Models Implemented

### 1. XGBoost (Best Performing Model)
- **Performance**: RMSE: 129,876 | MAE: 37,075 | R²: 0.9998 | Accuracy: 99.52%
- **Why it works best**: Captures complex non-linear relationships between multiple features
- **Best for**: Strategic planning and multi-week forecasts

### 2. Linear Regression (Baseline Model)
- **Performance**: RMSE: 1,321,375 | MAE: 735,611 | R²: 0.9760 | Accuracy: 90.41%
- **Strengths**: Simple, interpretable, good baseline performance
- **Best for**: Understanding feature importance and baseline comparisons

### 3. SARIMAX (Seasonal Time Series Model)
- **Performance**: RMSE: 606,045,185 | MAE: 437,821,384 | R²: 0.9390 | Accuracy: 85.41%
- **Strengths**: Excellent at capturing weekly seasonality and short-term patterns
- **Best for**: Daily/weekly operational planning (1-7 days ahead)

### 4. Auto ARIMA (Automated Time Series)
- **Performance**: Lower accuracy compared to other models
- **Strengths**: Automated parameter selection for simple time series
- **Limitations**: Struggles with complex, feature-rich datasets

## Key Business Insights

### Sales Patterns Discovered
- **Weekend Effect**: Weekends generate 40-60% more revenue than weekdays
- **Peak Days**: Thursday accounts for 20.9% of weekly sales
- **Revenue Drivers**: A small number of hit movies drive most ticket revenue
- **Optimal Showtimes**: Evening weekend showings generate highest profits

### Operational Recommendations
- Schedule hit movies on more screens during peak periods
- Adjust staffing levels based on daily/weekly patterns
- Time promotions to align with natural sales peaks
- Customize strategies by cinema location based on historical response

## Technical Details

**Programming Language**: Python
**Main Libraries**: pandas, numpy, scikit-learn, XGBoost, statsmodels, matplotlib, seaborn
**Data Source**: Real cinema transaction data
**Analysis Tool**: Jupyter Notebook

## How to Use This Repository

1. Clone the repository
2. Install required dependencies: `pip install pandas numpy scikit-learn xgboost statsmodels matplotlib seaborn`
3. Open `Model/pp.ipynb` in Jupyter Notebook to run the complete analysis
4. Explore the data in the `data/` directory
5. Review additional analysis in the `Project/` folder

## Key Findings

- **XGBoost emerged as the champion model** with near-perfect accuracy (99.52%)
- **SARIMAX excels at short-term operational forecasting** for daily/weekly planning
- **Linear Regression provides valuable interpretability** for understanding business drivers
- **Auto ARIMA struggles with the complexity** of cinema sales data due to its volatile nature

## Business Applications

This project can help cinema operators with:
- **Revenue forecasting** for budget planning
- **Staff scheduling optimization** based on predicted demand
- **Inventory management** for concessions and merchandise
- **Movie scheduling decisions** based on performance predictions
- **Promotional timing** to maximize campaign effectiveness

The models and insights can be adapted for other entertainment venues or retail businesses with similar temporal sales patterns.
