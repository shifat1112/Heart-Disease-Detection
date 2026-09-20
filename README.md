```markdown
# ❤️ Heart Disease Prediction Using Machine Learning

A machine learning research project for predicting heart disease from clinical, demographic, behavioral, and lifestyle-related health features.

The project evaluates multiple machine learning algorithms and explores model interpretability using SHAP to understand the contribution of important features.

---

## 📌 Overview

Heart disease is a major healthcare challenge where early identification of risk can support preventive healthcare and clinical decision-making.

This project investigates the use of machine learning for heart disease prediction using structured health data.

The workflow includes:
- Data preprocessing
- Missing-value handling
- Categorical feature encoding
- Feature scaling
- Feature selection
- Machine learning model training
- Model comparison
- Cross-validation
- ROC-AUC analysis
- Precision-recall analysis
- Confusion matrix analysis
- SHAP-based model interpretation
- Probability calibration
- Ensemble experimentation

---

## 🎯 Objectives

The main objectives of this project are:
1. Compare different machine learning models for heart disease prediction.
2. Identify relevant features associated with heart disease prediction.
3. Evaluate models using multiple classification metrics.
4. Analyze model behavior using interpretability techniques.
5. Explore machine learning approaches that could support clinical decision-support systems.

---

## 📊 Dataset

The research dataset contains:
- **1,961 patient records**
- **16 selected features**
- Clinical variables
- Demographic variables
- Behavioral variables
- Lifestyle-related variables

### Target Variable

`has_cardiovascular_disease`

This represents a binary heart disease classification outcome.

### Selected Features

The project uses features including:
- Age
- Gender
- Chest pain type
- Systolic blood pressure
- Blood sugar
- Pulse rate
- Shortness of breath
- Blood pressure status
- BMI
- Family history of heart disease
- Smoking status
- Diabetic status
- Hypertensive profile
- Physical activity
- Diet type

---

## 🔬 Machine Learning Workflow

```text
Raw Health Data
       ↓
Data Cleaning
       ↓
Missing Value Handling
       ↓
Categorical Encoding
       ↓
Feature Scaling
       ↓
Feature Selection
       ↓
Train/Test Split
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Interpretability Analysis
       ↓
Prediction

