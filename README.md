# 🚗 Insurance Claims Fraud Detection using Machine Learning & BI

## 📌 Project Overview
Insurance fraud is a growing global problem, costing over **$80 billion annually** and nearly **₹900 crore per year in India**. This project leverages **Machine Learning (ML)** and **Business Intelligence (BI)** to detect fraudulent vehicle insurance claims, empowering insurers to:

- **Stop losses** from fraudulent payouts  
- **Accelerate** genuine claim settlements  
- **Support investigators** with AI-driven insights  
- **Build trust** with transparent processes  

---

## 🎯 Objectives
- Build an **end-to-end ML pipeline** for fraud detection  
- Develop **interactive BI dashboards** for fraud monitoring  
- Provide a **real-time scoring API** for new claim assessments  

---

## 📊 Dataset
- **Source:** `fraud_oracle.csv` (15,420 records, 33 features)  
- **Features:** Policyholder info, vehicle details, claim history, fraud indicators  
- **Target Variable:** `FraudFound_P` (1 = Fraudulent, 0 = Genuine)  
- **Fraud Rate:** ~6% (highly imbalanced dataset, typical of real-world fraud detection)  

---

## 🔍 Exploratory Data Analysis (EDA)
- Fraud ratio imbalance visualization  
- Demographic trends (age, marital status, sex)  
- Vehicle-related fraud patterns (price, category, age)  
- Claim behavior (timing, address changes)  
- Policy & claim history (deductibles, past claims, supplements)  
- Investigation features (police reports, witnesses)  
- Correlation heatmaps  

---

## ⚙️ ML Modeling
Implemented multiple models to balance **accuracy, recall, and business impact**:

- **Baseline Models:**  
  - Logistic Regression  
  - Random Forest  
  - K-Nearest Neighbors (KNN)  

- **Advanced Model with Imbalance Handling:**  
  - **XGBoost + SMOTE**  
  - Threshold optimization for F1-score  
  - `scale_pos_weight` tuned for fraud vs. genuine ratio  

### 📈 Model Performance
| Model                         | Accuracy | Precision (Fraud=1) | Recall (Fraud=1) | F1-Score | ROC AUC |
|-------------------------------|----------|----------------------|------------------|----------|---------|
| Logistic Regression           | 0.94     | 0.67                 | 0.01             | 0.02     | 0.75    |
| Random Forest                 | 0.94     | 1.00                 | 0.01             | 0.01     | 0.78    |
| KNN                           | 0.93     | 0.25                 | 0.03             | 0.05     | 0.70    |
| **Logistic Regression + SMOTE** | 0.96   | 0.62                 | 0.76             | 0.68     | **0.966** |

---

## 💰 Business Impact
Fraud detection success is measured in **money saved**:

- **Without ML:** ~50% frauds caught → ₹3.75 Cr loss annually  
- **With ML (80% recall):** ~80% frauds caught → only ₹1.5 Cr loss  
- **Net Savings:** ~₹2.25 Cr/year  

False positives cost ~₹10k (extra investigation), but far outweigh the savings from reduced fraudulent payouts.  

---

## 📊 BI Dashboards
Using **Power BI** (or similar tools), dashboards highlight:
- Fraud hotspots & risk zones  
- High-risk claim clusters  
- Garage red flags  
- Investigator performance  
- Claim velocity trends  

---

## 🛠️ Tech Stack
- **Languages & Tools:** Python, Pandas, NumPy, Scikit-learn, XGBoost  
- **ML Techniques:** Logistic Regression, Random Forest, KNN, SMOTE, Threshold Optimization  
- **Visualization:** Matplotlib, Seaborn, Power BI  
- **Deployment:** Flask/FastAPI for real-time scoring (planned extension)  

---

## 🚀 Deliverables
✔️ Production-ready ML fraud detection pipeline  
✔️ BI dashboards for stakeholders  
✔️ Real-time scoring API (integration-ready)  

---

## 📌 Future Work
- Integration with **telematics data** & **image-based fraud detection (CV models)**  
- Deployment as a **microservice** in insurance claim systems  
- Expansion into **geospatial fraud mapping** for regional analysis  

---

## 👤 Author
**[Your Name]**  
- Domain experience in vehicle claims investigations  
- Data Science practitioner | ML | BI | AI for Insurance  

---
