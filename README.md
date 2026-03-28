# Canada Income Regression 

This project implements a univariate **Linear Regression** model to estimate Canada's per-capita income trend over time and predict the value for the year 2020 using the `canada_per_capita_income.csv` dataset.

## Project Objective
I build and evaluate a linear regression model that learns the relationship between **year** (independent variable) and **per-capita income** (dependent variable), then use it to predict income for a future year.

## Project Structure
- `canada_income_prediction.ipynb` — End-to-end notebook with preprocessing, model fitting, prediction, and visualization.
- `dataset/canada_per_capita_income.csv` — Input dataset.
- `README.md` — Project documentation.

## Theoretical Background

### 1) Linear Regression
Linear regression models a linear relationship between a feature $x$ and target $y$:

$$y = mx + c$$

Where:
- $m$ is the slope (model coefficient),
- $c$ is the intercept,
- $y$ is the predicted target value.

In this project:
- $x$ = year,
- $y$ = per-capita income (US$).

### 2) Model Fitting
The model finds $m$ and $c$ that minimize prediction error (typically through least squares), producing a best-fit regression line through the observed data points.

### 3) Prediction and Interpretation
After fitting, the model predicts income for year 2020. The coefficient indicates yearly change in income, while the intercept defines the baseline level when extrapolated to $x=0$.

## Workflow
1. Load dataset and rename the target column for convenience.
2. Visualize the year-income relationship.
3. Separate feature (`year`) and target (`per_capita_income`).
4. Train `LinearRegression` model.
5. Predict per-capita income for year 2020.
6. Inspect coefficient and intercept.
7. Plot actual data, regression line, and predicted point.

## Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib

## Author
**Manolina Das**  

