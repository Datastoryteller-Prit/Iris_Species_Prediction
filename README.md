# Iris Species Prediction:
## Overview
The Iris dataset, introduced by Ronald A. Fisher in 1936, is a classic in machine learning and statistics. My goal was to create separate models for predicting each species (Setosa, Versicolor, and Virginica) using both multinomial logistic regression and random forest, and to compare their accuracy. The dataset consists of 150 rows and 5 columns representing 4 features: sepal length, sepal width, petal length, and petal width, alongside the species.

## Process
 ### 1. Descriptive Statistics & Exploratory Data Analysis (EDA)
#### Tools: R programming, ggplot2, and corrplot
Initial analysis included summary statistics and visualizations to understand the distribution of variables and relationships between features.
### 2. Correlation Analysis
#### Tools: corrplot
Conducted a detailed correlation analysis to understand the relationships between variables. Petal length and petal width showed strong positive correlation.
### 3. Model Building
I created separate models for each species using:
Multinomial Logistic Regression (accuracy: 97%)
Random Forest (accuracy: 87%)
Both models were trained and evaluated to predict the species of the flower based on sepal and petal measurements.
### 4. Principal Component Analysis (PCA)
#### Purpose: 
To identify the most important features contributing to variance.
#### Findings: 
Setosa was distinctly separated from Versicolor and Virginica based on the first two principal components.
### 5. Feature Engineering
I derived two new features:
Petal Ratio = Petal Length / Petal Width
Sepal Ratio = Sepal Length / Sepal Width
The enhanced dataset (iris_new) now includes these ratios for better insight into morphological differences.
Using these engineered features, model accuracy improved:
Multinomial Logistic Regression: 93.33%
Random Forest: 90%
### 6. Separate Models for Sepal and Petal Data
Sepal Data (83% accuracy)
Petal Data (87% accuracy)
### 7. Shiny App
Developed a Shiny app that takes the petal ratio and sepal ratio as inputs and provides the probability of each species as output.
## Findings
According to PCA, Setosa is well-separated from Versicolor and Virginica.
Multinomial Logistic Regression consistently demonstrated higher accuracy compared to the Random Forest model, even after feature engineering.
The enhanced dataset, with newly created features (petal_ratio and sepal_ratio), improved the prediction performance.
