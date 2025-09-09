
# 🧠 Demand Forecasting for Retail Chains 🛒  
*Accurately predicting future sales using advanced machine learning models*

![Retail Forecasting Banner](https://ibb.co/Z18Rx3h1)  
<sub>Image by Freepik</sub>

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/status-completed-brightgreen.svg)]()

---

## 📌 Project Overview

Demand forecasting is a critical task for retail chains managing large product portfolios across multiple store locations. This project tackles that challenge using **three years of historical sales data** from one of the world’s largest retail chains — covering:

- 76 stores  
- Weekly sales of hundreds of SKUs  
- Pricing & promotion information

The objective is to build an efficient, accurate model to forecast **weekly sales for each product-store combination for the next 12 weeks**.

---

## 🎯 Objectives

- Predict future weekly **sales units** for each SKU-store pair
- Identify the **impact of promotions and pricing** on demand
- Use **machine learning** to optimize stock planning and reduce overstock/understock issues
- Segment products/stores using **clustering** for deeper insights

---

## 🗂 Dataset Overview

- **Duration**: 3 years of weekly data  
- **Records**: Millions of entries  
- **Key Features**:
  - `store_id`, `sku_id`, `week`
  - `total_price`, `base_price`
  - `is_featured_sku`, `is_display_sku`
  - `units_sold` (target)

---

## 🧪 Methodology

### 🧼 1. Data Preprocessing
- Date formatting & datetime feature extraction
- Price difference & relative price engineering
- Cleaned missing and inconsistent values

### 📊 2. Exploratory Data Analysis (EDA)
- Seasonal sales trends
- Promotion & price impact
- SKU/store-level distribution and performance

### ⚙️ 3. Model Building & Evaluation
- **Random Forest**, **LightGBM**, **SVM**, **Decision Tree**, **KNN**
- Evaluation metrics: **MSE**, **MSLE**
- **Hyperparameter tuning** using grid search

### 🔮 4. Forecasting
- Predicted **12 weeks forward** using best model (LightGBM)

---

## 📊 Visual Insights

- Seasonal peaks around **June–July**
- Notable **decline** post-2011
- Promotions strongly boost sales
- SKU clustering reveals high vs low performers

---

## 🤖 Clustering & Segmentation

- Applied **KMeans** clustering
- Optimal `k = 3` via Elbow method
- PCA for dimensionality reduction & visualization

---

## 🏁 Results Summary

| Model               | MSE (Before) | MSE (After) | Verdict |
|--------------------|--------------|-------------|---------|
| Random Forest       | High         | Medium      | ❌      |
| Decision Tree       | High         | Medium      | ❌      |
| Support Vector      | High         | High        | ❌      |
| K-Nearest Neighbors | High         | Medium      | ❌      |
| **LightGBM**        | ✅ **Lowest** | ✅ **Lowest** | ✅ ✅ ✅  |

---

## 📚 Tech Stack

- **Python 3.9+**
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**, **Plotly**
- **Scikit-learn**, **LightGBM**
- **KMeans**, **PCA** for clustering

---

## 📁 Repository Structure

```
📦 demand-forecasting-retail
├── 📁 data                 # Raw and processed data
├── 📁 notebooks            # Jupyter notebooks for EDA and model training
├── 📁 models               # Trained model files (optional)
├── 📁 results              # Plots, forecasts, and reports
├── 📄 Demand_Forecasting_Report.pdf
└── 📄 README.md            # You're here!
```

---

## 📈 Future Improvements

- Add interactive **Streamlit dashboard**
- Explore deep learning (e.g. **LSTM**, **Prophet**)
- Automate pipeline & deploy API for live forecasting

---

## 👨‍💻 Author

**Ahsanullah MRM**  
ML Engineer | AI Enthusiast | Data-Driven Innovator  
📍 Dubai | 🌐 Open to Collaborations  
📧 [Connect on LinkedIn](https://linkedin.com/in/ahsanullahmrm)

---

> “Data beats emotions.” – Sean Rad

