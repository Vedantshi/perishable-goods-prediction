# Smart Perishable Demand Forecasting in Grocery Retail

## Overview

This project addresses a common challenge in grocery retail: accurately forecasting the daily demand for perishable items like milk, fruits, vegetables, and meat. Using store-level sales data, weather conditions (temperature and rainfall), calendar features, and product types, we built a machine learning model to support smarter inventory decisions and reduce waste.

---

## Objectives

- Forecast daily sales at the **SKU-store** level
- Incorporate **weather**, **calendar**, and **store-specific** data
- Reduce **spoilage** and **stockouts** through better replenishment
- Visualize insights using an **interactive Tableau dashboard**
- Provide a **user input-based prediction tool** for real-time estimation

---

## Methodology

### Tools Used
- **Python (Pandas, LightGBM, Seaborn, Matplotlib)**
- **Jupyter Notebook**
- **Tableau**
- **CSV dataset**

### Key Steps
1. **Data Cleaning**  
   - Loaded and inspected raw data  
   - Converted date column to datetime format  
   - Identified and handled missing values and outliers (boxplots for temp/rainfall)  

2. **Feature Engineering**  
   - Extracted day-of-week, month, and weather features  
   - One-hot encoded categorical variables  

3. **Modeling**  
   - Trained a **LightGBM regressor** on cleaned data  
   - Evaluated using **MAE** and **RMSE**  
   - Final model tested for multiple store and product scenarios  

4. **Prediction Interface**  
   - Script allows users to input:  
     - Store ID  
     - Product Type  
     - Temperature (°C)  
     - Rainfall (mm)  
   - Returns predicted units sold  

5. **Visualization**  
   - Tableau dashboard to track demand trends across stores, dates, and weather conditions  

---

## Files Included

| File | Description |
|------|-------------|
| `code.ipynb` | Complete Python notebook: EDA, modeling, prediction script |
| `Data_for_2024.csv` | Cleaned dataset with sales, weather, and calendar data |
| `Tableau.twb` | Tableau workbook for visual storytelling |
| `Smart_Perishable_Demand_Final_Documentation.docx` | Final project documentation |
| `Smart_Perishable_Demand_Forecasting_SOW.docx` | Statement of Work outlining scope and goals |

---

## Results

- **MAE:** 3.76  
- **RMSE:** 4.74  
- Model captured demand trends accurately across various product-store combinations  
- Tableau dashboard revealed clear **seasonality**, **weather effects**, and **store-specific behaviors**

---

## Business Impact

- Reduced spoilage by forecasting only necessary stock
- Prevented lost sales from stockouts during high-demand periods
- Empowered store managers to make localized, data-driven decisions

---

## Future Scope

- Integrate real-time weather APIs for live prediction
- Expand to include **promotions**, **pricing**, and **supplier constraints**
- Deploy as a web app for seamless integration with retail systems

---

## Author

**Vedant Shinde**  
Master’s in Information Systems | Data & Retail Analytics  
[LinkedIn](https://www.linkedin.com/in/vedantshinde25) | [Email](mailto:shindev124@gmail.com)
