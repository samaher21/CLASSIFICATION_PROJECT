# Abstract
The main goal of this project is to predict weather if will rain or snow.

# Design
Using the data provide by kaggle, we are going to build a classification model to predicting the weather of a day given several features like temperature,
wind speed, humidity etc. and the targeted classification is two categories of weather they (rain and snow) of a next day.

# Data
The data that was used in this project from kaggle.The data was represented in **96,435 rows** and **12 columns**.
After performing the initial EDA After cleaning the data, we got **95,912 rows** and **16 columns**.

**Target:**
* Precip Type

**Features:**
- Formatted Date.
-	Summary.
-	Precip Type.
-	Temperature (C).
-	Apparent Temperature (C).
-	Humidity.
-	Wind Speed (km/h).
-	Wind Bearing (degrees).
-	Visibility (km).
-	Loud Cover.
-	Pressure (millibars).
-	Daily Summary.

# Methodology
* Gathiring Data.
* Exploratory Data Analysis was done to the dataset.
* Building multple models and finding out the well-suited one for this specific dataset.

**Cleaning**:
* Dropped unneeded columns.
* Handled nulls.
* Handled Duplicates.
* Detected the relationship between the target and feature through a pair and a correlation plot.

**Feature Engineering**
* Add new column (‘SEASON’).
* Encoding the columns into categorical values.
* Scaling using standard Scaler.

**Imbalanced dataset**
* SMOTE was use for handling the imbalanced, After resamplig SNOW: 83010
RAIN: 83010

**Model Building:** Around 7 models were tried and played with to get the best model with the dataset.
After performing simple train and validation on the 7 models one was chosen for further investigation. The implemented models:
1. Logistic Regression Classifier.
2. K-Nearest Neighbors Classifier
3. Decision Tree Classifier.
4. Random Forest Classifier.
5. XGB Classifier.
6. Guassian Classifier.
7. Support Vector Machine (SVM)
The best three models were then fitted into the Voiting Classifier, and those models are:
* Decision Tree Classifier.
* Random Forest Classifier.
* XGBoost Classifier.

**The chosen model**: voiting Classifier after refitting the best three models within it, resulted in the following score.
| Model              | Precision   |Recall     |F1        |Accuracy for Test |
| ------------------ | ----------- |-----------|----------|------------------|
| voiting Classifier | 1.00        |1.00       | 1.00     | 1.00             |

# Tools
* Numpy
* Pandas
* Pickle
* Matplotlib
* Seaborn
* SqlLite
* Sklearn
