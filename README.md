# 🛠️ AnomaData: Automated Anomaly Detection for Predictive Maintenance
![AnomaData1](https://github.com/user-attachments/assets/b5c2b26f-f267-41ae-a924-8f4d11f208f2)

## 📑 Table of Contents
1. [Project Overview](#-project-overview)  
2. [Data Sources](#-data-sources)  
3. [Data Preprocessing Steps](#-data-preprocessing-steps)  
4. [Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)  
5. [Feature Engineering](#-feature-engineering)  
6. [Model Selection & Training](#-model-selection--training)  
7. [Hyperparameter Tuning](#-hyperparameter-tuning)  
8. [Best Model](#-best-model-random-forest)  
9. [Performance Evaluation](#-performance-evaluation)  
10. [Deployment](#-deployment)  
11. [Future Work](#-future-work)  
12. [Benefits of the Model](#-benefits-of-the-model)  
   - [For Technical Users](#-for-technical-users)  
   - [For Industries & Maintenance Teams](#-for-industries--maintenance-teams)
13. [Conclusion](#-conclusion)
14. [Contributors](#-contributors)  

## 📌 Project Overview
Industries face challenges in maintaining machinery efficiently due to unplanned downtime, leading to increased costs and reduced productivity. This project develops an **Automated Anomaly Detection System** using machine learning to predict potential failures in industrial machines. The system analyzes sensor data and detects anomalies, enabling predictive maintenance to optimize maintenance schedules and enhance equipment lifespan.

## 📊 Data Sources
- **Dataset Name:** AnomaData.xlsx
- **Size:** 18,000+ Rows, 60+ Columns
- **Features:** Machine sensor readings (environmental conditions, system parameters)
- **Target Variable:** `y` (Binary Classification: 1 = anomaly, 0 = normal)
- **Challenges:** Highly imbalanced dataset (minority class represents anomalies)

## 🔍 Data Preprocessing Steps
1. **Data Loading & Inspection:** Handling missing values, duplicates, and inconsistencies.
2. **Outlier Detection & Removal:** Using IQR and Boxplots to eliminate extreme values.
3. **Feature Scaling:** Normalizing numerical features using StandardScaler.
4. **Handling Imbalanced Data:** Applying resampling (oversampling + undersampling) techniques.

## 📊 Exploratory Data Analysis (EDA)
- **Correlation Analysis:** Heatmaps to understand feature relationships.
- **Data Visualization:** Histograms, boxplots, and time-series analysis.
- **Feature Importance:** Identifying key parameters influencing anomaly detection.

## 🔧 Feature Engineering
- **Time-Based Features:** Extracting time-related patterns.
- **Feature Transformation:** Applying logarithmic transformations to reduce skewness.
- **Feature Selection:** Using correlation analysis and tree-based feature importance.

## 🤖 Model Selection & Training
The following machine learning models were evaluated:
- **Naïve Bayes**
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Random Forest Classifier** ✅ *(Best Model: 99.9% Accuracy)*
- **Support Vector Machine (SVM)**
- **Logistic Regression**

### **Hyperparameter Tuning**
- **Grid Search with Cross-Validation** to optimize model performance.
- **Evaluation Metrics:** Accuracy, Precision, Recall, F1-score, ROC-AUC.

## 🏆 Best Model: Random Forest
- **Achieved Accuracy:** 99.9%
- **Reason for Selection:** Best trade-off between precision, recall, and generalization.

## 📈 Performance Evaluation
- **Confusion Matrix & ROC Curve**
- **Precision, Recall, F1-Score**
- **Impact of Handling Imbalanced Data on Model Performance**

## 🚀 Deployment
### **Installation**
To install dependencies, run:
```bash
pip install -r requirements.txt
```

### **Train & Save the Model**
```bash
python train_model.py
```

## 🔮 Future Work
- **Real-Time Deployment:** API-based real-time anomaly detection.
- **IoT Integration:** Continuous sensor data monitoring.
- **Adaptive Learning:** Models that improve with new data.
- **Web Dashboard:** Interactive anomaly visualization.

## 📌 Benefits of the Model
### ✅ **For Technical Users**
- Automates anomaly detection and early warnings.
- Scalable to large datasets and IoT applications.
- Supports model interpretability with SHAP/LIME.

### ✅ **For Industries & Maintenance Teams**
- **Reduced Downtime:** Prevents unexpected machine failures.
- **Optimized Maintenance Costs:** Data-driven repair schedules.
- **Increased Equipment Lifespan & Safety Compliance.**

  ## Conclusion :
- The AnomaData project successfully demonstrated the application of machine learning techniques for predictive maintenance through anomaly detection. Among the evaluated models, the Random Forest initial model emerged as the best performer, achieving an outstanding accuracy of 99.9%.
-	This high accuracy, combined with superior precision, recall, F1-score, and AUC-ROC metrics, makes it the most reliable choice for detecting anomalies in the dataset.
-	The model effectively differentiates between normal and anomalous conditions, ensuring timely identification of potential failures. By leveraging this high-performing model, industries can proactively optimize maintenance strategies, reduce operational downtime, and enhance overall efficiency.


## 🏆 Contributors
- **Komal Sahu**
- **Course**: Data Science Bootcamp, upGrad 

---
