# ML_PROJECT_03
# Time-Series Forecasting of Carbon Monoxide and Nitrogen Dioxide Levels

## Overview
This project aims to build predictive models to forecast daily or hourly concentrations of Carbon Monoxide (CO) and Nitrogen Dioxide (NO₂) based on historical air quality data. The goal is to provide insights and recommendations for mitigating high levels of these gases.

## Dataset
The dataset used in this project is sourced from [Public Datasets](https://raw.githubusercontent.com/rashakil-ds/Public-Datasets/refs/heads/main/airquality.csv). It contains the following columns:

- `Date`: Date of the observation
- `Time`: Time of the observation
- `CO(GT)`: Carbon Monoxide concentration
- `NO2(GT)`: Nitrogen Dioxide concentration
- Other features related to air quality and environmental conditions (e.g., temperature, humidity).

## Project Workflow
1. **Data Preprocessing**
   - Combine `Date` and `Time` columns into a single datetime column.
   - Set the datetime column as the index of the dataset.
   - Resample the data into meaningful time intervals (e.g., hourly or daily averages).
   - Handle missing values using interpolation and outlier detection.

2. **Exploratory Data Analysis (EDA)**
   - Visualize long-term trends of CO and NO₂.
   - Identify seasonal patterns and correlations with other features.

3. **Feature Engineering**
   - Create lag features for CO and NO₂ to incorporate historical values.
   - Add time-based features (e.g., hour of the day, day of the week, month).
   - Include environmental factors (temperature, humidity) as predictors.

4. **Modeling**
   - Train various forecasting models, including:
     - SARIMAX
     - Random Forest Regressor
     - LSTM (Long Short-Term Memory) networks
   - Evaluate model performance using metrics such as Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

5. **Forecast Visualization**
   - Generate forecasts for future dates and visualize the trends.
   - Highlight seasonal patterns and periods of concern.

6. **Insights and Recommendations**
   - Provide actionable recommendations based on predicted trends to mitigate high levels of CO and NO₂.

## Installation
To run this project, you need to have Python installed along with the following libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels
- keras
