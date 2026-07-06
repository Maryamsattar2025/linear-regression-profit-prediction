# linear-regression-profit-prediction
# Linear Regression with One Variable

This repository contains my solution for the **Practice Lab: Linear Regression with One Variable** from the Machine Learning coursework. In this lab, I implemented the core parts of linear regression from scratch using Python and NumPy.

## Project Overview

The goal of this assignment is to build a simple **linear regression model** that predicts restaurant profit based on the population of a city.

The scenario is based on a restaurant franchise that wants to decide which cities are good candidates for opening a new branch. Using existing data from different cities, the model learns the relationship between **city population** and **restaurant profit**.

## Dataset

The dataset contains **97 training examples**.

* **Input feature (`x_train`)**: population of a city (in units of 10,000)
* **Target (`y_train`)**: profit of a restaurant in that city (in units of $10,000)

### Example

* `x = 6.1101` means the city population is **61,101**
* `y = 17.592` means the restaurant profit is **$175,920**

## What I Implemented

In this notebook, I completed the following graded functions:

### 1. `compute_cost(x, y, w, b)`

This function computes the **cost function** for linear regression:

* Calculates the predicted value for each training example
* Computes the squared error for each example
* Returns the average cost over the full dataset

### 2. `compute_gradient(x, y, w, b)`

This function computes the **gradients** of the cost function with respect to the model parameters:

* Computes prediction error for each training example
* Calculates gradient for:

  * `w` (slope)
  * `b` (intercept)
* Returns the averaged gradients used in gradient descent

## Gradient Descent

The notebook then uses **batch gradient descent** to learn the optimal values of `w` and `b`.

### Final learned parameters

* **w = 1.166362350335582**
* **b = -3.63029143940436**

These values define the best-fit line for the training data.

## Model Predictions

Using the trained model:

* For a city with population **35,000**, predicted profit is **$4,519.77**
* For a city with population **70,000**, predicted profit is **$45,342.45**

## Concepts Practiced

This lab helped me practice the following machine learning concepts:

* Linear regression with one variable
* Cost function calculation
* Gradient computation
* Batch gradient descent
* Model fitting and prediction
* Data visualization with Matplotlib

## Tools and Libraries Used

* **Python**
* **NumPy**
* **Matplotlib**
* **Jupyter Notebook**

## Files in this Project

* `C1_W2_Linear_Regression.ipynb` → main notebook containing the assignment solution
* `utils.py` → helper functions provided with the lab
* `README.md` → project overview and explanation

## Learning Outcome

By completing this assignment, I gained hands-on experience in implementing linear regression from scratch rather than relying on built-in machine learning libraries. This helped me understand how the cost function, gradients, and gradient descent work together to train a predictive model.

## Note

This project is part of my machine learning learning journey and portfolio. It demonstrates my understanding of the mathematical and programming foundations of supervised learning.
