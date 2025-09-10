# Linear Regression Implementation: Gradient Descent and Normal Equation

This project demonstrates the implementation of linear regression using both gradient descent and the closed-form (normal equation) solution across two distinct problems.

## Problems Overview

### Problem 1: Linear Regression on D3 Dataset
Implements multivariate linear regression using gradient descent to predict a target variable based on three input features from the `D3.csv` dataset.

### Problem 2: Predicting Website Visitor Spending
Uses the normal equation to predict the dollar amount visitors will spend on dongles-r-us.com based on their browsing behavior (time on page, mouse movement, and scrolling).

## Features

### Problem 1 Implementation
- Implements multivariate linear regression with three input features
- Uses gradient descent optimization with feature scaling
- Visualizes convergence through cost function plotting
- Compares results with closed-form solution for verification
- Makes predictions for new input samples

### Problem 2 Implementation
- Applies the normal equation for direct parameter computation
- Analyzes website visitor behavior data (11 customers)
- Includes multiple verification methods (lstsq, pseudoinverse)
- Provides clear interpretation of learned coefficients

## Workflow

### Problem 1: Gradient Descent Approach
1. **Data Preparation**
   - Load D3.csv dataset and separate features/target
   - Standardize features for efficient gradient descent

2. **Model Training**
   - Add bias (intercept) term to feature matrix
   - Implement gradient descent with learning rate α = 0.01
   - Track cost function over 20,000 iterations

3. **Verification & Prediction**
   - Convert coefficients back to original scale
   - Compare with closed-form solution
   - Make predictions for specified test inputs

### Problem 2: Normal Equation Approach
1. **Data Setup**
   - Organize visitor data: time, jiggle, scroll, sales
   - Construct design matrix with intercept column

2. **Direct Solution**
   - Apply normal equation: θ = (X^T X)^(-1) X^T y
   - Verify results using alternative methods

3. **Analysis**
   - Interpret coefficients for business insights
   - Validate solution consistency across methods

## Technologies Used

- **Python 3.x**
- **NumPy** - Matrix operations and mathematical computations
- **Pandas** - Data loading and manipulation
- **Matplotlib** - Cost function visualization
- **Jupyter Notebook** - Interactive development and presentation

## Dataset Information

- **D3.csv**: Contains numerical data for Problem 1 regression analysis
- **Visitor Data**: 11-customer dataset with time, jiggle, scroll, and sales metrics

## How to Run

1. **Install dependencies:**
   ```bash
   pip install numpy pandas matplotlib notebook
   ```

2. **Start Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

3. **Open `linearRegression.ipynb`** and run cells sequentially to:
   - Execute Problem 1: gradient descent implementation
   - Execute Problem 2: normal equation solution
   - View results, plots, and verification

## Results Summary

### Problem 1 Final Model
- Successfully implements gradient descent with convergence verification
- Achieves coefficient matching between gradient descent and normal equation
- Provides predictions for three test cases

### Problem 2 Final Model
- **Baseline spending**: ~2626 cents when all variables are zero
- **Time effect**: +0.42 cents per additional second on page
- **Mouse activity effect**: +12.72 cents per cm of mouse movement
- **Scroll effect**: -6.50 cents per cm of scrolling (negative correlation)

---

## Academic Note
This project includes proper AI assistance disclosure and follows all assignment requirements including feature scaling, bias terms, convergence verification, and closed-form solution comparison.

**Status**: ✅ Complete - Both problems implemented with full mathematical derivations and code verification