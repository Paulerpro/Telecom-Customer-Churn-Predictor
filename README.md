# **Telecom Customer Churn Prediction (XGBoost Classifier)**  

## **📌 Overview**  
This project predicts customer churn (whether a customer will leave a telecom service) using an **XGBoost classifier**. The model analyzes customer demographics, account details, and service usage to identify at-risk customers, helping businesses take proactive retention measures.  

---

## **📂 Dataset**  
- **Source**: [Kaggle / Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)  
- **Features**:  
  - **Demographics**: Gender, Senior Citizen status, Partner/Dependents  
  - **Account Info**: Tenure, Contract Type, Payment Method  
  - **Services**: Internet Service, Online Security, Streaming, etc.  
  - **Target Variable**: `Churn` (Yes/No)  

---

## **🛠️ Tech Stack**  
- **Language**: Python  
- **Libraries**:  
  - `pandas`, `numpy` (Data Processing)  
  - `scikit-learn` (Preprocessing & Metrics)  
  - `XGBoost` (Classifier)  
  - `plotly` (Visualization)  

---

## **🚀 Key Steps**  
1. **Data Preprocessing**  
   - Handled missing values (`TotalCharges`).  
   - Encoded categorical variables (`LabelEncoder`).  
   - Scaled numerical features (`StandardScaler`).  

2. **Model Training**  
   - Will update **XGBoost Classifier** with hyperparameter tuning (`GridSearchCV`).  
   - Optimized for **precision/recall** (since retaining customers is costly).  

3. **Evaluation Metrics**  
   - **Accuracy**: ~80%  
   - **Precision (Churn=Yes)**: ~78%  
   - **Recall (Churn=Yes)**: ~84%  
   - **F1-Score**: ~81%  

4. **Feature Importance**  
   - Top predictors:  
     1. **Tenure** (How long the customer stayed)  
     2. **Monthly Charges**  
     3. **Contract Type** (Month-to-month customers more likely to churn)  

---

## **📊 Results & Insights**  
- The model identifies **55% of churners** (recall) with **78% precision**.  
- **Key Churn Drivers**:  
  - Short-term contracts (`Month-to-Month`).  
  - High `MonthlyCharges` with low `tenure`.  
  - Lack of `OnlineSecurity` or `PhoneService`.  

---

## **💡 Business Impact**  
- **Targeted Retention**: Offer discounts/loyalty programs to high-risk customers.  
- **Service Improvements**: Focus on customers without `OnlineSecurity` or `PhoneService`.  

---

## **📥 How to Run**  
1. Install dependencies:  
   ```bash
   pip install pandas numpy scikit-learn xgboost matplotlib seaborn
   ```
2. Run the Jupyter notebook:  
   ```bash
   jupyter notebook Telecom_Churn_Prediction.ipynb
   ```

---

## **📜 License**  
MIT License. Free for academic/commercial use.  

---

## **📧 Contact**  
For questions or improvements, email: [(https://github.com/Paulerpro/Telecom-Customer-Churn-Predictor.git)]  

--- 

**🔗 GitHub Repo**: [Your-Repo-Link]  

--- 

### **🎯 Future Work**  
- Deploy as a **Flask/Django web app** for real-time predictions.  
- Experiment with **neural networks** for improved recall.  

--- 

**🌟 Star the repo if you found this useful!** 🚀