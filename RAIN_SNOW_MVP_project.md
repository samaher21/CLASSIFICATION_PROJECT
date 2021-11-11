
# Weather_rain-or-snow
### Goal of the project:
The core objective of this project is to classify whether will rain or snow based on weather data.

### Workflow:
The dataset for this project is the weather History dataset on Kaggle,
And our target is the **PRECIP TYPE** (rain, snow) column.

1-Dropped all duplicated rows and unneeded columns.

2-Removed nulls and outliers.

3-Converting object-type columns into numeric.

4-find the correlation and plot heatmap

The number of columns and rows before cleaning were **12** and **96,453** After cleaning up the data the number of columns and rows are **16** and **95,829**.

The figure below shows the correlation between the features

<img src="https://github.com/samaher21/CLASSIFICATION_PROJECT/blob/main/heatmapforWeather.png" alt="drawing" width="600"/>  

### Next step:

Afterwards, We plan to experiment with the Logistic Regression, Random Forest, XGBoost, Support Vector Machines,Decision Tree, KNN and Naive Bayes models.
Currently, we’re in the midst of tuning the logistic regression model to obtain better results.
