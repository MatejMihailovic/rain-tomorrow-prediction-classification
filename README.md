#Weather Prediction Project 
This project aims to predict rainfall for the next day using machine learning models based on the 'WeatherAUS' dataset sourced from Kaggle. The task is a classification problem, with 'RainTomorrow' as the target variable.

##Dataset
The dataset comprises various meteorological features collected daily, providing insights into weather patterns across different locations in Australia.

##Exploratory Data Analysis (EDA)
The exploratory analysis involved:

* Inspecting the dataset's structure and attributes.
* Handling missing values, mainly dropping rows with 'RainTomorrow' or 'RainToday' as null.
* Addressing missing values for numerical columns with a threshold of 5%, either through imputation or dropping.
* Converting 'Date' column to DateTime, extracting 'Year', 'Month', and 'Day', and dropping the original 'Date'.
* Identifying potential outliers in specific numerical columns.
* Handling outliers using a top-coding approach to cap maximum values.
##Data Preparation
* Dropped highly correlated columns ('Temp3pm', 'Temp9am', 'Humidity9am').
* Encoded categorical variables using one-hot encoding.
* Scaled data using MinMaxScaler for improved model performance.
##Model Building
* Trained and evaluated multiple machine learning models:
  * Logistic Regression
  * K-Nearest Neighbors (KNN)
  * Naive Bayes
  * Support Vector Machines (SVM)
* Explored model-specific insights such as precision-recall curves, feature importance, and hyperparameter tuning.
##Model Evaluation
* Compared models based on accuracy, precision, recall, ROC-AUC, F1 score, and confusion matrices.
* Identified Logistic Regression as the top-performing model with balanced metrics.
##Handling Imbalanced Data
* Employed under-sampling and over-sampling techniques using RandomUnderSampler and SMOTE.
* Evaluated the performance of models post-sampling to understand their impact on predictions.
##Weighting and Stratification
* Explored weighted and unweighted models to understand their impact on capturing positive cases and overall performance.
* Highlighted differences in metrics between the unweighted and weighted versions of various models (Logistic Regression, KNN, Naive Bayes, SVM).
##Conclusion
* Logistic Regression demonstrated superior overall performance but with considerations for different evaluation metrics.
* Model performance varied between weighted and unweighted versions, emphasizing trade-offs between capturing positive cases and overall accuracy, precision, and recall.



 
