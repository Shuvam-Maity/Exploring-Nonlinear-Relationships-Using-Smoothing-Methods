# Exploring-Nonlinear-Relationships-Using-Smoothing-Methods

# 📌 Project Overview

This project explores the nonlinear and saturating relationship between GDP per capita and life expectancy at birth using real-world socioeconomic data. Traditional linear models fail to capture this pattern, so nonparametric smoothing techniques are applied to model the relationship flexibly without assuming a fixed functional form.

The analysis demonstrates how different smoothing methods handle bias–variance trade-offs and identifies the most effective approach through systematic evaluation.

# 📊 Dataset

=>Source: Our World in Data

=>Observations: 1,400+ country-year records after cleaning

=>Features Used:

>GDP per capita (independent variable)

>Life expectancy at birth (dependent variable)

>Missing values were removed and outliers were filtered using the Interquartile Range (IQR) method to ensure robust modeling.

# 🔧 Methodology

>Performed exploratory data analysis to identify nonlinear trends.

>Applied nonparametric regression techniques:

>Bin Smoothing

>K-Nearest Neighbors Smoothing

>LOESS

>Kernel Regression

>Used 5-fold cross-validation for hyperparameter tuning.

>Evaluated models using Mean Squared Error (MSE) and Mean Absolute Error (MAE).

>Compared models based on predictive accuracy, smoothness, and interpretability.

# ✅ Key Results

>The Kernel Regression model using the Epanechnikov kernel with bandwidth 0.10 achieved the lowest test error.

>Results confirm a saturating nonlinear relationship, where life expectancy increases rapidly at low income levels and flattens at higher GDP levels.

>The findings are consistent with established economic theory, including the Preston Curve.

# 🛠 Tools & Technologies

Languages: R, Python

Libraries: NumPy, Pandas, SciPy, scikit-learn, statsmodels, Matplotlib

Techniques: Nonparametric Regression, Cross-Validation, Hyperparameter Tuning, Data Visualization

# 📌 Conclusion

This project highlights the effectiveness of nonparametric smoothing methods for modeling complex real-world relationships. It demonstrates the importance of careful hyperparameter tuning and model evaluation to balance flexibility and generalization.
