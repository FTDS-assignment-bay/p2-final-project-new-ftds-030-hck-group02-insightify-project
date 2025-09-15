# Insightify – Causal Inference for Marketing Campaign Effectiveness

## 📌 Description
Insightify is an analytics application that leverages causal inference to evaluate the effectiveness of marketing campaigns.
The system measures the true impact of campaigns on customer spending behavior using demographic, transaction, and product category data.

With Insightify, businesses can:

Identify the best customer segments for campaigns.
Determine the optimal timing for campaigns.
Design strategies to improve Return on Investment (ROI).

---

## 🎯 Project Objectives
1.Estimate the causal impact of campaigns (Average Treatment Effect / ATE).
2.Explore heterogeneity of effects (CATE/ITE) across segments or individuals.
3.Predict whether a campaign is on target or off target for a customer.
4.Build an interactive application (Streamlit/HuggingFace) for prediction simulation.

---

## ⚙️ Methodology
1. Variable Identification
   - Treatment: campaign participation.
   - Outcome: customer spending.
   - Confounders: demographics, historical transactions, product categories.
   - Effect Estimation (Backdoor Adjustment)

2. OLS Regression Adjustment.
   - Propensity Score Matching (PSM).
   - Inverse Probability Weighting (IPW).
   - Doubly Robust (DR Learner).
   - Heterogeneous & Individual Effects

3. Causal Forest (CATE/ITE).
   - Customer segmentation based on causal effects.
   - Business Insights

4. Segments most influenced by the campaign.
   - Optimal campaign timing.
   - ROI estimation.
   - Deployment

5. Streamlit/HuggingFace App:
   - Input: user attributes (age, income, historical spending, product categories).
   - Output: prediction of whether the campaign is on target along with the estimated uplift.

---

## 🛠️ Requirements
- Python 3.10+
- Libraries utama:
     - `pandas`, `numpy`, `matplotlib`, `seaborn`
     - `scikit-learn`
     - `dowhy`, `econml`
     - `pymc`
     - `streamlit`

Instalasi dengan Conda:
```bash
conda env create -f environment.yml

conda activate insightify
