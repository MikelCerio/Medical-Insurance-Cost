# 🔍 Predictive Analysis of Medical Insurance Costs

This project explores a structured dataset of medical insurance records to identify the main drivers behind insurance costs and build an interpretable predictive model using Python and Scikit-Learn.

---

## 🎯 Objective

The goal is to determine which factors most influence medical insurance charges and to develop a simple yet effective linear regression model for estimating those costs. The output can help insurers make smarter decisions and design more personalized premiums.

---

## 📊 Dataset Overview

- **Records:** 1,338 individuals
- **Features:**
  - `age`
  - `sex`
  - `bmi` (Body Mass Index)
  - `children`
  - `smoker` (yes/no)
  - `region`
  - `charges` (target)

The dataset contains no missing values and is balanced and ready for modeling.

---

## 📈 Exploratory Analysis

- **Age** and **BMI** show a moderate correlation with insurance costs.
- **Smoker status** has a massive impact — the key driver of high costs.
- Features like **region** or **number of children** have very limited predictive power.

---

## 🧠 Predictive Model

- **Algorithm:** Linear Regression
- **Feature Engineering:** OneHot Encoding for categorical variables
- **Performance:**
  - Mean Absolute Error (MAE): ~€4,181
  - R² Score: 0.78 (explains 78% of the cost variability)

### Most impactful variables:
| Variable      | Effect         |
|---------------|----------------|
| `smoker=yes`  | +€23,651       |
| `age`         | +€256 per year |
| `bmi`         | +€337 per point|

---

## 📊 Advanced Visuals

- Smoking dramatically increases charges, especially after age 30.
- High BMI combined with smoking = explosive cost risk.
- High-cost cluster detected: age 45–60, BMI >30, smokers.

---

## 🧾 Final Conclusion

> The highest-risk profile is a smoker aged 45–60 with a BMI over 30.  
> Quitting smoking could save up to €23,000 per person in insurance costs.

---

## 💡 Recommendations

- Use this model as a base for personalized pricing.
- Promote health campaigns targeting smoking and obesity.
- Focus interventions in high-risk demographic clusters.

---

## 🛠 Tech Stack

- Python
- Pandas, Seaborn, Matplotlib
- Scikit-Learn
- Jupyter Notebooks or Streamlit (for interactive visualizations)

---

## 👤 Author

**Mikel Cerio**  
Project built as part of a data science portfolio and advanced analytics training.

