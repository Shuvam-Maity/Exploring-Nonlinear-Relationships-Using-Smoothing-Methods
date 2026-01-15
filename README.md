# Exploring Nonlinear Relationships Using Smoothing Methods

## 📌 Project Overview
This project investigates the **nonlinear and saturating relationship between GDP per capita and life expectancy at birth** using real-world socioeconomic data. Traditional linear regression models fail to capture this pattern, motivating the use of **nonparametric smoothing techniques** that adapt flexibly to the data without imposing a fixed functional form.

The study evaluates multiple smoothing methods and demonstrates how bias–variance trade-offs influence predictive performance.

---

## 📊 Dataset
- **Source:** Our World in Data  
- **Observations:** 1,400+ country–year records after cleaning  

### Features Used
- **GDP per capita** (independent variable)  
- **Life expectancy at birth** (dependent variable)

### Data Preprocessing
- Removed missing values
- Filtered outliers using the **Interquartile Range (IQR)** method
- Standardized variables where required for fair model comparison

---

## 🔧 Methodology
1. Conducted exploratory data analysis to identify nonlinear trends
2. Applied the following nonparametric regression techniques:
   - Bin Smoothing
   - K-Nearest Neighbors (KNN) Smoothing
   - LOESS
   - Kernel Regression
3. Performed **5-fold cross-validation** for hyperparameter tuning
4. Evaluated models using:
   - Mean Squared Error (MSE)
   - Mean Absolute Error (MAE)
5. Compared models based on:
   - Predictive accuracy
   - Smoothness
   - Interpretability

---

## ✅ Key Results
- **Kernel Regression** with an **Epanechnikov kernel** and bandwidth **0.10** achieved the lowest test error.
- The relationship exhibits a clear **saturation effect**:
  - Rapid gains in life expectancy at low income levels
  - Diminishing returns at higher GDP per capita
- Results align with established economic theory, particularly the **Preston Curve**.

---

## 📈 Visualizations
The project includes:
- Scatter plots with smoothed regression curves
- Model comparison plots across smoothing techniques
- Cross-validation error vs. bandwidth/parameter plots

---

## 🛠 Tools & Technologies
**Languages:**  
- R  
- Python  

**Libraries:**  
- NumPy  
- Pandas  
- SciPy  
- scikit-learn  
- statsmodels  
- Matplotlib  

**Techniques:**  
- Nonparametric Regression  
- Cross-Validation  
- Hyperparameter Tuning  
- Data Visualization  
