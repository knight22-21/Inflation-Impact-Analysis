# **Exchange Rate & Inflation Analysis: A PPP-Based Study**

## **📌 Project Overview**
This project analyzes the relationship between **Inflation Rates (India & U.S.)** and the **INR/USD Exchange Rate** over time. The analysis includes:
- Trends in **exchange rates** and **inflation rates**.
- Correlation analysis between inflation and exchange rates.
- A **Purchasing Power Parity (PPP)-based exchange rate prediction** and comparison with actual rates.

## **📂 Dataset Information**
The project utilizes two datasets:
1. **Inflation Rates Data** (`Inflation_Rates_Transformed.csv`): Contains yearly inflation rates for multiple countries, including India and the U.S.
2. **Exchange Rate Data** (`USD_INR_Exchange_Rates_1980_2024.csv`): Contains the historical INR/USD exchange rates from 1980 to 2024.

### **🛠 Data Preprocessing**
- Filtered **Inflation Data** for India and the U.S.
- **Pivoted** inflation data to have separate columns for each country.
- **Merged** exchange rate data with inflation data for a consolidated dataset.

## **📊 Analysis Conducted**
### **1️⃣ Trend Analysis**
- Visualized trends in **INR/USD Exchange Rate, Inflation in India, and Inflation in the U.S.**
- Observed that INR has **depreciated over time** but not always in direct correlation with inflation.

### **2️⃣ Correlation Analysis**
- Exchange Rate vs. Inflation (India) → **Weak Negative Correlation (~ -0.34)**
- Exchange Rate vs. Inflation (U.S.) → **Weak Positive Correlation (~ 0.24)**
- Inflation (India) vs. Inflation (U.S.) → **Very Weak Negative Correlation (~ -0.12)**

### **3️⃣ Purchasing Power Parity (PPP) Analysis**
- **Formula Used:**
  \[ \text{Expected Exchange Rate} = \text{Initial Exchange Rate} \times \prod \left( \frac{1 + \text{Inflation Rate (India)}}{1 + \text{Inflation Rate (U.S.)}} \right) \]
- Compared **actual exchange rate** with the **PPP-predicted exchange rate**.
- Found that **PPP-based rate increased more rapidly than the actual rate**, suggesting additional economic factors influencing the exchange rate.

## **📈 Key Findings**
- Inflation impacts the exchange rate but **is not the sole determinant**.
- The **actual INR depreciation was less than PPP-based predictions**, suggesting intervention by economic policies.
- **Other macroeconomic factors** such as monetary policy, foreign investment, trade balance, and forex reserves influence exchange rate trends.

## **🔧 Tech Stack Used**
- **Python** (pandas, plotly, numpy)
- **Data Visualization**: Plotly
- **Correlation Analysis**: pandas `.corr()`
