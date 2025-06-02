# 🌳 Heart Disease Prediction using Decision Tree & Random Forest

This project uses two popular classification algorithms — **Decision Tree** and **Random Forest** — to predict whether a person has heart disease based on clinical data.

---

## 📁 Dataset

- **Source**: [Kaggle – Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- **Samples**: 303
- **Target Variable**: `target` (1 = has disease, 0 = no disease)

---

## 🔧 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn (DecisionTreeClassifier, RandomForestClassifier)
- Matplotlib, Seaborn

---

## ✅ Project Workflow

1. **Data Cleaning**  
   - Checked missing values  
   - Target encoded as binary (0/1)

2. **Train-Test Split**  
   - 80% training, 20% testing

3. **Model Training**  
   - `DecisionTreeClassifier()`  
   - `RandomForestClassifier()`

4. **Model Evaluation**  
   - Accuracy Score  
   - Confusion Matrix  
   - Classification Report  
   - ROC-AUC Score (Optional)

5. **Overfitting Check**  
   - Tree Depth limited (`max_depth=4`)

6. **Feature Importance Analysis**  
   - Bar plot of most influential features

7. **Cross-Validation**  
   - Used `cross_val_score` for Random Forest

---

## 📊 Results

### 🎯 Decision Tree

| Metric | Value |
|--------|-------|
| Accuracy | 85–90% |
| Limiting Depth (max_depth=4) | Prevents Overfitting |

### 🌲 Random Forest

| Metric | Value |
|--------|-------|
| Accuracy | 90–95% |
| Cross-Validation Score | ~91% |
| Feature Importance | Age, Chest Pain Type, Max Heart Rate, etc. |

---

## 📈 Visuals

- Confusion Matrix for both models
- Decision Tree plot (`plot_tree`)
- Feature Importance (bar graph)

---

## 🧠 Key Learnings

- **Decision Trees** are simple but prone to overfitting
- **Random Forest** gives more stable and accurate results
- **Feature importance** helps understand which clinical indicators matter most
- **Cross-validation** ensures model is generalizable

---

## 📂 Files Included

- `heart_model.ipynb`: Jupyter notebook with code
- `heart.csv`: Dataset
- `README.md`: Project summary

---

## ✅ Conclusion

The Random Forest classifier achieved high accuracy and reliability in predicting heart disease. Feature importance analysis further revealed the key health indicators that contribute most to the prediction.
