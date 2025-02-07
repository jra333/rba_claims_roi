# RBA Claims (EDA & Modeling)

This notebook provides an extensive framework to perform exploratory data analysis (EDA) and modeling on claims data. The analysis and modeling aims to find the statistical significance of various marketing metrics to insuarance claims (sales). Given the nuanced sector in which this analysis was performed on the results varied and warrant further exploration -- with search based spending showing more "correlation."  The amount of unknowns outweighed the amount of data available to attribute a large portion of market spends to actual claims.

## Overview

The notebook is structured into several sections:

1. **Import Libraries & Initialize Functions**  
   - Loads essential libraries for data processing (e.g., pandas, numpy), visualization (e.g., matplotlib, seaborn), and modeling (e.g., scikit-learn, statsmodels).
   - Initializes utility functions (e.g., for safe division and data processing).

2. **Gather and Process Datasets**  
   - Pulls claims data (from Excel files and/or Snowflake) and RBA data.
   - Cleans and preprocesses the data:
     - Date parsing and reindexing.
     - Handling missing values/extrapolation via interpolation.
     - Converting data types and reformatting headers.

3. **Exploratory Data Analysis (EDA)**  
   - Investigates the dataset by performing:
     - Seasonal decomposition to evaluate trends.
     - Autocorrelation analysis.
     - Visualization of the correlation matrix and heatmaps.
     - Joint plots and monthly time series (line) plots.
     
4. **Modeling**  
   - Implements various regression techniques (e.g., Linear Regression, Ridge, Lasso, Random Forest, Gradient Boosting) for evaluating claims.
   - Includes cross-validation and parameter tuning pipelines.
   - Evaluates model performance using metrics such as MSE, MAE, R², etc.

5. **Visualization of Model Outputs**  
   - Provides visual insights into model performance.
   - Explores the impact of impression lags on overall model accuracy.
   - Contains sections for further exploration such as combined LSTM and digital LSTM approaches for sequential data modeling.