```

---

## 🤖 Machine Learning Models

The project evaluates several classification algorithms:

| Model | Purpose |
| --- | --- |
| **Decision Tree** | Interpretable tree-based classification |
| **Random Forest** | Ensemble classification |
| **XGBoost** | Gradient boosting for structured data |
| **SVM** | Margin-based classification |
| **Naive Bayes** | Probabilistic classification |
| **MLP Neural Network** | Neural-network-based classification |

The notebook also explores LightGBM and a soft-voting ensemble for additional experimentation.

---

## ⚙️ Data Preprocessing

The preprocessing pipeline includes the following steps:

* **Missing Values:**
* Numerical missing values are handled using median imputation.
* Categorical missing values are handled using mode imputation.


* **Categorical Encoding:** Categorical variables are transformed using one-hot encoding.
* **Feature Scaling:** Continuous variables are standardized using `StandardScaler`.
* **Feature Selection:** A Random Forest-based feature selection approach is used to identify relevant features before model training.

---

## 📈 Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* Macro F1-score
* ROC-AUC
* Confusion Matrix
* Precision-Recall Curve
* Calibration Curve
* Cross-validation

*Multiple metrics are considered because accuracy alone may not adequately describe performance in healthcare classification problems.*

---

## 📊 Model Performance

According to the project report, the reported test results were:

| Model | Accuracy | Precision | Recall | Macro F1 | ROC-AUC |
| --- | --- | --- | --- | --- | --- |
| **XGBoost** | 0.9695 | 0.95 | 0.96 | 0.9506 | 0.9650 |
| **Decision Tree** | 0.9593 | 0.92 | 0.95 | 0.9354 | 0.9860 |
| **Random Forest** | 0.9135 | 0.89 | 0.81 | 0.8433 | 0.9517 |
| **SVM** | 0.8982 | 0.86 | 0.79 | 0.8157 | 0.7565 |
| **MLP Neural Network** | 0.8906 | 0.84 | 0.78 | 0.8031 | 0.8435 |
| **Naive Bayes** | 0.8830 | 0.82 | 0.77 | 0.7931 | 0.8557 |

*Note: These values are reported in the accompanying research report.*

---

## 🔍 Model Interpretability with SHAP

SHAP (SHapley Additive exPlanations) is used to investigate how individual features contribute to model predictions.

The analysis examines feature contributions and helps provide a more interpretable view of the machine learning models. The research report discusses features such as:

* Chest pain type (cp)
* Thalassemia (thal)
* Number of major vessels (ca)
* Oldpeak
* Cholesterol (chol)
* Age
* Systolic blood pressure
* Diabetes status

---

## 📉 Visual Analysis

The project includes several visual analyses:

* Age distribution
* Gender and age distribution
* Chest pain distribution
* Heart disease distribution
* Physical activity vs. heart disease
* Correlation heatmap
* Model accuracy comparison
* ROC curves
* Confusion matrices
* Precision-recall curves
* SHAP feature importance
* Calibration curves

---

## 🖼️ Project Visuals

*(Note: Assuming you want to link the images from your `images/` directory, uncomment these links by removing the backticks)*

* `![Machine Learning Workflow](images/workflow.png)`
* `![Correlation Heatmap](images/correlation-heatmap.png)`
* `![Model Comparison](images/model-comparison.png)`
* `![ROC Curves](images/roc-curves.png)`
* `![Confusion Matrix](images/confusion-matrix.png)`
* `![Precision-Recall Curves](images/precision-recall.png)`
* `![SHAP Analysis](images/shap-analysis.png)`
* `![Calibration Curve](images/calibration-curve.png)`

---

## 🛠️ Technologies

* **Programming:** Python 3.10
* **Machine Learning:** Scikit-learn, XGBoost, LightGBM
* **Data Processing:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Explainable AI:** SHAP
* **Development:** Jupyter Notebook, Google Colab, VS Code, Git

---

## 📁 Project Structure

```text
Heart-Disease-Prediction/
│
├── README.md
├── Heart_Disease.ipynb
├── requirements.txt
│
├── images/
│   ├── README.md
│   ├── workflow.png
│   ├── correlation-heatmap.png
│   ├── model-comparison.png
│   ├── roc-curves.png
│   ├── confusion-matrix.png
│   ├── precision-recall.png
│   ├── shap-analysis.png
│   └── calibration-curve.png
│
└── data/
    └── README.md

```

---

## 🚀 Running the Project

**1. Clone the Repository**

```bash
git clone [https://github.com/shifat1112/Heart-Disease-Prediction.git](https://github.com/shifat1112/Heart-Disease-Prediction.git)

```

**2. Navigate to the Project**

```bash
cd Heart-Disease-Prediction

```

**3. Install Dependencies**

```bash
pip install -r requirements.txt

```

**4. Open the Notebook**

```bash
jupyter notebook Heart_Disease.ipynb

```

*You can also run the notebook using Google Colab.*

> **Note:** The original notebook was developed with Google Colab and accesses the dataset through Google Drive. The original dataset is not included in this repository.

---

## 🔐 Data Privacy

The original patient-level dataset is not included in this public repository.

Healthcare datasets may contain sensitive information. Users reproducing this project should use appropriately sourced, anonymized data and follow applicable privacy, ethical, and data-use requirements.

For details about the dataset and privacy considerations, see: `data/README.md`

---

## ⚠️ Disclaimer

This project is an academic machine learning research project.

The predictions generated by the models should not be considered a medical diagnosis or a substitute for professional medical advice. Any real-world clinical deployment would require appropriate clinical validation, privacy protection, fairness evaluation, regulatory compliance, and expert oversight.

---

## 🔮 Future Work

Potential future improvements include:

* Larger and more diverse datasets
* External validation
* Fairness evaluation across demographic groups
* Model optimization
* Real-time monitoring
* Hospital information-system integration
* Wearable-device integration
* Clinician-friendly web/mobile interface
* Lightweight deployment for resource-constrained environments

---

## 👨‍💻 Author

**Md. Shifat Ahmed**

B.Sc. in Computer Science and Engineering

Daffodil International University

---

## 📚 Research Context

This project was developed as an academic machine learning research project focusing on data-driven heart disease prediction and model interpretability.

The work combines classical machine learning, ensemble learning, performance evaluation, and explainable AI techniques to investigate heart disease classification using structured health-related data.

```

```
