# [EDA Grocery Data Analysis 2018](https://nicolerouleau.github.io/R_Grocery/)
#### Author
Nicole Rouleau

### Overview
This project analyzes grocery sales data to understand short-term demand patterns and generate sales forecasts using regression-based methods in R. The analysis focuses on identifying key drivers of sales variation across products and locations, and on producing interpretable forecasts suited for business decision-making rather than long-horizon prediction.
The project emphasizes model transparency, feature engineering, and practical forecasting choices given data constraints.

### Data
The dataset contains transactional grocery sales data with features such as:
- Sales volume
- Product category
- Store location (city)
- Time variables (weekly aggregation)
- Additional explanatory variables related to pricing and product mix
Due to a limited historical time window and a large number of covariates, traditional time-series models (e.g., ARIMA) were not well suited for this dataset.

### Methods
The analysis was conducted entirely in R, using a regression-based forecasting approach. Key steps include:
- Data cleaning and aggregation to weekly sales levels
- Feature engineering, including categorical variables for product category and city
- Exploratory data analysis to assess sales distribution and variation across dimensions
- Regression modeling to estimate the relationship between sales volume and explanatory variables
- Out-of-sample evaluation to assess short-term forecast performance
Rather than relying on univariate time-series methods, the model leverages cross-sectional variation to improve predictive accuracy and interpretability.

### Key Findings
Sales patterns varied substantially by product category and city, indicating that location-specific and category-specific effects are important drivers of demand. Regression-based models performed well for short-term forecasting when sufficient explanatory variables were included. Incorporating categorical features allowed the model to capture structural differences in demand that would be missed by purely time-based approaches. Forecast accuracy was more sensitive to feature selection than to model complexity.

### Visualizations
The project includes:
- Exploratory plots of sales trends by product category and city
- Model diagnostics and coefficient summaries
- Actual vs. predicted sales comparisons for evaluation periods
- Visualizations were designed to support interpretability for non-technical stakeholders.

### Tools & Technologies
- R
- tidyverse
- ggplot2
- regression modeling (base R / tidy modeling tools)

### Why This Project Matters
Retail sales forecasting often involves many predictors but limited time history, making standard time-series approaches impractical. This project demonstrates how regression-based methods can be effectively used to forecast demand, extract actionable insights, and support business planning in data-constrained environments. The approach shown here is directly applicable to roles involving business analytics, demand forecasting, and applied data science.
