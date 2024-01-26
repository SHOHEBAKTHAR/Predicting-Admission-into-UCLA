# Predicting Admission into UCLA

## Introduction
This machine learning project is designed to predict the probability of admission into the prestigious University of California, Los Angeles (UCLA) based on various academic and application-related factors. The primary goal is to develop a robust predictive model that can assist prospective students in understanding their chances of admission.

## Dataset
The dataset employed for this project is derived from the 'admission_predict.csv' file, encompassing comprehensive information about applicants. Key attributes include GRE scores, TOEFL scores, University ratings, Statement of Purpose (SOP) and Letter of Recommendation (LOR) ratings, CGPA, and the probability of admission. The initial steps involve loading the dataset and implementing necessary preprocessing steps to ensure data quality.

## Exploratory Data Analysis (EDA)
The Exploratory Data Analysis phase is crucial for gaining insights into the dataset's characteristics. Columns are appropriately renamed for clarity, and visualizations are created to understand the distributions of critical features such as GRE scores, TOEFL scores, University ratings, SOP ratings, and LOR ratings. These visualizations aid in identifying patterns and trends within the data.

## Data Preprocessing
To prepare the data for effective model training, several preprocessing steps are undertaken:
- The 'Serial No.' column, devoid of meaningful information, is removed.
- Zero values in significant features (GRE, TOEFL, University Rating, SOP, LOR, and CGPA) are replaced with NaN to handle missing data gracefully.
- A thorough check is performed to identify and quantify missing values in each column, ensuring a comprehensive understanding of the dataset's integrity.

## Model Selection
The selection of an appropriate regression model is a critical aspect of this project. Leveraging GridSearchCV, a systematic exploration of various regression algorithms is conducted. The models considered include:
- Linear Regression
- Lasso Regression
- Support Vector Regression (SVR)
- Decision Tree Regression
- Random Forest Regression
- K-Nearest Neighbors Regression

## Model Evaluation
To assess the performance of each model, cross_val_score is utilized to determine the highest accuracy. The dataset is then split into training and testing sets, with 80% dedicated to training and 20% for testing. A Linear Regression model is instantiated, trained on the designated training set, and subsequently evaluated on the test set.

## Prediction Example
To provide a practical demonstration of the model's capabilities, a sample prediction is showcased. Input values for GRE, TOEFL, University Rating, SOP, LOR, CGPA, and Research are specified, and the model predicts the probability of admission for this specific case.

Feel free to explore the accompanying Jupyter notebook for an in-depth examination of the code, visualizations, and a more profound understanding of the project. The flexibility to adjust input values allows prospective applicants to obtain personalized predictions, aiding them in making informed decisions about their academic pursuits at UCLA.