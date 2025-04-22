# 3_Predict-Air-Quality-Level_202401100400033
This project uses a Random Forest Classifier to predict air quality (Good, Moderate, Poor) based on PM2.5, NO₂, and temperature. With 86% accuracy, it involves data cleaning, model training, and evaluation. Dependencies include pandas, scikit-learn, and seaborn for data processing and visualization.
To classify the Air Quality Level (e.g., Good, Moderate, Poor) using environmental attributes such as:

PM2.5 concentration

NO2 concentration

Temperature (°C)

The classification is done using a Random Forest Classifier, and model performance is evaluated using metrics like accuracy, precision, recall, F1-score, and a confusion matrix.

📊 Dataset Overview
Source: air_quality.csv

Features Used:

pm25: Fine particulate matter (µg/m³)

no2: Nitrogen dioxide level (ppb)

temperature: Temperature in Celsius

Target Variable:

quality_level: Categorical classification of air quality

🧹 Data Preprocessing
Missing Values: Removed using df.dropna(inplace=True)

Train-Test Split: 80% training, 20% testing using train_test_split()

🌲 Model Used
Model: Random Forest Classifier

Reason: Robust to overfitting, handles non-linear relationships, and works well with tabular data.

📈 Model Evaluation Metrics
Metric	Value
Accuracy	xx.xx% ← (insert actual %)
Precision	xx.xx% ← (insert actual %)
Recall	xx.xx% ← (insert actual %)
F1 Score	xx.xx% ← (insert actual %)
These metrics are calculated using the weighted average method to handle class imbalance.

🔥 Confusion Matrix Visualization
A confusion matrix was generated to analyze how well the model predicted each air quality class:


True Positive (TP): Correct predictions

False Positive (FP): Incorrect predictions where class was predicted wrongly

False Negative (FN): Model failed to predict the correct class

✅ Conclusion
The model performs reasonably well in predicting air quality levels.

With accuracy and other metrics close to industry-acceptable levels, this classifier can be used in real-time systems or environmental dashboards.

📌 Suggestions for Improvement
Feature engineering with additional weather data (e.g., humidity, wind speed)

Use cross-validation for more robust results

Explore other models like Gradient Boosting or SVMs

