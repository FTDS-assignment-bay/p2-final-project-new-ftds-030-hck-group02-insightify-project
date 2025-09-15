# Insightify – Causal Inference for Marketing Campaign Effectiveness

## 📌 Deskripsi
Insightify adalah aplikasi analitik yang menggunakan **causal inference** untuk mengevaluasi efektivitas kampanye pemasaran.  
Sistem ini mengukur **dampak nyata kampanye** terhadap perilaku belanja pelanggan dengan memanfaatkan data demografi, transaksi, dan kategori produk.  

Dengan Insightify, bisnis dapat:
- Mengidentifikasi segmen pelanggan terbaik untuk kampanye.
- Menentukan waktu kampanye yang optimal.
- Merancang strategi untuk meningkatkan **Return on Investment (ROI)**.

---

## 🎯 Tujuan Project
1. Mengestimasi dampak kausal kampanye (Average Treatment Effect / ATE).  
2. Mengeksplorasi heterogenitas efek (CATE/ITE) per segmen atau individu.  
3. Memprediksi apakah campaign **on target** atau **off target** bagi seorang pelanggan.  
4. Membuat aplikasi interaktif (Streamlit/HuggingFace) untuk simulasi prediksi.  

---

## ⚙️ Metodologi
1. **Identifikasi Variabel**
   - Treatment: partisipasi campaign.
   - Outcome: spending pelanggan.
   - Confounder: demografi, transaksi historis, kategori produk.

2. **Estimasi Efek (Backdoor Adjustment)**
   - OLS Regression Adjustment.
   - Propensity Score Matching (PSM).
   - Inverse Probability Weighting (IPW).
   - Doubly Robust (DR Learner).

3. **Heterogeneous & Individual Effects**
   - Causal Forest (CATE/ITE).
   - Segmentasi pelanggan berdasarkan efek kausal.

4. **Business Insights**
   - Segmen paling terpengaruh kampanye.
   - Waktu kampanye optimal.
   - Estimasi ROI.

5. **Deployment**
   - Streamlit/HuggingFace App:
     - Input: atribut user (usia, income, spending historis, kategori produk).
     - Output: prediksi apakah campaign **on target** beserta uplift yang diperkirakan.

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