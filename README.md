# human-personality-ml-model
This project predicts personality types — Extrovert or Introvert — using machine learning on behavioral data like social activity, alone time, and stage fear for personality and behavior analysis.

# Personality Classification Using Ensemble Learning

## 📘 Description

This project focuses on predicting personality types — **Extrovert** or **Introvert** — using supervised machine learning. The dataset captures key behavioral indicators and habits that differentiate extroverts from introverts. It is ideal for researchers, psychologists, and data scientists interested in social behavior modeling and classification algorithms.

---

## 📊 Dataset Overview

The dataset includes behavioral and lifestyle features such as:

- `Time_spent_Alone`: Hours spent alone daily (0–11)  
- `Stage_fear`: Presence of stage fright (Yes/No)  
- `Social_event_attendance`: Frequency of attending social events (0–10)  
- `Going_outside`: Frequency of going outside (0–7)  
- `Drained_after_socializing`: Whether the person feels drained after socializing (Yes/No)  
- `Friends_circle_size`: Number of close friends (0–15)  
- `Post_frequency`: Frequency of social media posts (0–10)  
- `Personality`: Target variable — Extrovert or Introvert  

---

## 🧠 Machine Learning Models Used

1. **Decision Tree Classifier**
2. **Random Forest Classifier**
3. **Gradient Boosting Classifier**
4. **Stacking Classifier** (Ensemble of Random Forest + Gradient Boosting with Logistic Regression as meta-model)

---

## 🔁 Workflow Summary

1. **Data Preprocessing**
   - Label encoding of categorical variables
   - Feature and target separation
   - Train-test split
   - Feature scaling with `StandardScaler`

2. **Model Training**
   - Fitting individual models (Decision Tree, Random Forest, Gradient Boosting)
   - Building and training a Stacking Classifier

3. **Evaluation**
   - Confusion Matrix
   - Classification Report (Precision, Recall, F1-Score)
   - Heatmaps for visualization

---

## 📈 Confusion Matrix Format

The confusion matrices follow the structure:
```
[[TN FP]
 [FN TP]]
```


- **TN**: True Negatives (Correctly predicted Extroverts)
- **TP**: True Positives (Correctly predicted Introverts)
- **FP**: False Positives (Predicted Introvert, actual Extrovert)
- **FN**: False Negatives (Predicted Extrovert, actual Introvert)

---

## 🛠 Tools & Libraries

- Python (Pandas, NumPy)
- Scikit-learn (`DecisionTreeClassifier`, `RandomForestClassifier`, `GradientBoostingClassifier`, `StackingClassifier`)
- Seaborn & Matplotlib for visualization

---

## 📌 Results

The Stacking Classifier showed improved performance by combining the strengths of individual classifiers using Logistic Regression as a meta-model.

---

## ✅ Future Work

- Hyperparameter tuning with GridSearchCV
- Support for multi-class classification
- Use of deep learning models for more complex patterns

---

## 📂 Folder Structure

