# Feature-Engineering-to-Predicted-Freight-Delay-Risk
Engineered logistic and financial features to build a Random Forest model that predicts freight delivery delays using supply chain data. The model enabled risk-based insurance pricing, calculating premiums that balance expected claims, fixed costs, and profit margins.

## Objectives:
- Predict whether a shipment would be **late**, based on information available **at the time of purchase**.
- Calculate a **risk-based insurance premium** that considers:
  - Expected claims
  - Fixed administrative expenses
  - Profit margins

## Feature Engineering Summary
These features added predictive power beyond the raw dataset, aligning with real-world shipment risks and behavior patterns.

| Engineered Feature               | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| `Average Customer Order Value`           | Sales per order, calculated from order item totals.                |
| `Discount Impact`               | Estimated financial impact of discounts on order profitability.             |
| `Order Value per Quantity`      | Normalized order value by quantity to detect order complexity.              |
| `Order Value to Quantity Ratio` | Captures efficiency of value shipped per unit ordered.                      |
| `Avg. Sales per Customer Segment`             | Average sales segmented by customer or product group to reflect priority.   |

![Visualization FE](https://github.com/SalazarHerna/Feature-Engineering-to-Predicted-Freight-Delay-Risk/blob/43ea897b1f39c22d0b7a6d8c41e0fd4dd85c8294/Document%20%26%20Code/Feature%20Engineering%20for%20Freight%20Delays%20Prediction.jpeg)

---
## Key Outcomes
- Built a **Random Forest Classifier** using both original and engineered features to classify freight delay risk.
- Achieved **63.75% accuracy**, with strong **precision and recall** for late deliveries, making the model a reliable predictor of potential claims.
- Calculated a **personalized insurance premium.
  
## Insights
- **Feature engineering** was central to model success, enhancing model depth and interpretability.
- Predictive features like `Discount Impact` and `Order Value to Quantity Ratio` captured underlying financial and logistic patterns affecting delay risk.
- Insurance premiums increase **linearly with profit loading**, giving actuaries flexibility in balancing profitability with competitiveness.

### Strategic Takeaway
This approach shows that **smart feature engineering combined with machine learning** enables scalable, data-driven insurance pricing—even in complex, logistics-heavy markets.

![Visualization EC](https://github.com/SalazarHerna/Feature-Engineering-to-Predicted-Freight-Delay-Risk/blob/263bcc992b9f74743ac14e5d06d0e54250052efc/Document%20%26%20Code/Expected%20Claims%20and%20Premium%20Over%20Time.jpeg)

---
## Tools Used

| Task                        | Tools & Libraries                     |
|-----------------------------|---------------------------------------|
| Data Cleaning & Wrangling   | `pandas`, `NumPy`                     |
| Visualization               | `matplotlib`, `seaborn`               |
| Modeling                    | `scikit-learn` (`RandomForestClassifier`) |
| Feature Engineering         | Custom logic, domain intuition        |
| Outlier Detection           | Z-Score, IQR                          |
| Notebook Environment        | Jupyter Notebook                      |

---
## Steps to Engineer Features and Build Prediction Model
#### Step 1: Data Preparation
#### Step 2: Feature Engineering
#### Step 3: Model Training
  - **Random Forest Classifier** due to:
  - Dedine Model Assumptions:**
#### Step 4: Performance Evaluation
- **Accuracy:** 63.75%
- **Precision & Recall:** Stronger for predicting **late deliveries (Class 1)**
- Conclusion: Model is effective for **real-world claim prediction and premium setting**
#### Step 5: Insurance Premium Calculation

## Conclusions & Recommendations
This project demonstrates the power of **feature engineering combined with machine learning** to deliver intelligent, risk-based insurance pricing models:
- Personalized pricing improves **fairness** and **business sustainability**
- Predictive modeling reduces **exposure to high-risk claims**
- Feature-rich models lead to **stable and justifiable premium structures**

