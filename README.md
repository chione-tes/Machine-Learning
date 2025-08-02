# Machine-Learning
Polynomial Regression on Combined Cycle Power Plant Dataset

This project applies **Polynomial Regression** to predict the net electrical power output (PE) of a Combined Cycle Power Plant using ambient variables such as temperature, exhaust vacuum, ambient pressure, and relative humidity. The dataset is sourced from the UCI Machine Learning Repository.
Dataset Overview

Source: [UCI Machine Learning Repository – Combined Cycle Power Plant](https://archive.ics.uci.edu/dataset/294/combined+cycle+power+plant)
Features:
  - `AT`: Ambient Temperature (°C)
  - `V`: Exhaust Vacuum (cm Hg)
  - `AP`: Ambient Pressure (millibar)
  - `RH`: Relative Humidity (%)
- **Target**:
  - `PE`: Net hourly electrical energy output (MW)

Objective

To build a **Polynomial Regression model (degree=2)** that accurately predicts the net power output of the power plant using environmental conditions. The pipeline includes feature scaling and polynomial expansion for improved modeling of non-linear relationships.

---

 Tech Stack

- **Language**: Python
- **Libraries**:
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn` (`LinearRegression`, `PolynomialFeatures`, `StandardScaler`, `train_test_split`, etc.)
  - `ucimlrepo` (to fetch UCI datasets easily)

---

Methodology

1. **Data Fetching**: Retrieved directly using `ucimlrepo` package.
2. **Preprocessing**:
   - Train-test split (80:20)
   - Polynomial feature generation (degree=2)
   - Feature standardization
3. **Modeling**: Linear Regression applied on transformed features.
4. **Evaluation**:
   - `R² Score` and `Mean Squared Error` for both training and test sets.
   - Scatter plots comparing Actual vs Predicted values.
