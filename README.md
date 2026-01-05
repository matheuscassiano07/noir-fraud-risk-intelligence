# 🌑 NOIR – Network-Oriented Intelligence for Risk

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python)
![AI](https://img.shields.io/badge/Scikit_Learn-Random_Forest-orange?style=for-the-badge&logo=scikit-learn)
![Graph](https://img.shields.io/badge/NetworkX-Graph_Analytics-red?style=for-the-badge&logo=networkx)
![Status](https://img.shields.io/badge/Status-Production_Ready-success?style=for-the-badge)

> **"Fraud is not an isolated event. It is a network."**

## 💼 The Mission
Standard fraud detection systems look at transactions in isolation (e.g., *"Is this transfer > $10k?"*). Sophisticated criminal rings bypass this easily.

**NOIR** changes the paradigm. Instead of analyzing just the transaction, we analyze the **topology of the network**. We use Graph Theory combined with Forensic Feature Engineering to detect not just the fraud, but the **fraudster's entire ring**.

**The Goal:** Dismantle organized crime networks within a dataset of **6.3 million transactions** by identifying hidden connections (Device Sharing, Mule Accounts, and Circular Flows).

---

## 🔬 Key Innovations (The "Secret Sauce")
Unlike generic models, NOIR employs 5 custom-built forensic signals:

1.  **🕸️ The Domino Effect (Graph Analytics):**
    * Uses **NetworkX** to map "Device Fingerprint" connections.
    * **Capability:** If *one* account is flagged, the system automatically traces and blocks the entire connected subgraph (the criminal ring).
    * *Result:* Single detection leads to multi-account takedowns.

2.  **💸 Physics of Money (Velocity & Burn Rate):**
    * Calculates `Cash Residence Time` (how long money sits in an account).
    * Detects "Mule Accounts" that receive and cash out funds instantly (< 1 minute).

3.  **🌪️ Entropy Analysis:**
    * Measures the mathematical chaos in beneficiary patterns. Legit users have predictable flows; fraudsters have high entropy.

---

## 📊 Visual Intelligence

### 1. The Network Takedown (Graph Analysis)
*Visualizing the hidden connections between "Mule Accounts" sharing the same device fingerprint.*

<img width="895" height="592" alt="image" src="https://github.com/user-attachments/assets/b59e0ea1-a3fd-49bd-b6e3-442c3257c13c" />


### 2. Feature Importance
*Proving that behavioral signals (Burn Rate) outperform static data.*

<img width="872" height="293" alt="image" src="https://github.com/user-attachments/assets/c97c21c0-2a21-461f-b5da-1c5992fc7bfe" />


---

## 🚀 Performance Metrics (Simulated on 500k+ Samples)

| Metric | Result | Impact |
| :--- | :--- | :--- |
| **Detection Logic** | **Random Forest + Graph Hybrid** | Best of both worlds (Pattern + Connection) |
| **Network Takedown** | **Active** | Blocks connected users automatically |
| **Processing Speed** | **< 45ms** | Real-time ready latency |
| **ROI (Estimated)** | **High Impact** | Prevention of mass-scale attacks |

> *Note: Metrics derived from a balanced stratified sample of the PaySim dataset.*

---

## 🛠️ Tech Stack & Architecture

* **Core Engine:** Python 3.10
* **Data Engineering:** Pandas & NumPy (Vectorized operations for 1M+ rows)
* **Machine Learning:** Scikit-Learn (Random Forest with Balanced Subsampling)
* **Graph Intelligence:** NetworkX (Connected Components & Centrality Algorithms)
* **Visualization:** Matplotlib & Seaborn (Forensic Reporting)


**Matheus Cassiano**
*Software Developer | Python & AI Enthusiast*

Looking for: **Internship / Junior Opportunities** in Backend & Security.

[LinkedIn](https://www.linkedin.com/in/matheus-cassiano-/) • [Kaggle](https://www.kaggle.com/matheus7cassiano)

> *"Transforming coffee into secure code and data insights."* ☕🐍
