# Regression Analysis with Python

This project demonstrates a regression analysis pipeline using Python, focusing on comparing the performance of two regression models: **Linear Regression** and **Random Forest Regressor**. The analysis includes data preprocessing, model training, evaluation, and visualization.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Project Steps](#project-steps)
- [Results](#results)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [License](#license)

## Project Overview
The goal of this project is to predict a target variable using regression models and evaluate their performance. Using the **California Housing Dataset** from Scikit-Learn, I aim to assess the models' accuracy by comparing their **Mean Squared Error (MSE)** and **R² score**.

## Dataset
I use the **California Housing Dataset** from Scikit-Learn, which provides data on various features of housing in California.

## Project Steps
1. **Setup and Imports**  
   Import essential libraries for data handling, model training, and evaluation:
   - **Scikit-Learn** for model training and evaluation.
   - **Pandas** and **NumPy** for data handling.
   - **Matplotlib** and **Seaborn** for visualizations.

2. **Load and Explore the Dataset**  
   Load the dataset using `load_data()` or `pd.read_csv()`. Perform an **Exploratory Data Analysis (EDA)** to understand:
   - Data distribution.
   - Missing values.
   - Correlations between features.

3. **Data Preprocessing**  
   - Handle missing values if any.
   - Scale the features to improve model performance.
   - Split data into features (X) and target (y).

4. **Train-Test Split**  
   Divide the dataset into training and testing sets.

5. **Model Selection and Training**  
   Train two regression models:
   - **Linear Regression**
   - **Random Forest Regressor**

6. **Prediction and Evaluation**  
   - Use both models to predict target values on the test set.
   - Calculate **MSE** and **R² score** as performance metrics.

7. **Cross-Validation**  
   Apply k-fold cross-validation to check model generalizability.

8. **Visualization of Results**  
   Plot predicted vs. actual values to visualize model performance.

## Results
Based on the evaluation metrics, **Random Forest Regressor (Model 2)** outperforms **Linear Regression (Model 1)**:

- **Mean Squared Error (MSE)**:
  - **Linear Regression**: MSE = 0.5559
  - **Random Forest Regressor**: MSE = 0.2525
  - A lower MSE indicates that the Random Forest model has better predictive accuracy.

- **R-squared (R²) Score**:
  - **Linear Regression**: R² = 0.5758
  - **Random Forest Regressor**: R² = 0.8073
  - A higher R² score signifies that the Random Forest model explains the variance better in the data.

## Visualizations
Visualizations included:
- **Predicted vs. Actual Values** plot to assess model performance visually.
- **Feature Importance** (for the Random Forest model) to understand which features have the most influence.

## Conclusion
The **Random Forest Regressor** demonstrates superior performance over **Linear Regression** in this regression analysis, as evidenced by its lower MSE and higher R² score. This project showcases how to evaluate regression models' accuracy, perform data preprocessing, and visualize results in Python.

## License
This project is open-source under the MIT License.
