# Network Intrusion Detection System (Machine Learning-Based)

A machine learning-based Intrusion Detection System (IDS) designed to classify network attacks into four categories: Denial of Service (DoS), Probe, Remote to Local (R2L), and User to Root (U2R). This project uses the NSL-KDD dataset—an enhanced version of the original KDD Cup 1999 dataset—to train and evaluate predictive models capable of detecting anomalous network traffic patterns.

---

## Overview

The IDS leverages machine learning techniques for automated attack classification and aims to enhance cybersecurity through efficient data preprocessing and robust model evaluation.

Key results:
- Processed over 125,000 network records  
- Reduced model training time by 28% through optimized preprocessing  
- Achieved 91.2% accuracy, 92.5% recall, and an F1-score of 0.91 using the Random Forest model

Key features:
- Classification of network attacks across 4 categories (DoS, Probe, R2L, U2R)  
- Preprocessing using normalization, one-hot encoding, and feature selection  
- Multiple models evaluated for optimal performance  
- Interactive Flask web application for intrusion detection tasks  

---

## Dataset

The project utilizes the **NSL-KDD dataset**, a refined version of the KDD’99 dataset that addresses redundancy and imbalance issues.  
The dataset includes 41 features describing each network connection, categorized into normal traffic and several standardized attack families.

---

## System Workflow

1. Data preprocessing:
   - Removal of duplicates and irrelevant features  
   - Normalization using MinMaxScaler  
   - One-hot encoding of categorical attributes  
   - Feature selection using correlation analysis and mutual information  

2. Model building:
   - Training and comparison of multiple models including Random Forest, SVM, and Logistic Regression  
   - Tuning hyperparameters for maximum precision and recall  

3. Evaluation metrics:
   - Accuracy: 91.2%  
   - Recall: 92.5%  
   - F1-Score: 0.91  

---

## Getting Started

### Prerequisites

Ensure you have installed:
- Python 3.x  
- Libraries: pandas, numpy, scikit-learn, flask, pickle

---

## Installation

1. **Clone the repository**
git clone https://github.com/<username>/network-intrusion-detection.git
cd network-intrusion-detection

2. **Install dependencies**
pip install -r requirements.txt

3. **Run the Flask application**
python app.py

4. **Access the app**
Open your browser and visit:
http://127.0.0.1:5000/

---

## Built With

- [Python](https://www.python.org/) – Programming language  
- [Flask](https://flask.palletsprojects.com/en/latest/) – Web framework for frontend integration  
- [Scikit-learn](https://scikit-learn.org/stable/) – ML algorithms and evaluation tools  

---

## Future Enhancements

- Integration with real-time network traffic monitoring tools  
- Implementation of deep learning models like CNNs or LSTMs for anomaly detection  
- Visualization dashboard for advanced analytics and attack trends  
- Support for live data streaming (Apache Kafka integration)  

---

## Author

Developed by Dev Maheshwari
Computer Science Engineering student focused on applications of machine learning in cybersecurity.

---

## License

This project is licensed under the MIT License.  
You are free to use, modify, and distribute it for educational or research applications.
