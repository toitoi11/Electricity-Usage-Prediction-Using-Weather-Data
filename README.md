# Electricity Usage Prediction Using Weather Data
## Description
This project uses weather data (e.g., temperature, humidity, rainfall, etc.) to predict electricity usage using machine learning techniques. The project explores various combinations of input features and evaluates the performance of a linear regression model based on the R2 score and the accuracy of the predictions. The goal is to find the best combination of weather-related features that accurately predicts electricity usage.

## Features
* Weather Data-Based Prediction: Predicts electricity usage based on various weather features like temperature, rainfall, humidity, daylight, etc.
* Multiple Feature Combinations: Evaluates different combinations of input features to determine the most effective predictors of electricity usage.
* R2 Score Evaluation: The model is evaluated using R2 scores, and predictions are compared against actual values.
* Scaled R2 Scores: R2 scores are scaled and sorted to provide insights into the accuracy of different feature combinations.
* Accuracy Assessment: Calculates the percentage of correct predictions within a margin of error.

# Data Format
The input data should be in CSV format with the following columns:

* date: The date of the weather observation.
* temp_mean: The mean temperature of the day.
* temp_high: The highest temperature of the day.
* temp_low: The lowest temperature of the day.
* rain: Rainfall (in mm).
* humid: Humidity (in percentage).
* day: The number of daylight hours.
* light: Daylight intensity.
* sunrise: The time of sunrise (converted into minutes from midnight).
* elec: The electricity usage.

# Model Evaluation
* The script evaluates the linear regression model using the R2 score for different combinations of input features.
* The results are sorted by the highest R2 scores, and the model's accuracy is assessed by comparing actual and predicted electricity usage.

# Example Output
* R-squared (R2) Score: The script sorts and displays the R2 scores for all feature combinations in descending order, along with scaled R2 values.
* Accuracy: It calculates the percentage of correct predictions within the first 31 rows of the test data.
* Results are saved in result_output_sorted.txt.
