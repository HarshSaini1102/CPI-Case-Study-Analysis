# 📈 Consumer Price Index (CPI) Inflation Analysis & Dashboard (2017–2023)

An executive-ready macroeconomic case study analyzing **India's CPI Inflation dataset (2017–2023)**. This project evaluates headline inflation trends, isolates category-level price shocks during the Covid-19 pandemic, and features an automated, self-auditing QA validation block built directly into Excel.

---

## 📌 Project Overview
* **Timeframe Analyzed:** 2017 – 2023 
* **Primary Tool:** Microsoft Excel (Advanced `LET`, `XLOOKUP`, `SUMIF`, Dynamic Formatting)
* **Core Focus:** Evaluating category basket contributions (Food, Fuel, Health, Personal Care) and mapping pre- and post-pandemic structural price shifts.

---

## 📊 Key Insights
1. **Food Basket Dominance:** Food & Beverages account for **~50% of the CPI basket weight**, making agricultural price volatility the primary driver of headline inflation.
2. **Extreme Basket Divergence:** 
   - **Spices** experienced an extreme upward surge (**+32.67 shift**), driven by severe weather and crop yield disruptions.
   - **Oils and Fats** recorded a sharp decline (**-31.37 shift**), serving as a deflationary buffer due to global price rationalization.
3. **Covid Shock Trajectories:**
   - **Fuel & Light:** Exhibited a V-shaped curve, surging from **2.35% (Mar '19)** to **6.59% (Mar '20)**, dropping to **4.43% (Mar '21)** during lockdowns, and rebounding to **7.52% (Mar '22)** during post-lockdown global crude rallies.
   - **Health:** Experienced a persistent ratchet effect, climbing from **4.17% (Mar '20)** to **6.99% (Mar '22)** due to rising administrative overheads and API import costs.

---

## 🛡️ Model Validation & Quality Assurance Layer
To guarantee reporting integrity and avoid silent formula errors, the dashboard integrates a dedicated **Model Validation & Sanity Checks** matrix :
* **Category Basket Balance:** Validates $100\%$ weight allocation using `LET` and `ROUND`.
* **Data Continuity:** Ensures all 7 years ($2017\text{--}2023$) and 120 monthly periods are fully accounted for.
* **Range Verification:** Automatically flags out-of-bound values, mismatched records ,to count rows and catch errors.

---

## 📁 Repository Structure
```text
├── Cpi_Case_Study_analysis.xlsx       # Interactive Excel Dashboard & Automated QA Layer
├── Dashboard.png/                # Dashboard previews & visual component exports
└── README.md                   # Case study summary and project documentation
