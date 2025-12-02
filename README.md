# Machine-Learning
This project applies machine-learning techniques to analyze and forecast the evolution of renewable-energy usage worldwide. Using a Kaggle dataset containing historical renewable-energy shares for each country, combined with World Bank income-group information.


# README – Renewable Energy Forecasting with Machine Learning

## Project Overview

This project analyzes the global evolution of renewable-energy usage and builds machine-learning models to forecast future trends. Using historical energy data combined with World Bank income-group classifications, the project compares renewable adoption across countries of different economic levels and evaluates several regression models to project the renewable-energy share up to 2050.

The work follows a full data-science pipeline:  
**data acquisition → cleaning → exploration → modeling → evaluation → forecasting → interpretation**

---

## Datasets Used

### **1. Renewable Energy Share Dataset**
Contains the share of renewable energy in primary energy consumption for each country and year.  
Used to analyze historical trends and build forecasting models.

### **2. World Bank Income Groups Dataset**
Provides the income classification for each country:  
**High income**, **Upper middle income**, **Lower middle income**, **Low income**.  
Used to compare renewable-energy growth across economic categories.

After cleaning and merging, the final dataset contains:  
- **Entity** (country)  
- **Year**  
- **Renewable-energy share (%)**  
- **IncomeGroup**

---

## Steps of the Project

### **1. Defining the Problem**
We aim to model and forecast the renewable-energy share for the coming decades, while examining disparities across income groups. This allows us to evaluate how global progress aligns with climate objectives.

### **2. Data Cleaning**
- Handling missing values  
- Merging with the income-group dataset  
- Creating a final clean dataframe

### **3. Data Exploration**
We visualize:
- Global historical trends  
- Differences between income groups  
- Yearly averages for each category  

These visualizations help understand how renewable adoption evolves across the world.

### **4. Machine-Learning Models**
The task is formalized as a regression problem. Models tested:
- **Linear Regression**
- **Decision Tree**
- **k-Nearest Neighbors**
- **SVM – RBF kernel**

Models are evaluated using:
- **MAE** (Mean Absolute Error)  
- **RMSE** (Root Mean Squared Error)  
- **R² Score**

We also perform **GridSearchCV** to optimize hyperparameters.

### **5. Forecasting**
The best model, **SVM**, is used to:
- Predict the global renewable-energy share up to 2050  
- Generate separate projections for each income group  

Historical curves and SVM predictions are plotted together for comparison.

---

## Key Results

- **SVM** is the most accurate and stable model for long-term forecasting.  
- High-income countries show **strong acceleration** in renewable adoption.  
- Middle- and lower-income groups show **slower growth**, leading to widening disparities.  
- Global projections remain **below what is required** to meet 1.5°C or 2°C climate targets.  
- Renewable adoption must increase significantly to align with IPCC scenarios.

---

##  Conclusion

This project demonstrates how machine-learning techniques can be applied to understand and forecast global renewable-energy trends. While clear progress is visible in high-income countries, global adoption remains too slow to meet climate objectives. Achieving climate-aligned pathways will require stronger policies, greater investment, and enhanced international cooperation to accelerate renewable-energy deployment worldwide.

