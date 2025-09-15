# Insightify – Causal Inference for Marketing Campaign Effectiveness

## 📌 Description
Insightify is an analytics application that leverages causal inference to evaluate the effectiveness of marketing campaigns.
The system measures the true impact of campaigns on customer spending behavior using demographic, transaction, and product category data.

With Insightify, businesses can:

- Identify the best customer segments for campaigns.
- Determine the optimal timing for campaigns.
- Design strategies to improve Return on Investment (ROI).

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

5. Streamlit App:
   - Input: user attributes (age, income, historical spending, product categories).
   - Output: prediction of whether the campaign is on target along with the estimated uplift.
   - Link Deployment : https://causalinferencemodel.streamlit.app/

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
```

---

👥 Project Team & Contributions

- Ilham Maulud – Data Analyst | [Github](https://github.com/ilhammaulud) | [LinkedIn](https://www.linkedin.com/in/ilham-maulud/)

   - Performed data cleaning and preparation.

   - Conducted Exploratory Data Analysis (EDA).

   - Created visualizations to identify customer behavior patterns and key insights.

- Nindia Ekasuci Larasati – Data Scientist | [Github](https://github.com/NindiaEka) | [LinkedIn](https://www.linkedin.com/in/nindia-ekasuci-larasati/)

   - Designed and implemented causal inference methodologies (ATE, CATE, ITE).

   - Applied methods: OLS Regression Adjustment, PSM, IPW, Doubly Robust Learner, and Causal Forest.

   - Built and deployed an interactive application using Streamlit for campaign effectiveness simulation.

- Muhammad Luthfi Alfatih – Data Engineer | [Github](https://github.com/upilup) | [LinkedIn](https://www.linkedin.com/in/luthfialfatih/)

   - Managed data integration and preprocessing to ensure data quality.

   - Prepared model artifacts and environment setup for deployment.

   - Ensured the Streamlit application runs smoothly in production.


