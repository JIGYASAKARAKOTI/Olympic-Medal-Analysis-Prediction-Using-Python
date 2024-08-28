# Olympic-Medal-Analysis-Prediction-Using-Python
## Data Extraction
### The dataset athlete_events.csv is loaded and basic statistics are extracted, including distributions of age, gender, season, and participation by country.Exploratory Data Analysis (EDA) is conducted with visualizations of participant distribution by age, gender, season, and countries' participation and medal achievements.
### Dataset- Athlete_Events

## Data Cleaning and Feature Engineering
### Missing values are handled by filling in the mean values for numerical columns like Age, Height, and Weight. Unnecessary columns are dropped, and categorical columns are binary encoded (like Sex, Season) or one-hot encoded (like Team, NOC, City, etc.). Feature selection is performed using SelectKBest with the chi2 method, extracting the top 10 features.
## Data Scaling
### Features are scaled using MinMaxScaler.
## Modeling : Several classification algorithms are applied to the dataset:
#### Logistic Regression: Achieves an accuracy of ~87.6%, but fails to predict the minority class (medal winners).
#### Multinomial Naive Bayes: Similar performance to Logistic Regression with the same issues.
#### Decision Tree Classifier: Slightly better in predicting the minority class but still has limitations.
#### Random Forest Classifier: Achieves the highest accuracy (~89.0%) and performs better in predicting medal winners but still has room for improvement.
