# AI-Fraud-detection

This project focuses on fraud detection in financial transactions using a synthetically generated dataset. The dataset is highly imbalanced and contains:
194 fraudulent transactions and 2583 non-fraudulent transactions
The goal is to identify anomalous transaction patterns using unsupervised anomaly detection techniques.

Methodology
1. Data Preparation
Synthetic dataset representing transactional behavior
Imbalanced class distribution (fraud is minority class)
Data preprocessing and normalization applied before modeling
2. Models Used
The project compares multiple unsupervised anomaly detection algorithms:
Isolation Forest
Detects anomalies by isolating observations in random partitions
Local Outlier Factor (LOF)
Identifies anomalies based on local density deviation
One-Class SVM
Learns the boundary of normal transactions and detects outliers
3. Evaluation Metrics
Although models are unsupervised, performance is evaluated using labeled data:
Accuracy
Precision
Recall
F1-score
Additionally:
ROC curves are used to evaluate model discrimination ability

Risk Segmentation
Detected anomalies are further analyzed and grouped into risk levels, enabling:
Identification of highly suspicious transactions
Prioritization for investigation
Generation of a suspicious activity report

Output
Model comparison across three anomaly detection techniques
ROC curve visualization
Classification metrics summary
Risk-level segmentation of transactions
Suspicious transaction reporting

Limitations
Synthetic data may not reflect real-world fraud complexity
Class imbalance can bias evaluation metrics (especially accuracy)
Unsupervised models depend heavily on parameter tuning

Possible Improvements
Use semi-supervised or supervised models (e.g., XGBoost)
Apply advanced imbalance handling (SMOTE, cost-sensitive learning)
Feature engineering based on transaction patterns (time, frequency, velocity)
Hyperparameter optimization
