# Housing-Price-Prediction
Predicted house sale prices in Ames, Iowa, using the dataset provided by the Kaggle House Prices competition. In this comprehensive approach, I demonstrate data cleaning, feature engineering, and an ensemble of regression models.

# House Price Prediction



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

Top predictive features include:
- Overall quality of the house
- Living area square footage
- Neighborhood
- External quality
- Kitchen quality
- Garage size and quality

