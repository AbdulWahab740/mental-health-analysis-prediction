# 🧠 Mental Health in Tech - Classification Project

## 📂 Dataset Overview

This dataset explores various factors related to **mental health in the workplace**, especially within the **technology industry**. The goal is to predict whether an individual has sought **treatment for mental health issues** based on multiple workplace, personal, and demographic factors.

---

## 📊 Features

| Feature Name                 | Description                                                        |
|-----------------------------|--------------------------------------------------------------------|
| `Gender`                    | Reported gender identity                                           |
| `self_employed`             | Whether the person is self-employed                                |
| `family_history`            | Family history of mental illness                                   |
| `treatment`                 | **Target variable**: Has the person sought treatment? (Yes/No)     |
| `no_employees`              | Company size                                                       |
| `remote_work`               | Whether they work remotely                                         |
| `tech_company`              | Whether they work in a tech company                                |
| `benefits`                  | Whether employer provides mental health benefits                   |
| `care_options`              | Options for mental health care                                     |
| `wellness_program`          | Presence of mental health wellness program                         |
| `seek_help`                 | Ease of seeking mental health help at work                         |
| `anonymity`                 | Anonymity of mental health issues in the workplace                 |
| `leave`                     | Ease of taking mental health leave                                 |
| `mental_health_consequence` | Consequences of discussing mental health at work                   |
| `phys_health_consequence`   | Consequences of discussing physical health at work                 |
| `coworkers`, `supervisor`   | Comfort level discussing with coworkers/supervisors                |
| `mental_vs_physical`        | Perception of mental vs. physical health importance                |
| `obs_consequence`           | Consequence of mental illness on work                              |

---

## 🛠️ Data Preprocessing

- Cleaned inconsistent labels (e.g., gender values like `Femake`, `Male-ish`, `cis male`)
- Encoded categorical variables using label encoding or ordinal mapping
- Removed irrelevant or low-importance features ( most important )

---

## Problem with the Data
The main issue in the visualization of Treatment with all the other columns is that in most of the columns if the value is `No`, the **Treatment** has equal or more distribution for `YES` rather than `No`. which may cause the bad learning of the model while training.

So we actually has to check whether these graphs actaully has any affect on the treatment which is our Label, while on training. For that, we will use **Cramers Algorithm** to calculate the weightage.

## 🤖 Models Used

- Logistic Regression  
- Random Forest Classifier  
- XGBoost  
- LightGBM
- GaussianNB
- SVC  
- Ensemble Bagging Classifier  

**Evaluation Metrics**:
- ✅ F1-Score (Primary Metric)
- ✅ Accuracy
- ✅ Precision & Recall
- ✅ ROC-AUC

---

## 📌 Project Goal

To build a robust classification model that can **identify individuals likely to seek treatment** for mental health, helping inform policy or workplace support systems.

---

## 📁 Files in This Project

- `notebook.ipynb` – Code for EDA, preprocessing, training & evaluation  
- `models.pkl` – (Optional) Saved best models  
- `requirements.txt` – Python dependencies  
- `README.md` – You’re here!  

---

## 🔍 License

This project is for educational purposes only. Attribution to the original dataset source (e.g., Kaggle or OSMI) if applicable.

---

## 🙋‍♂️ Author

**Abdul Wahab**  
[LinkedIn](https://www.linkedin.com/in/abwahab07) | [GitHub](https://github.com/AbdulWahab07)

