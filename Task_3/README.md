#  Predicting Insurance Claim Amounts using Linear Regression

This project builds a linear regression model to predict medical insurance charges based on various factors like age, sex, BMI, number of children, smoking status, and region. 

---

##  Dataset

* **Source**: [Kaggle - Insurance Dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)
* **Features**:

  * `age`: Age of primary beneficiary
  * `sex`: Insurance contractor gender (male/female)
  * `bmi`: Body mass index
  * `children`: Number of children covered by health insurance
  * `smoker`: Smoking status
  * `region`: Residential area in the US
  * `charges`: Medical costs billed by health insurance

---

##  Project Steps

###  1. Data Preprocessing

* Loaded the CSV dataset
* Checked for missing values
* Converted categorical variables (`sex`, `smoker`, `region`) into numerical values

###  2. Exploratory Data Analysis (EDA)

* **Scatter Plots**:

  * Age vs Charges
  * BMI vs Charges
* **Bar Plot**:

  * Average Charges: Smokers vs Non-Smokers
* **Heatmap**:

  * Feature correlation

###  3. Model Training

* Used **Linear Regression**
* Split dataset (80% training, 20% testing)
* Trained using `scikit-learn`

###  4. Evaluation Metrics

* **MAE (Mean Absolute Error)**: `$4186.51`
* **RMSE (Root Mean Squared Error)**: `$5799.59`
* **R² Score (Accuracy)**: `0.7833`

###  5. Visualizations

* Actual vs Predicted Charges (scatter plot)
* Prediction Error Distribution (histogram)
* Feature Importance (bar chart)

### 6. Real-World Prediction Example

Predicted charges for a:

* 35-year-old male smoker
* BMI: 28.5
* 2 children
* Living in the Northwest

 **Estimated Charges**: `$30,828.06`

 *This prediction aligns well with the average smoker charges, indicating that the model is performing realistically and can provide useful estimates in real-life cases.*

---

##  Averages Comparison

* **Overall Average**: `$13,270.42`
* **Smokers Average**: `$32,050.23`
* **Non-Smokers Average**: `$8,434.27`

---

##  Feature Importance (Coefficient Values)

* `smoker`: **23647.82** → Highest impact on charges
* `children`: 425.09
* `bmi`: 335.78
* `region`: 271.28
* `age`: 257.06
* `sex`: -18.79

---

##  Conclusion

The model achieved a good R² score of **78.33%**, showing strong predictive power. Smoking, age, and BMI are key contributors to insurance charges. This model can help insurance companies set personalized premiums fairly.

---

##  Future Improvements

* Try other models like Decision Tree or Random Forest for better results
* Use more data to improve the model
* Handle outliers to make predictions more accurate
* Add new features (like BMI category) for deeper analysis
* Tune model settings to improve accuracy

---

## 💻 Requirements

```bash
pandas
numpy
matplotlib
seaborn
scikit-learn
```

---

## 📂 How to Run

1. Clone this repo
2. Ensure `insurance.csv` is in the root folder
3. Run the notebook 

---

## 📬 Author

**Gulam Zuhra**
Internship Project — Data Science

---
