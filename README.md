
# FinTech Credit Risk Engine: Automated Loan Decisioning 

![Python](https://img.shields.io/badge/Language-Python-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Financial Risk](https://img.shields.io/badge/Focus-Credit%20Scoring-red)

##  Project Overview
As an experienced Audit Manager, I developed this **Credit Risk Engine** to solve the primary challenge in digital lending: distinguishing between safe borrowers and high-risk defaulters. This project moves beyond simple "Yes/No" classification by generating a **300-1000 Credit Score**, enabling risk-based pricing and automated approvals similar to systems used by top Nigerian FinTechs.

##  Advanced Methodology
* **Handling Data Imbalance (SMOTE):** In banking, defaulters are a minority. I implemented **SMOTE (Synthetic Minority Over-sampling Technique)** to balance the dataset, ensuring the model identifies "Bad" loans with high precision.
* **Algorithm:** Utilized a **Random Forest Classifier** to capture non-linear relationships in financial behavior (e.g., how age and loan duration interact to create risk).
* **Scorecard Engineering:** Developed a custom mapping function to transform model probabilities into a standard credit scoring scale (300 - 1000).



##  Key Audit Insights (Feature Importance)
The model identified the following as the top 3 drivers of credit risk:
1. **Checking Account Status:** The most critical indicator of immediate liquidity.
2. **Loan Duration:** Longer-term commitments showed a statistically significant increase in default probability.
3. **Credit History:** Past reliability remains a powerful predictor of future performance.



##  The Business Impact: The "Risk Scorecard"
Instead of a "Black Box" decision, this engine provides a **transparent risk score**:
* **Score > 700:** Automatic Approval (Low Risk)
* **Score 500 - 700:** Manual Audit Required (Medium Risk)
* **Score < 500:** Automatic Rejection (High Risk)

##  Files in this Repo
* `credit_risk_modeling.ipynb`: Complete pipeline from data balancing to scorecard generation.
* `risk_drivers.png`: Visualization of top factors impacting the credit score.
* `requirements.txt`: Necessary libraries (including `imblearn` for SMOTE).
