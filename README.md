# Predictive-Analytics-Using-Machine-Learning-Regression-Models
# The Visual Shopper  
**Predicting Computer Prices Using User-Facing Features**

## Project Overview
The Visual Shopper is a machine learning project that predicts computer (laptop) prices using *user-facing and visual features* rather than deep technical specifications. The project validates the **Visual Shopper Hypothesis** — that market prices are largely driven by features consumers actually notice, such as brand, RAM, display quality, and form factor.

Using a large real-world dataset and advanced machine learning models, the project achieves high prediction accuracy while maintaining interpretability and business relevance.

---

## Objectives
- Predict retail computer prices with high accuracy (Target MAE < $200)
- Identify key pricing drivers in the consumer computer market
- Compare multiple machine learning models
- Deliver business insights for consumers, retailers, and manufacturers

---

## Dataset
- **Source:** Kaggle – All Computer Prices Dataset  
- **Initial Size:** ~100,000 records  
- **Final Size:** ~89,000 records (after cleaning)  
- **Features:** Brand, RAM, GPU, OS, display resolution, screen size, weight, form factor, and more  
- **Target Variable:** Price (USD)

### Data Cleaning
- Removed outliers using percentile capping  
- Eliminated impossible or fraudulent configurations  
- Filtered anomalous low-priced high-end hardware listings  

---

## Feature Engineering
- **GPU Tiers:** Ordinal encoding of GPU performance levels  
- **Screen PPI:** Engineered from resolution and display size  
- **Brand Reputation Score:** Proxy for ecosystem and brand premium  

---

## Models Implemented
- **Ridge Regression** (Baseline)
- **Random Forest**
- **XGBoost (Optimized – Final Model)**

### Model Validation
- 80/20 Train-Test Split  
- 5-Fold Cross-Validation  
- Hyperparameter tuning using GridSearchCV and RandomizedSearchCV  

---

## Performance
- **Best Model:** XGBoost  
- **Mean Absolute Error (MAE):** ~$173  
- **R² Score:** ~0.76  
- **Improvement over Baseline:** ~19%

### Key Pricing Drivers
1. RAM (~40%)  
2. Brand (Apple premium effect)  
3. Operating System (macOS)  
4. Screen Quality (PPI)  
5. Brand Reputation  

---

## Business Value
- **Consumers:** Price verification and negotiation confidence  
- **Retailers:** Mispricing detection and inventory optimization  
- **Manufacturers:** Feature value quantification for product strategy  

---


---

## How to Run
1. Clone the repository  
2. Open `ml_project_17.ipynb` in Jupyter Notebook  
3. Run cells sequentially to reproduce results  

---

## Results Summary
The project successfully demonstrates that high-level, consumer-visible features can explain nearly 75–80% of price variance in the computer market. The XGBoost model provides reliable predictions, especially in the mid-range price segment ($800–$2,000).

---

## Future Enhancements
- NLP on product titles and descriptions  
- Time-based pricing trends and depreciation  
- Neural network models for premium segment accuracy  
- Model deployment as a web application  

---
