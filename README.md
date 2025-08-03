# 🚧 Predictive Maintenance of Industrial Machinery

This project aims to develop a **predictive maintenance model** for industrial machines using real-time and historical sensor data. The goal is to anticipate machine failures such as **tool wear**, **overheating**, and **power issues** using a **Batched Tree Ensemble Classifier**, enabling proactive maintenance and reducing downtime.

---

## 📌 Problem Statement

Industrial machines often experience unplanned failures that lead to operational delays and increased maintenance costs. This system leverages IoT sensor data and machine learning to predict the **type of failure** before it occurs, allowing maintenance to be scheduled in advance.

---

## 🛠️ System Approach

### ✅ System Requirements
- IBM Cloud Platform with Watson Machine Learning
- IBM Watson IoT Platform for real-time data ingestion
- IBM Streaming Analytics for batch processing
- IBM Cloudant or Db2 for storage
- Alert system using IBM Instana or Grafana

### 📚 Libraries Used
- `pandas`, `numpy` – Data processing
- `scikit-learn`, `xgboost` – Model training
- `matplotlib`, `seaborn` – Visualization
- `joblib`, `pickle` – Model saving/loading
- `ibm_watson_machine_learning` – Deployment on IBM Cloud

---

## 🤖 Machine Learning Algorithm

### ✅ Batched Tree Ensemble Classifier
- Aggregates sensor data into time-based batches (e.g., 10-minute windows)
- Extracts features like mean, std, max, and rate of change
- Trains a Random Forest/XGBoost model to classify failure types
- Evaluated using accuracy, F1-score, and feature importance

---

## ⚙️ Deployment

- Model deployed as a REST API via **IBM Watson Machine Learning**
- Integrated with **IBM Watson IoT Platform** for real-time prediction
- Streaming sensor data is preprocessed and fed to the API
- Alerts are triggered based on model outputs

---

## 📈 Results

- **Accuracy:** ~99.5% (using cross-validation)
- **High recall** on critical failures (tool wear, overheating)
- **Reduced unplanned downtime** and **lower maintenance costs**
- Feature importance highlights critical sensor indicators

### 🔍 Pipeline Leaderboard on IBM Watson Studio

![Model Leaderboard](./Screenshot%20(129).png)

### 🔍 Prediction Output Example from IBM Cloud

![Prediction Output](./Screenshot%20(126).png)

---

## ✅ Conclusion

The predictive maintenance model using a Batched Tree Ensemble Classifier effectively identifies machine failures such as tool wear, overheating, and power issues. It leverages real-time sensor data and batch-wise feature extraction to deliver high accuracy and timely predictions. The model's strong performance metrics enable proactive maintenance, reducing unexpected breakdowns and downtime. Integration with IBM Cloud ensures scalable, real-time deployment. Overall, the solution improves operational reliability and lowers maintenance costs.

---

## 🔮 Future Scope

1. **Incorporate Deep Learning Models** – Use LSTM/Transformer architectures to capture temporal dependencies from raw sensor data.
2. **Implement Continuous Learning** – Automate retraining pipelines to improve model adaptability as more failure data becomes available.

---

## 📚 References

- [IBM Watson IoT Platform](https://www.ibm.com/cloud/watson-iot-platform)  
- [IBM Watson Machine Learning](https://www.ibm.com/cloud/machine-learning)  
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)  
- [XGBoost Documentation](https://xgboost.readthedocs.io/)  
- [McKinsey on Predictive Maintenance](https://www.mckinsey.com/business-functions/operations/our-insights/next-generation-maintenance)

---

## 👤 Author

**Yuvaraj Reddy V**  
Presidency University – Computer Science Engineering  
Capstone Project under IBM SkillsBuild
