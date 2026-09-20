# Dataset Overview: Heart Health in Bangladesh

This directory is intended to store the clinical health dataset used for the machine learning models. 

## 📊 Dataset Description
The research utilizes a structured clinical health database comprising **1,961 patient records** and **16 selected features**. The data encompasses clinical indicators, demographic details, and lifestyle attributes collected in a real-world clinical setting.

### Feature Dictionary
| Feature | Data Type | Description |
| :--- | :--- | :--- |
| **age** | Numerical | Patient’s age in years. |
| **gender** | Categorical | Patient's biological sex. |
| **chest_pain_type** | Categorical | Type of chest pain experienced. |
| **SYSTOLIC** | Numerical | Systolic blood pressure. |
| **SUGAR** | Numerical | Blood sugar level. |
| **PULSE_RATE** | Numerical | Heart rate in beats per minute. |
| **shortness_of_breath** | Categorical | Symptom presence indicating distress. |
| **RESULT_STAT_BP** | Categorical | Blood pressure status (e.g., Normal, Elevated). |
| **BMI** | Numerical | Body Mass Index. |
| **has_cardiovascular_disease** | Categorical | Binary target variable (0 = No, 1 = Yes). |
| **family_history_hd** | Categorical | Family history of heart disease. |
| **smoking_status** | Categorical | Patient’s smoking habits. |
| **diabetic** | Categorical | Diabetes diagnosis status. |
| **profile_hypertensive** | Categorical | Hypertension profile classification. |
| **physical_activity** | Categorical | Level of physical exercise. |
| **diet_type** | Categorical | Dietary habits. |

*Note: Missing numerical values were handled using median imputation, while categorical nulls were assigned mode values or flagged as "Unknown" to preserve statistical reliability*.

## 🔐 Data Privacy & Ethics
**The raw, patient-level dataset is strictly excluded from this repository.** 
Due to the sensitive nature of healthcare records, only anonymized, aggregated, or synthetic sample data may be uploaded. Any reproduction of this workflow must adhere to standard ethical data-use agreements and privacy regulations (e.g., HIPAA, GDPR).
