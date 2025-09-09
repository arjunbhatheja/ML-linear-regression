# Linear Regression with Gradient Descent and Normal Equation

This project demonstrates the application of linear regression using both gradient descent and the closed-form (normal equation) solution. The dataset (`D3.csv`) contains three explanatory variables and one dependent variable.

## Features

- Implements multivariate linear regression with three input features.
- Uses gradient descent to fit the model and visualize convergence.
- Applies feature scaling for efficient optimization.
- Predicts target values for new input samples.
- Computes the closed-form solution for comparison.

## Workflow

1. **Data Preparation**
   - Load the dataset and separate features and target.
   - Standardize features for gradient descent.

2. **Model Training**
   - Add a bias (intercept) term to the feature matrix.
   - Fit the model using gradient descent.
   - Track and plot the cost function to verify convergence.

3. **Prediction**
   - Use the trained model to predict target values for new inputs.
   - Convert coefficients back to the original scale if features were standardized.

4. **Closed-Form Solution**
   - Compute model parameters using the normal equation for verification.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook (recommended for step-by-step explanations and visualization)

## How to Run

1. Install dependencies:
   ```
   pip install numpy pandas matplotlib notebook
   ```
2. Start Jupyter Notebook:
   ```
   jupyter notebook
   ```
3. Open the notebook and follow the steps to run the code and view results.

---

This project provides a clear, step-by-step approach to understanding and implementing linear regression for multivariate data.
