# 🩸 Early Detection of Menstrual Irregularities using AI

## Resources
You can view or download the full project report in PDF format here:
[Download Full Report (PDF)](https://drive.google.com/file/d/1_dYRaLaP3jO128QUYmdPuJpvj157BaGg/view?usp=sharing)

You can watch the full presentation of the project here:
[Watch Project Presentation](https://www.youtube.com/watch?v=0feW7Xa_eVM)

## 📋 Project Overview
Menstrual health is a vital indicator of overall reproductive well-being. However, irregularities are often underestimated or misdiagnosed. This project leverages **Machine Learning and Deep Learning** to automate the detection of these patterns using objective clinical features.

---

**Clinical Motivation:**
* **14-25%** of women suffer from menstrual irregularities.
* These are often linked to chronic conditions like **PCOS, Endometriosis, and Anemia**.
* **Goal:** To move beyond subjective diagnosis and use data to predict cycle irregularities early.

## 📊 Dataset & Features
The study uses a clinical dataset of **10,000 patient records** with 16 attributes and one binary target variable.

### Target Variable: `duration_abnormality_flag`
* **0 (Normal):** Healthy menstrual pattern.
* **1 (Abnormal):** Presence of a menstrual irregularity.

### Feature Dictionary
| Attribute | Description |
| :--- | :--- |
| `age` | Patient's age. |
| `bmi` | Body Mass Index. |
| `life_stage` | Reproductive stage (e.g., Adolescent, Reproductive). |
| `tracking_duration_months` | Reliability of historical data. |
| `avg_cycle_length` | Average days between periods. |
| `avg_bleeding_days` | Average duration of bleeding. |
| `cycle_length_variation` | Standard deviation (fluctuation). |
| `cycle_variation_coeff` | Relative variability. |
| `bleeding_volume_score` | Intensity of flow. |
| `pain_score` | Dysmenorrhea severity (0-10). |
| `intermenstrual_episodes` | Count of spotting between cycles. |
| `pattern_disruption_score` | Composite score of irregularity. |
| `Oligomenorrhea` | Indicator for infrequent periods. |
| `Polymenorrhea` | Indicator for frequent periods. |
| `Menorrhagia` | Indicator for heavy bleeding. |
| `Amenorrhea` | Indicator for absence of menstruation. |

---

## 📉 Statistical Validation (T-Tests)
We performed Paired T-Tests to ensure our results were not due to random chance.
* **Conclusion:** Neural Networks and Rule-Based models proved to be the most robust strategies.
* **Cost Significance:** The tests confirmed that optimizing for accuracy does *not* necessarily minimize clinical cost, validating the need for our Cost-Sensitive approach.

---

## 🏆 Final Conclusion
The **Cost-Sensitive Deep Learning Model (Keras Model 2)** is the recommended solution. It successfully minimizes the risk of underdiagnosis (False Negatives) while maintaining high precision, fulfilling the project's goal of improving women's health through early AI detection.
