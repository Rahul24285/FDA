# 🛡️ Fraud Detection System for Financial Transactions

## 📚 Project Overview
This project implements a **Machine Learning-based fraud detection system** using a financial transactions dataset. Inspired by real-world applications like **Robinhood**, it employs various algorithms to identify fraudulent transactions and evaluates their performance. The system demonstrates the power of data science in enhancing security, compliance, and financial integrity.

---

## 🚀 Key Features
- **Multiple Models Evaluated**:
  - Random Forest
  - Logistic Regression
  - Neural Network (MLPClassifier)
  - Isolation Forest (unsupervised anomaly detection)
  - Decision Tree
- **Data Preprocessing**:
  - Dropping uninformative columns (`zipcodeOri`, `zipMerchant`)
  - Label encoding of categorical features
  - Scaling features with StandardScaler
  - Handling missing data
- **Imbalance Handling**:
  - SMOTE (Synthetic Minority Oversampling Technique) applied to balance the training set and improve model learning for rare fraud cases.
- **Model Evaluation**:
  - Metrics: Precision, Recall, F1-score, AUC (Area Under the ROC Curve)
  - Comprehensive classification reports
  - Analysis of confusion matrices

---

## 🔍 Problem Statement
Financial institutions like **Robinhood** face significant risks from fraudulent transactions. The goal is to build a machine learning model that accurately identifies fraud while minimizing false positives, thereby:
- Preventing financial losses
- Protecting customer accounts
- Enhancing compliance with KYC/AML regulations
- Maintaining platform reputation and customer trust

---

## 💡 Practical Benefits for Robinhood
- **Real-Time Fraud Detection**: Rapidly flag suspicious trades and accounts for investigation.
- **Behavioral Analysis**: Learn patterns of fraud versus normal behavior, even as tactics evolve.
- **Regulatory Compliance**: Automate suspicious activity reporting and auditing.
- **Financial Protection**: Reduce losses, legal costs, and chargebacks from fraudulent activities.
- **Strategic Advantage**: Secure operations enable growth into new markets like crypto and margin lending.

---

## 📊 Dataset
The dataset (`bs140513_032310.csv`) simulates real transaction data with attributes like customer ID, merchant ID, age, gender, category, and fraud label. It’s structured to mimic real-world scenarios with class imbalance (~1.2% fraud).

---

## 🏗️ Project Pipeline
1. **Load and Clean Data**
2. **Feature Engineering**: Label encoding, scaling, SMOTE application
3. **Model Training**: Train multiple models with the same preprocessing pipeline
4. **Evaluation**: Analyze metrics and confusion matrices to compare models
5. **Result Interpretation**: Explain why some models performed better than others

---

## 📈 Key Takeaways
- **Neural Networks** achieved the highest AUC and recall, best for catching fraud but less interpretable.
- **Random Forest** balanced performance and interpretability, offering a strong candidate for deployment.
- **Isolation Forest** underperformed due to its unsupervised nature and inability to learn from labeled data.
- **Logistic Regression** and **Decision Tree** provided useful baselines but lacked the sophistication needed for high-stakes fraud detection.

---

## 🔐 Conclusion
This project highlights the critical role of machine learning in securing financial systems and protecting users from fraud. It demonstrates how businesses like **Robinhood** can integrate intelligent fraud detection into their platforms to stay ahead of evolving threats and maintain user trust.
