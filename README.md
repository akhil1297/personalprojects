# personalprojects

Seoul Bike Sharing System Analysis:

Introduction
The Seoul Bike Sharing System dataset offers comprehensive insights into bike rentals per hour, alongside holiday information and meteorological data. This analysis aims to uncover trends in bike rental demand and understand the influence of various factors such as weather conditions, time of day, and holidays. The report addresses specific questions raised in the data selection assignment, provides insights into hourly and daily rental patterns, and investigates the impact of weather.

Exploratory Data Analysis

Data Overview:
The dataset consists of 8,760 observations and 15 variables.
Variables include date, bike count, hour, temperature, humidity, wind speed, visibility, dew point temperature, solar radiation, rainfall, snowfall, seasons, holiday status, functioning day, and a weekend indicator.

Numeric Variables Summary:
Numeric variables exhibit a wide range of values, potentially requiring scaling for certain regression models.

Categorical Variables:
Categorical variables are appropriately formatted, with correctly ordered factor levels.

Date Variable:
The date variable is suitable for time-series analysis, though ensuring an appropriate date range is essential.

Missing Values:
It's crucial to check for missing values in the dataset to ensure data integrity.

Identification of Methods Used:
Regression Models
To answer the questions posed in the data selection assignment, linear regression and logistic regression methods were employed.

Linear Regression:
Hourly Weather Impact
Average Daily Weather Influence

Interpretation of Hourly Weather Impact Linear Regression Results and overall Model Fit
The overall model is statistically significant (p-value < 0.00000000000000022), indicating the presence of significant predictor variables.

Coefficient Interpretation
Temperature: Bicycle rentals rise by 28.40 for every unit increase in temperature.
Humidity: A reduction of 12.51 bike rentals is associated with a one-unit increase in humidity.
Wind Speed: An increase of one unit in wind speed correlates with a 64.67 rise in bike rentals.
Sun Radiation: There is a 119.21 drop in bike rentals for every unit increase in solar radiation.
Rainfall: A one-unit increase in rainfall corresponds to a 50.04 bike rental decrease.
Snowfall: An increase of 48.90 bike rentals is correlated with every unit increase in snowfall.
Seasons: Bicycle rentals are differently affected by seasons.
Holiday: Non-holiday days are linked to a rise in bike rentals compared to holidays.
Functioning Day: Functioning days are associated with a significant increase in bike rentals.

Model Performance
RMSE: Approximately 461.1264, indicating average prediction deviation.
R-squared: Approximately 0.4833206, explaining 48.33% of the variance in bike counts.
MAE: Approximately 336.9342, representing average absolute differences between predicted and actual values.
Strengths
Moderate Explanation: A significant amount of the variation in bike counts can be explained by the model.
Stable Generalization: Consistent model performance across various data subsets.
All-Inclusive Features: Incorporating a range of weather conditions and factors improves the model's explanatory power.

Areas for Improvement
Improved Prediction Accuracy: Reduction of average prediction errors.
Handling Metric Challenges: Addressing challenges with extreme or near-zero values in the dataset.

Feature Refinement: Further research into feature engineering methods could enhance predictive performance.

Significance of Predictors
All predictor variables are statistically significant except for visibility and dew point temperature.

Residual Plot
The residuals appear to be randomly scattered around the horizontal line at y = 0, indicating the appropriateness of the model for the data.

Conclusion
Temperature, wind speed, and functioning days positively influence bike rental demand.
Humidity, solar radiation, rainfall, and winter negatively impact bike rental demand.
Non-holiday days are associated with higher bike rental counts.
