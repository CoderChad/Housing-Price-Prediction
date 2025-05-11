# House Price Prediction

## Advanced Regression Techniques for Ames Housing Dataset

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-orange.svg)
![XGBoost](https://img.shields.io/badge/XGBoost-Latest-green.svg)
![LightGBM](https://img.shields.io/badge/LightGBM-Latest-lightgreen.svg)

A comprehensive solution for the [Kaggle House Prices Competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques).

## Project Overview

This project aims to predict house sale prices for residential homes in Ames, Iowa, using advanced regression techniques. The dataset contains 79 explanatory variables describing various aspects of residential homes.

### Key Features

- Extensive exploratory data analysis with visualizations
- Comprehensive data preprocessing and feature engineering
- Multiple regression models with ensemble techniques
- Advanced model stacking and weighted averaging

## Dataset

The Ames Housing dataset contains information from the Ames Assessor's Office used in computing assessed values for residential properties sold in Ames, Iowa from 2006 to 2010.

- Training set: 1,460 observations
- Test set: 1,459 observations
- Features: 79 explanatory variables (mix of categorical and numerical)

## Project Structure

```
├── data/
│   ├── train.csv
│   ├── test.csv
│   └── data_description.txt
├── images/
│   ├── correlation_matrix.png
│   ├── feature_importance.png
│   ├── saleprice_distribution.png
│   └── ...
├── house_prices_prediction.py
├── report.md
├── requirements.txt
└── README.md
```

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/house-price-prediction.git
cd house-price-prediction

# Install dependencies
pip install -r requirements.txt
```

## Requirements

```
numpy>=1.20.0
pandas>=1.3.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=1.0.0
xgboost>=1.5.0
lightgbm>=3.3.0
scipy>=1.7.0
```

## Usage

```bash
# Run the complete solution
python house_prices_prediction.py

# This will:
# 1. Process the data
# 2. Train the models
# 3. Generate predictions
# 4. Create a submission.csv file
```

## Approach

The solution follows these key steps:

1. **Exploratory Data Analysis**
   - Analyze target variable distribution
   - Identify correlations between features
   - Visualize important relationships

2. **Data Preprocessing**
   - Handle missing values based on domain knowledge
   - Transform skewed numerical features
   - Encode categorical variables

3. **Feature Engineering**
   - Create composite features (TotalSF, TotalBathrooms)
   - Generate age-related features (HouseAge, RemodAge)
   - Develop quality score indicators

4. **Modeling**
   - Train multiple base models (Lasso, Ridge, ElasticNet, GBM, XGBoost, LightGBM)
   - Evaluate performance using cross-validation
   - Implement stacking and weighted averaging for ensemble prediction

5. **Evaluation & Submission**
   - Measure performance using RMSE
   - Generate final predictions for test data
   - Create submission file

## Results

The solution achieves competitive results on the Kaggle leaderboard. The ensemble approach combining multiple models helps mitigate individual model weaknesses and produces robust predictions.

Top predictive features include:
- Overall quality of the house
- Living area square footage
- Neighborhood
- External quality
- Kitchen quality
- Garage size and quality

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Kaggle](https://www.kaggle.com) for hosting the competition
- The Ames Assessor's Office for providing the dataset
- Dean De Cock for creating the dataset
