# Predictive E-Commerce Cart Abandonment & Conversion Analytics

## 📌 Project Overview
This project provides an end-to-end analytical solution for predicting e-commerce cart abandonment. By analyzing customer browsing behavior, operating systems, and page values, this project leverages machine learning to identify the key drivers of successful checkouts. 

The workflow follows the **CRISP-DM** methodology, utilizing **IBM SPSS Modeler** for robust data preparation and predictive modeling, and **Microsoft Power BI** for translating complex machine learning outputs into an interactive, executive-level dashboard.

## 🛠️ Tools & Technologies
* **IBM SPSS Modeler:** Data engineering, feature creation, and machine learning (Classification and Regression Trees, Logistic Regression, Neural Networks).
* **Microsoft Power BI:** Executive storytelling, data visualization, and interactive business intelligence.

## 📊 Key Insights & Business Value
1. **The 'Page Value' Indicator:** Machine learning evaluation (C&R Tree splits and ROC Curves) revealed that `PageValues` is the single most important predictor of whether a user will complete a purchase.
2. **OS Conversion Discrepancy:** The dashboard highlights that Mac/iOS users drive the highest volume (nearly 61%) of successful purchases.
3. **Behavioral & Seasonal Trends:** Custom visuals tracking Weekend Shopper Behavior and Seasonality Trends provide actionable insights for marketing teams to optimize ad spend timing.

## ⚙️ Methodology (CRISP-DM)
### 1. Data Preparation & Engineering (SPSS)
* Created a custom `Total_Browsing_Duration` field to aggregate administrative, informational, and product-related durations.
* Grouped `OperatingSystems` into meaningful categorical buckets (Mac/iOS, Windows, Android, Other) to streamline pattern recognition.
* Partitioned the dataset into **70% Training** and **30% Testing** sets to prevent model overfitting.

### 2. Predictive Modeling (SPSS)
Three primary models were trained to predict the `Revenue` (checkout success) target variable:
* **Classification and Regression (C&R) Tree:** Used to generate transparent decision rules and identify absolute feature importance.
* **Logistic Regression:** Established a statistical baseline for binary classification.
* **Neural Network:** Captured complex, non-linear relationships within the customer behavioral data.

### 3. Executive Dashboarding (Power BI)
Built a unified, interactive dashboard for stakeholders featuring:
* Actual Checkouts vs. Predicted model performance.
* Horizontal impact charts proving the correlation between Page Value and checkout success.
* Interactive `Customer Segment` slicers to filter metrics instantly by New vs. Returning visitors.

## 📁 Repository Structure
* `cart_abandonment_predictive_model.str` - The complete IBM SPSS Modeler stream file containing the data prep and modeling nodes.
* `Ecommerce_Scored_Output.csv` - The final processed dataset containing the machine learning predictions and scoring.
* `cart_abandonment_dashboard.pbix` - The interactive Power BI executive dashboard file.
* `cart_abandonment_dashboard.pdf` - A static PDF export of the Power BI dashboard for immediate browser viewing.
* `Ecommerce_Cart_Abandonment_Project_Explanation.pdf` - The comprehensive final report containing the data audit, SPSS model evaluations, decision tree splits, and visual methodology.

