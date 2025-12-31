# 🛡️ NOIR – Fraud & Risk Intelligence

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Library](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Status](https://img.shields.io/badge/Status-MVP%20Completed-success)

## 💼 Business Problem
Financial fraud and money laundering cost the global economy billions annually. Traditional rule-based systems (e.g., "if transaction > $10k") generate too many false positives and fail to detect sophisticated patterns.

**The Goal:** Build an AI capable of detecting fraudulent patterns in a dataset of **6.3 million transactions**, focusing on the "Modus Operandi" rather than user identity.

## 🚀 Key Results (Performance)
The **NOIR** system (Random Forest Classifier) achieved:
* **Accuracy:** 99.8%
* **Processed Volume:** 2.7 Million filtered transactions (High Risk)
* **Estimated Fraud Prevention:** R$ 11.8 Billion (Simulated)

## 🛠️ Tech Stack & Strategy
* **Data Processing:** Pandas (ETL, Cleaning, Feature Engineering)
* **Model:** Scikit-Learn (Random Forest)
* **Feature Engineering:**
    * *Temporal Analysis:* Converted linear time steps into "Time of Day" to capture circadian fraud cycles.
    * *Dimensionality Reduction:* Removed high-cardinality ID features to prevent overfitting.
    * *Binary Encoding:* Mapped transaction types for mathematical efficiency.

## 📊 Project Structure
```bash
├── 📁 data/             # Dataset (Ignored in git)
├── 📁 notebooks/        # Jupyter Notebooks (Data Analysis & Model Training)
├── 📁 src/              # Source code for the production pipeline
└── README.md            # Project Documentation
👨‍💻 Author
Matheus Cassiano

[LinkedIn](linkedin.com/in/matheus-cassiano-/)

[Kaggle](kaggle.com/matheus7cassiano)

Built with logic, data, and aggression. 🐍
