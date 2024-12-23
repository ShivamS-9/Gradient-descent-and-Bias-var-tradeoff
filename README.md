# Gradient descent and Bias variance tradeoff

> This repository contains the work done for **Machine, Data and Learning** as part of the coursework. The tasks involve applying machine learning concepts such as **Gradient Descent**, **Bias-Variance Tradeoff**, **Model Complexity**, and **Irreducible Error** on a dataset.

## Tasks Covered
- **Task 1**: Gradient Descent
- **Task 2**: Numerical Problems on Bias and Variance
- **Task 3**: Calculating Bias and Variance for different model complexities
- **Task 4**: Calculating Irreducible Error
- **Task 5**: Plotting Bias² - Variance Graph and analyzing the Bias-Variance Tradeoff

## Overview
This repository implements key machine learning concepts including gradient descent optimization and the analysis of model bias and variance. The report and implementation provide a hands-on approach to understanding how model complexity affects performance and generalization.

## Task Descriptions

### Task 1: Gradient Descent
- **Goal**: Implement gradient descent to minimize the cost function for linear regression models.
- **Explanation**: Gradient descent is an optimization algorithm used to find the values of parameters (e.g., weights in linear regression) that minimize the cost function (e.g., Mean Squared Error). It works by iteratively adjusting the parameters in the direction of the negative gradient (the steepest descent) until the cost function reaches its minimum.

### Task 2: Numerical on Bias and Variance
- **Goal**: Perform theoretical calculations to understand how bias and variance change with different model complexities.
- **Explanation**: Bias refers to the error introduced by simplifying assumptions in the model, while variance measures how much the predictions vary with different training data. A model with high bias tends to underfit, and a model with high variance tends to overfit. This task helps in quantifying and understanding how the bias-variance tradeoff works.

### Task 3: Calculating Bias and Variance
- **Goal**: Calculate bias and variance for models of varying complexity, specifically polynomial models of different degrees.
- **Explanation**: By calculating bias and variance for polynomial regression models of different degrees, we can observe how the complexity of the model affects these two components of error. A low-degree polynomial may have high bias (underfitting), while a high-degree polynomial may have high variance (overfitting). The goal is to balance bias and variance to build a model that generalizes well.

### Task 4: Calculating Irreducible Error
- **Goal**: Calculate and discuss the irreducible error of a model.
- **Explanation**: The irreducible error is the noise in the data that cannot be eliminated by any model. This error is intrinsic to the problem and independent of the model used. While increasing model complexity can reduce bias and variance, it cannot reduce the irreducible error, which sets a fundamental limit on model performance.

### Task 5: Plotting Bias² - Variance Graph and Analyzing the Bias-Variance Tradeoff
- **Goal**: Visualize the bias-variance tradeoff by plotting the Bias² - Variance graph.
- **Explanation**: This task involves plotting a graph that shows the relationship between bias² and variance for different model complexities. The bias-variance tradeoff is a key concept in machine learning, where a model can either underfit (high bias) or overfit (high variance). The optimal model complexity is the point where bias and variance are balanced, leading to good generalization. This task helps in identifying underfitting and overfitting behavior and understanding how to select the right model complexity for a given problem.

## Tech Stack

### 1. **Programming Language**
   - **Python**: The primary programming language used for implementing the models and analysis in this project.

### 2. **Libraries and Frameworks**
   - **Numpy**: Used for numerical computations and array manipulations.
   - **Matplotlib**: Used for plotting various graphs, including the Bias² - Variance tradeoff graph, Bias, Variance, and Irreducible Error plots.
   - **Scikit-learn**: 
     - **LinearRegression**: Used to fit linear regression models for training and predictions.
     - **PolynomialFeatures**: Used to transform the input features to polynomial features for different degrees (up to degree 10).
   - **PrettyTable**: Used for creating and displaying tables for the bias, variance, and irreducible error values for different model complexities.

### 3. **Data Processing**
   - **Pickle**: Used to load the dataset (`data.pickle`) containing the training and test data, ensuring compatibility with Python objects.
   - **Numpy**:
     - Used to manipulate and shuffle the data, as well as to split the training dataset into 15 equal parts.
     - Arrays were used to store and calculate bias, variance, mean squared error (MSE), and irreducible error.

### 4. **Task-Specific Methods**
   - **Gradient Descent**: While this specific assignment focuses on bias-variance tradeoff, gradient descent was used in related parts of the project (outside the provided script) to minimize error functions and optimize model parameters.
   - **Polynomial Regression**: Polynomial models of degrees ranging from 1 to 10 were used to observe how model complexity affects bias, variance, and MSE.
   - **Bias and Variance Calculation**: Bias, variance, and irreducible error were calculated using model predictions across multiple training sets, with the errors computed based on the test set.
   - **MSE Calculation**: MSE was calculated for each model to measure performance, and the resulting values were stored for later analysis.

### 5. **Visualization**
   - **Bias-Variance Tradeoff Graph**: Plotted the relationship between bias², variance, and MSE, showing the tradeoff as the degree of the polynomial model increases.
   - **Bias and Variance Plots**: Individual plots for bias, variance, and irreducible error to understand how each varies with model complexity.
   - **Irreducible Error Plot**: Visualized the irreducible error as a function of the polynomial degree, showing how it behaves irrespective of model complexity.

### 6. **Output and Reports**
   - **Tables**: Bias, variance, irreducible error, and MSE for each model were presented in tabular form using `PrettyTable`, providing a clear summary for each degree of the polynomial model.
   - **Plots**: Multiple plots were created using Matplotlib to visualize and analyze the behavior of the model as complexity changes.

### 7. **Data Sources**
   - The data used in this project was provided in a pickle file (`data.pickle`), containing both the training and test datasets.
