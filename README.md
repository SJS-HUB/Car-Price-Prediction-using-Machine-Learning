# 🚗 Car Price Prediction using Machine Learning

## 📌 Objective
Build a regression model to predict the selling price of used cars based on features such as car age, fuel type, seller type, and transmission type. This project aims to assist used car dealerships in pricing vehicles more accurately.

---

## 📁 Dataset
- **Source**: [Mention the source or say “provided dataset” if unavailable]
- **Description**: Contains details of used cars including:
  - `Year` – Manufacturing year
  - `Present_Price` – Current ex-showroom price (in lakhs)
  - `Kms_Driven` – Kilometers driven
  - `Fuel_Type`, `Seller_Type`, `Transmission` – Categorical features
  - `Owner` – Number of previous owners
  - `Selling_Price` – Target variable

---

## 🛠️ Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (Linear Regression, train_test_split, model evaluation metrics)

---

## 📊 Workflow

### 1. Data Preprocessing
- Converted year to `car_age`
- Handled categorical features via encoding
- Removed irrelevant or redundant columns

### 2. Exploratory Data Analysis
- Visualized distribution of prices, fuel types, and seller types
- Analyzed correlations and feature relationships

### 3. Model Building
- Trained a **Linear Regression** model
- Evaluated performance using:
  - R² Score
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)

### 4. Key Insights
- Car age negatively correlates with price
- Diesel and manual cars had higher selling prices in dataset
- Dealer-sold cars were priced higher on average

---

## 📈 Results
- Achieved a reasonable R² score indicating good model fit
- Identified key price influencers: `Present_Price`, `car_age`, `Fuel_Type`, and `Transmission`

📈 Model Performance & Comparison
Several regression models were trained and evaluated using the R² Score:

Model	R² Score
Linear Regression	0.68
K-Nearest Neighbors	0.14
Decision Tree	0.70
Random Forest	0.85
![image](https://github.com/user-attachments/assets/ff8033af-3362-4abc-9049-d0aae2e22cb4)

🔍 Insights:
Random Forest Regressor delivered the best performance with an R² score of 0.85, capturing the most variance in car prices.

Linear Regression and Decision Tree performed moderately well, but were outperformed by Random Forest.

KNN showed poor performance, likely due to sensitivity to feature scaling and high dimensionality.

Ensemble methods like Random Forest are better suited for capturing non-linear relationships in car price prediction tasks
---

## 🔍 Next Steps
- Add more robust models: like XGBoost
- Perform hyperparameter tuning
- Deploy using Flask or Streamlit (future scope)

---

## 🧠 Learnings
- Applied end-to-end regression workflow from data ingestion to model evaluation
- Gained hands-on experience in EDA, preprocessing, and performance metrics

---

## 📎 How to Run
1. Clone this repository
2. Run the Jupyter Notebook:  
   `jupyter notebook P1_Car_price_prediction.ipynb`

---

## 🤝 Contributions & Feedback
Feel free to fork, suggest improvements, or contribute enhancements via pull requests.

---
