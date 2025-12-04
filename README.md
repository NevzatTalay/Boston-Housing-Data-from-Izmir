# 🏡 Boston Housing Prices Analysis Project

This project contains statistical analyses and data visualizations exploring the characteristics of the housing market in Boston and the factors influencing the median home value, based on the Boston Housing Dataset.

---

## 🎯 Project Goal

The primary objective is to understand the relationships between the median value of owner-occupied homes (**MEDV**) and various environmental and socioeconomic factors in Boston. This involves conducting descriptive analysis and using statistical hypothesis testing to determine the significance of these relationships.

---

## 💾 Dataset Overview (Boston Housing Dataset)

The dataset used contains **506 observations** and **14 variables** related to different tracts of land in the Boston area, collected in the 1970s.

### Dataset Variables

| Variable | Description |
| :--- | :--- |
| **CRIM** | Per capita crime rate by town |
| **ZN** | Proportion of residential land zoned for lots over 25,000 sq.ft. |
| **INDUS** | Proportion of non-retail business acres per town |
| **CHAS** | Charles River dummy variable (1 if tract bounds river; 0 otherwise) |
| **NOX** | Nitric oxides concentration (parts per 10 million) |
| **RM** | Average number of rooms per dwelling |
| **AGE** | Proportion of owner-occupied units built prior to 1940 |
| **DIS** | Weighted distances to five Boston employment centres |
| **RAD** | Index of accessibility to radial highways |
| **TAX** | Full-value property-tax rate per \$10,000 |
| **PTRATIO** | Pupil-teacher ratio by town |
| **LSTAT** | % lower status of the population |
| **MEDV** | Median value of owner-occupied homes in \$1000's |

---

## 🛠️ Tools and Libraries Used

* **Language:** Python
* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `seaborn`, `matplotlib.pyplot`
* **Statistics & Modeling:** `scipy.stats`, `statsmodels.api`

---

## 📊 Analytical Tasks

The project is structured around two main tasks:

### Task 1: Descriptive Statistics and Visualizations

Visualizations were generated to explore the distribution and initial relationships of key variables:

* Boxplot for **MEDV** (Median value of owner-occupied homes).
* Bar plot for **CHAS** (Charles River variable).
* Boxplot for **MEDV** vs. **AGE** (Discretized into three groups).
* Scatter plot for the relationship between **NOX** (Nitric oxide concentration) and **INDUS** (Non-retail business acres).
* Histogram for the **PTRATIO** (Pupil-teacher ratio) variable.

### Task 2: Statistical Hypothesis Testing

The following hypotheses were tested using the appropriate statistical methods at an $\alpha = 0.05$ significance level:

1.  **T-Test:** Is there a significant difference in **MEDV** for houses bounded by the Charles River?
2.  **ANOVA:** Is there a difference in **MEDV** across the three groups of the **AGE** variable?
3.  **Pearson Correlation:** Is there a significant relationship between **NOX** and **INDUS**?
4.  **Simple Linear Regression:** What is the impact of **DIS** (weighted distance) on **MEDV**?

---

## 🚀 How to Run the Analysis

To run this analysis, you must have the necessary Python libraries installed and the `boston_housing.csv` data accessible.

```bash
# Install the required libraries
pip install pandas numpy seaborn scipy statsmodels
