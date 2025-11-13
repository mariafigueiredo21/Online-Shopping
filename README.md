# 📊 Online Retail Predictive Analytics Project

Customer Behavior, Forecasting & Profitability Intelligence

Author: Maria Figueiredo

Date: November 2025

---

## 🚀 Project Overview

This repository contains a complete end‑to‑end predictive analytics pipeline built using the Online Retail Dataset (UCI Machine Learning Repository). The project covers the full lifecycle of data science in a real e‑commerce context:
- 🧹 Data Cleaning & Preparation
- 📦 Product-Level Analytics
- 👥 Customer Segmentation (RFM, K-Means)
- 💰 Customer Lifetime Value (CLV) Modeling
- 🔄 Retention & Churn Prediction
- 🔮 Time Series Forecasting (Sales, Churn, CLV, Product Demand)
- 🏗 Strategic Insights for Marketing, Finance & Operations

The goal is to transform transactional retail data into actionable intelligence, supporting decision‑making on retention, logistics, promotions, inventory, and long-term customer profitability.

## 📥 Dataset Instructions
The dataset is available from the UCI Machine Learning Repository.

🔗 Download “Online Retail.xlsx” here:
https://archive.ics.uci.edu/ml/datasets/Online+Retail

After downloading:
- Place the file inside the folder: data/
- Clean it using the steps provided in 0_Data_Cleaning.py
- Save the cleaned CSV as: Online_Retail_CLEAN.csv

⚠️ Note: The dataset is not included in this repository due to licensing restrictions.

The central hypothesis:
**- Firms with higher sales growth and stronger liquidity ratios behave as “quality firms” — stable and efficient, but not systematically mispriced.**

## 🔧 Installation & Setup
#### 1️⃣ Create a virtual environment
- python -m venv venv
- source venv/bin/activate # macOS/Linux
- venv\Scripts\activate # Windows

#### 2️⃣ Install the required packages
- pip install -r requirements.txt

#### 3️⃣ Run any of the analytical steps

## 🧠 Key Analytical Components
#### 1️⃣ Customer Segmentation (RFM)
  - Recency, Frequency and Monetary metrics
  - Identification of VIPs, at‑risk customers, and churn candidates
#### 2️⃣ CLV Modeling
  - Historic CLV per customer
  - Predictive CLV via regression and Prophet forecasting
#### 3️⃣ Churn Prediction
  - Behavioral churn definition based on recency
  - Random Forest Classifier with feature importance
  - Monthly churn forecasting using Prophet
#### 4️⃣ Product Demand Forecasting
  - Top-selling items identified through sales contribution
  - Prophet-based monthly demand forecasts for operational planning
#### 5️⃣ Strategic Analytics
  - Revenue optimization
  - The objective is to evaluate temporal and cross-sectional stability (Fama–MacBeth, downside risk).

## 📈 Main Results Delivered
- A full churn intelligence system (individual + forecasted)
- CLV projections showing +18–25% yearly value growth
- Demand forecasting identifying seasonal inventory peaks
- Segmentation for micro-targeted marketing
- Predictive models ready for business dashboards

This project bridges:
- Customer analytics 🧍
- Financial forecasting 💰
- Operational demand planning 📦

## 🧩 Technologies Used
- Python (pandas, numpy, seaborn, matplotlib)
- Machine Learning: scikit-learn (Random Forest, K-Means)
- Time Series Forecasting: Meta Prophet
- Visualization: seaborn, matplotlib

## 🧠 How to Use This Project
You can:
- Run each step independently
- Use STEP 9 as a complete forecasting pipeline
- Integrate the models into a Power BI dashboard
- Adapt thresholds, segmentation, forecast horizons, etc.

## 🎯 FINAL INTERPRETATIONS & TAKEAWAYS
#### 1. Customer Behavior is Predictable — and Profitable
Across RFM, churn, and CLV modelling, customer patterns display strong predictability:
- Recency is the single most powerful predictor of future engagement.
- Frequent and high-spending customers consistently show higher retention and CLV.
- Customer activity clusters around seasonal periods (especially Q4).

