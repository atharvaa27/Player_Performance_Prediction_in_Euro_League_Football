# **Player Performance Prediction in Euro League Football**

## **Introduction**
This project develops a **predictive model** to forecast **player performance** in **European football leagues**. The model predicts **form scores** for upcoming seasons by analyzing **historical data** and incorporating **contextual factors** such as **match location and weather conditions**.

---

## **Key Stakeholders**
### **Who Benefits from This Model?**
- **🏆 Team Managers & Coaches** – Helps in making **proactive decisions** about **lineups and training focus**.
- **📊 Sports Analysts** – Enhances **long-term analyses and prediction accuracy**.
- **⚽ Fans & Enthusiasts** – Provides **data-driven insights** to boost engagement.

---

## **Data**
### **Dataset Source:**  
**Statbunker Football Statistics**

### **Coverage:**  
- **Seasons:** 2014/15 to 2022/23  
- **Leagues Covered:**  
  - Premier League  
  - Bundesliga  
  - La Liga  
  - French Ligue 1  
  - Eredivisie  
  - Serie A  
  - Scottish Premiership  

### **Key Features:**
- **📊 Player Performance Metrics**
- **📍 Contextual Data (match location, weather)**
- **🏟️ Team Metrics**
- **📄 100,000+ rows and 117 features**

---

## **Methods**
### **1. Data Preparation**
- Merged **63 CSV files** covering multiple seasons.
- Standardized key columns for consistency.
- Implemented **systematic data cleaning** to remove inconsistencies.

### **2. Feature Engineering**
- **Weather Summary Integration**
- **Position-Specific Form Score Development**
- **Rolling Feature Creation**
  - **Rolling Mean (3-match window)**
  - **Rolling Variance**

### **3. Modeling Approaches**
#### **Machine Learning Models:**
- **Random Forest Regressor**
- **Linear Regression**
- **XGBoost Regressor**

#### **Time Series Models:**
- **SARIMA**
- **Facebook Prophet**

---

## **Results**
### **Model Performance**
#### **Random Forest Regressor**
- **Cross-validation R²:** 0.9239 ± 0.0176  
- **Test R²:** 0.8983  
- **Best-performing model for generalization**  

#### **XGBoost Regressor**
- **Cross-validation R²:** 0.9945 ± 0.0065  
- **Test R²:** 0.9834  
- **Excellent accuracy but potential overfitting**  

#### **Linear Regression**
- **R²:** 0.9999  
- **MSE:** 2.8926e-13  
- **Indicates potential overfitting**  

---

### **Weather Impact Analysis**
- **🌦️ Weather conditions had minimal impact on form scores**, with variations only in the **fourth or fifth decimal place**.

---

## **Limitations**
**Minimal Weather Impact** – Initial hypotheses suggested greater influence of weather, but results showed negligible effects.  
**Career Changes Not Considered** – **Time series models** do not account for **injuries, transfers, or major career shifts**.  
**Transfer Impact** – Limited ability to **predict the effect of a player transferring between leagues**.  

---

## **Future Work**
**Integration of Additional Contextual Features:**
- **🚑 Player injuries**
- **📊 Team formations**
- **🤝 Player-club synergy**
- **⚽ Inter-player interactions**

**Development of an Interactive Dashboard**
- **📊 Visualization tools** for stakeholders to **analyze player performance predictions effectively**.

---

## **Contributors**
👤 Aaryan Wani
🔗 LinkedIn

