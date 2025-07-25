<h1 align="center">Credit Risk Management and Client Analysis</h1>

<p align="center">
  <img src="https://imgs.search.brave.com/xK0kGwfVCDsY0WCLvOefP-9V7t1OCxdxzbVJZE47Dok/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly90aHVt/YnMuZHJlYW1zdGlt/ZS5jb20vYi9jcmVk/aXQtcmlzay1tYW5h/Z2VtZW50LXNob3du/LXVzaW5nLXRleHQt/cGhvdG8tZG9sbGFy/cy1jcmVkaXQtcmlz/ay1tYW5hZ2VtZW50/LXNob3duLXVzaW5n/LXRleHQtcGhvdG8t/MjYxMjAyMTQ0Lmpw/Zw" alt="Probability-Based Risk Scoring Diagram" width="600"/>
</p>

## 🔍 Overview

This project demonstrates how **machine learning** can power smarter, faster, and more inclusive credit risk assessment in fintech platforms. Using the publicly available **German Credit Dataset**, we explore how financial and demographic data can be used to build predictive models that assess the likelihood of default — especially for **young professionals**, a large but high-risk customer segment.

---

## 🎯 Objective

To build a **credit risk classification model** that:

- Predicts whether a customer is likely to default on a loan.
- Enables **automated, real-time lending decisions**.
- Moves beyond binary classification (0 or 1) to more **granular, probability-based scoring** that mirrors real-world credit scoring systems like FICO or Upstart.

---

## 🛠️ What I Did

- Conducted **EDA (Exploratory Data Analysis)** to uncover key patterns related to age, credit duration, account balance, and marital status.
- Trained a **Random Forest Classifier** using selected features such as:
  - Age group
  - Duration of credit
  - Account balance
  - Number of credits
  - Marital status and gender
- Evaluated model performance:
  - ✅ Accuracy: 77%
  - ✅ Precision (Class 1): 81%
  - ✅ Recall (Class 1): 85%
  - ✅ F1-Score: 83%
- Proposed **risk-band based probability scoring** instead of binary output — making lending decisions more flexible and data-driven.

---

## 📈 Results

- Long-term loans showed up to **51% default rate**, compared to 21% for short-term loans — reinforcing the need for **credit product design** based on risk segments.
- Customers with **no checking account** or **no balance** had 40–50% default rates.
- **Young customers (<25)** had the highest bad credit rate (41.33%) despite smaller loans — signaling opportunity and risk.

---

## 🚀 Future Potential & Real-World Use Case

This system forms the backbone for a **modern credit engine** that fintech companies can scale to production. With proper upgrades, it can:

- Offer **starter credit products** with lower limits to risky segments like young professionals.
- Assign **credit limits dynamically** based on probability of default.
- Use **behavioral nudges and rewards** to improve repayment patterns.
- Integrate with real-time financial data sources (e.g., UPI, utility bills, e-commerce behavior).

---

## 🧠 To-Do (Planned Updates)

- [ ] **Replace binary labels (0 = No Default, 1 = Default)** with **calibrated probability scores** using `.predict_proba()` from classifiers.
    - Enables decisions like:  
      - **< 0.45** → Low Risk → Fast-track approval  
      - **0.45–0.75** → Medium Risk → Manual review  
      - **> 0.75** → High Risk → Reject or restrict
- [ ] Introduce **XGBoost / LightGBM** models for higher accuracy.
- [ ] Add new features: employment status, loan purpose, credit utilization ratio.
- [ ] Implement **SHAP / LIME** for explainability (required for regulatory use).
- [ ] Build a **full API pipeline** for model deployment.
- [ ] Add **K-Means or segmentation model** for borrower personas.

---

## 📄 Resources

- 📘 [📑 Full Report (PDF)](https://github.com/lakshit2508/Credit-Risk-Management-and-Client-analysis/blob/main/Credit%20Risk%20Model%20Report.pdf)
- 🧪 [🔗 Model Code (Colab)](https://colab.research.google.com/github/lxshit1/Credit-Risk-Management-and-Client-analysis/blob/main/Untitled6.ipynb#scrollTo=bFEfa56_yRxj)

---

## ✅ Final Note

This is a work in progress intended to evolve into a **production-ready credit decision system** tailored for fintech lenders. Contributions, suggestions, and forks are welcome!
