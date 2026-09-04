# Linear Regression

A simple implementation and exploration of **Linear Regression** using a salary dataset with years of experience as the input feature and salary as the target.

This repository contains two approaches:

* Linear Regression implemented **from scratch**
* Linear Regression using **Scikit-learn**

## Dataset

The dataset contains:

* `YearsExperience` — years of work experience
* `Salary` — corresponding salary

The dataset contains **30 observations**, with experience ranging from **1.1 to 10.5 years**.

## Linear Regression From Scratch

`LinearRegression_from_scratch.ipynb`

The model is implemented using NumPy without using a machine learning library for the regression algorithm.

It includes:

* Mean and variance calculation
* Feature normalization
* Custom `SimpleLR` class
* Weight and bias initialization
* Gradient descent
* Loss calculation and tracking
* Regression visualization

The implementation uses a learning rate of `0.1` and a maximum of `2000` iterations.

The recorded training run reduced the loss substantially, ending at approximately **15.64 million**.

## Linear Regression Using Scikit-learn

`LinearRegression_using_scikit_learn.ipynb`

The second notebook uses Scikit-learn's `LinearRegression` implementation to train the model and make salary predictions.

### Model Results

| Metric      |         Result |
| ----------- | -------------: |
| R² Score    |    **0.95696** |
| Coefficient | **144,419.01** |
| Intercept   |  **76,003.00** |

The model's predicted salaries are generated from normalized years of experience.

## Tools & Libraries

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
Linear_Regression/
│
├── data/
│   └── Salary_Data.csv
│
├── notebooks/
│   ├── LinearRegression_from_scratch.ipynb
│   └── LinearRegression_using_scikit_learn.ipynb
│
└── README.md

## Purpose

The project demonstrates the fundamentals of Linear Regression by comparing a custom implementation with Scikit-learn's implementation.
