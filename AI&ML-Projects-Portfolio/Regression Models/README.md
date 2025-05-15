# Linear and Polynomial Regression

This project compares linear and polynomial regression methods on two synthetic datasets using both manual and library implementations.

## 📊 Dataset Description
- **Dataset 1**: Linear function + Gaussian noise
- **Dataset 2**: Nonlinear function + Gaussian noise
- **Split**: 50% training, 50% validation

## 🧠 Models & Implementations

### Linear Regression
- **Scikit-learn** LinearRegression model
- **Manual OLS**: using matrix pseudoinverse
- **Manual Gradient Descent**: custom implementation with MSE loss

### Polynomial Regression
- **Polynomial Degrees Tested**: 1, 3, 5, 7
- **Manual degree-3 implementation** for comparison
- Used NumPy to expand features

## 🧪 Evaluation
- Mean Squared Error (MSE) computed for all models
- Plots of regression line fits on training/validation sets
- Underfitting vs overfitting observed across polynomial degrees

## 🛠️ Tech Stack
Python, NumPy, Scikit-learn, Matplotlib

## 🚀 How to Run
1. Run the notebook in Jupyter or Colab
2. Compare line fits, errors, and loss curves across model types