Implication: Retention programs should focus on “slipping customers” (Recency 30–90 days) with personalized offers.

#### 2. Revenue and Demand Follow Clear Seasonal Cycles
Prophet models consistently reveal:
- Revenue peaks in November–December.
- Demand drops in Q1 (January–February).
- Product-level seasonality varies strongly by SKU but aligns with macro retail cycles.

*Implication*: Inventory planning, staffing, and marketing should be synchronized with these predictable cycles.

#### 3. Churn Declines Over Time — but Seasonality Matters
Churn forecasting identified:
- A mild downward trend in churn over months (improving retention).
- Churn spikes immediately after major sales periods.
- Longer periods of inactivity strongly predict dropout.

Implication: Proactive reactivation campaigns should target customers right after seasonal peaks.

#### 4. CLV Shows Strong Growth Potential
CLV projections indicate:
- An expected +18–25% increase in customer value over the next year.
- Seasonal boosts in Q4 driven by higher basket value and purchase frequency.
- Stable long-term growth aligned with revenue trends.

Implication: Marketing budgets should be weighted toward high-CLV segments and peak-value months.

#### 5. Top Products Drive Disproportionate Revenue
Demand forecasting shows:
- A small subset of products consistently produces the highest demand peaks.
- Many SKUs have predictable monthly seasonality.
- Some products display long-term upward trends, valuable for growth strategies.

Implication: Both pricing and stocking strategies should prioritize these high-impact products.

#### 6. Integrated Forecasting Enables End-to-End Optimization
By combining CLV + Churn + Revenue + Demand Forecasting:
- Companies can match customer expectations with inventory readiness.
- CLV peaks can be paired with upselling and loyalty programs.
- Demand peaks can be aligned with stock, supply chain, and promotions.
- Churn cycles inform CRM automation and personalized communication.

Ultimate Result: A holistic, predictive ecosystem that reduces risk, increases profitability, and enhances customer satisfaction.

---

### ✅ Project Summary
This project delivers a complete end-to-end analytical pipeline for e-commerce behavioral and financial intelligence, using the Online Retail dataset (UCI).
Across nine progressive steps, the analysis evolves from raw data exploration to predictive modeling, integrating customer behavior, sales performance, forecasting, churn prediction, and product demand.
The full workflow includes:

#### 1. Data Exploration & Cleaning
- Identified and corrected missing values, negative quantities, and cancelled invoices
- Engineered key variables (e.g., TotalPrice, invoice-level aggregation).
- Created a data dictionary and structural overview.

#### 2. Customer Behavior Insights
- Built RFM (Recency–Frequency–Monetary) features for segmentation and customer profiling.
- Analyzed spending intensity, purchase patterns, and geolocation dynamics.

#### 3. Financial Analysis
- Assessed revenue distribution, high-value products, and customer contribution.
- Investigated seasonal and cyclical patterns.

#### 4. Customer Retention & Churn
- Created churn labels using behavioral thresholds.
- Trained a Random Forest classification model to predict churn risk with high accuracy.
- Identified the strongest churn drivers (Recency > Frequency > Monetary).
- Built a long-term churn forecast using Prophet.

#### 5. Sales Forecasting (Prophet)
- Forecasted total monthly revenue using Meta Prophet.
- Identified predictable seasonal peaks (Q4) and post-holiday declines.

#### 6. CLV Forecasting
- Calculated Customer Lifetime Value per customer.
- Projected future CLV trends, showing consistent financial growth over 12 months.

#### 7. Product Demand Forecasting
- Built demand forecasts for top products.
- Detected SKU-specific seasonality and long-term growth opportunities.

#### 8. Strategic Integration
All components are linked into a unified predictive intelligence framework, enabling full visibility across:
- Customer behavior
- Sales dynamics
- retention cycles
- product demand
- lifetime value
- financial forecasting

---

### 💡 “By transforming raw customer behavior into predictive intelligence, this project demonstrates how analytics can directly drive strategic decision-making. It proves that in modern commerce, foresight is not an advantage — it is a necessity.”

