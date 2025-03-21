# CASIA_ProgrammingAsssignment5

Here's a README file you can include once you finish the project:

---

# Cybersecurity Attack Classification Using Random Forest

## 📚 **Project Overview**
This project is part of Programming Assignment 5 for the Technological University of the Philippines – Manila, College of Engineering, Electronics Engineering Department. The objective is to develop a machine learning model to classify various types of cyberattacks using a Random Forest classifier. 

The model is trained on a simulated network traffic dataset and aims to detect attacks such as **DDoS**, **Botnet**, **PortScan**, and **Phishing**. 

---

## 🚀 **Dataset**
The dataset used is `cyber_attacks.csv`, which contains the following features:

- `protocol_type`: Protocol (0: TCP, 1: UDP, 2: ICMP)  
- `duration`: Connection duration (seconds)  
- `src_bytes`: Bytes sent from the source  
- `dst_bytes`: Bytes sent to the destination  
- `num_packets`: Number of packets transmitted  
- `num_connections`: Number of connections  
- `attack_type`: Attack label (Normal, Botnet, DDoS, PortScan, Phishing)  

---

## ⚙️ **Preprocessing Steps**
1. **Loading and Exploring the Data**
    - Loaded the dataset and conducted Exploratory Data Analysis (EDA).  
    - Visualized distributions of key features.  

2. **Data Preprocessing**
    - Handled missing values by:  
        - Imputing with median/mean for numerical features.  
        - Using mode or 'Unknown' for categorical values.  
    - Encoded the `protocol_type` using **One-Hot Encoding**.  
    - Scaled numerical features using **StandardScaler**.  
    - Addressed class imbalance with **SMOTE (Synthetic Minority Over-sampling Technique)**.  

---

## 🌲 **Model Development**
- Trained a **Random Forest Classifier** using the preprocessed dataset.  
- Tuned the following hyperparameters:  
    - `n_estimators`: Number of trees.  
    - `max_depth`: Maximum tree depth.  
    - `min_samples_split`: Minimum samples to split a node.  
    - `min_samples_leaf`: Minimum samples for a leaf node.  
- Used **Pipeline** for efficient preprocessing and model fitting.  

---

## 📊 **Evaluation**
- Evaluated the model using:  
    - **Precision**, **Recall**, and **F1-score** to handle class imbalance effectively.  
    - Confusion matrix and classification report for detailed performance analysis.  
- Identified the hardest-to-classify attack types and discussed potential reasons.  

---

## 🔥 **Feature Importance**
- Analyzed feature importance using the Random Forest model.  
- Visualized the most significant features for attack classification.  

---

## 🌐 **Deployment and Real-World Application**
- Suggested steps for deploying the model in a real-time network monitoring system.  
- Discussed strategies to handle unseen attack types using **incremental learning** or **continuous retraining**.  

---

## 📂 **Files and Structure**
- `cyber_attacks.csv`: Dataset used for training.  
- `assignment_5_rf.ipynb`: Jupyter Notebook with the full code and analysis.  
- `README.md`: This documentation file.  
- `requirements.txt`: Python libraries used.  

---

## 🛠️ **Technologies Used**
- Python  
- Pandas, NumPy (data manipulation)  
- Matplotlib, Seaborn (visualization)  
- Scikit-Learn (model development and evaluation)  
- SMOTE (handling class imbalance)  

---

## 🚦 **How to Run**
1. Clone the repository:
   ```bash
   git clone <repository_link>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook assignment_5_rf.ipynb
   ```

---

## 🤝 **Contributors**
- CASIA, Axle Jade D; FERNANDEZ, Joseph Bryan Lloyd
- Technological University of the Philippines – Manila  
- Electronics Engineering Department  

---
