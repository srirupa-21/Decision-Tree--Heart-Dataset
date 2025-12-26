# 🫀 Heart Disease Prediction using Decision Tree

This project demonstrates how to build, train, evaluate, and visualize a **Decision Tree Classifier** using the **Heart Disease dataset**.  
It is designed for **beginners** to understand machine learning workflows step by step.

---

## 📌 Project Overview

The goal of this project is to predict whether a person has heart disease based on medical attributes such as age, cholesterol level, blood pressure, and other clinical features using a **Decision Tree model**.

---

## 📂 Dataset

- **Dataset Name:** Heart Disease Dataset  
- **Target Column:** `target`  
  - `0` → No heart disease  
  - `1` → Heart disease present  

The dataset contains both **numerical and categorical features**, making it suitable for Decision Tree models.

---

## 🛠️ Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  

---

## 🧠 Machine Learning Workflow

### 1️⃣ Data Exploration
- Displayed dataset shape and column names  
- Viewed first 5 rows  
- Identified target and feature columns  
- Checked missing values and data types  

---

### 2️⃣ Data Preprocessing
- Handled missing values (if any)  
- Separated features (**X**) and target (**y**)  
- Split data into:
  - Training set: **80%**
  - Testing set: **20%**
- Used `random_state = 42` for reproducibility  

---

### 3️⃣ Model Building
- Built a **Decision Tree Classifier**
- Used:
  - `criterion = 'gini'`
  - `random_state = 42`
- Trained the model on training data  
- Predicted results on test data  

---

### 4️⃣ Model Evaluation
- Calculated:
  - Accuracy Score  
  - Confusion Matrix  
  - Classification Report  
- Achieved **~98–99% accuracy**  
- Both classes were predicted very well  

---

### 5️⃣ Tree Depth Experiment
Tested multiple values of `max_depth`:
- `max_depth = 2` → Underfitting  
- `max_depth = 5` → Best performance  
- `max_depth = None` → Overfitting  

---

### 6️⃣ Tree Visualization
- Visualized the best-performing Decision Tree  
- Included:
  - Feature names  
  - Class names  
- Made the model easy to interpret  

---

### 7️⃣ Hyperparameter Comparison
- Compared:
  - `criterion = 'gini'` vs `criterion = 'entropy'`
- Tested different values of:
  - `min_samples_leaf`
- Observed that:
  - Gini and Entropy give similar results  
  - Moderate `min_samples_leaf` improves generalization  

---

## 📊 Key Results

- **Accuracy:** ~98–99%  
- **Best Model:** Decision Tree with controlled depth  
- **Observation:** Decision Trees can overfit if not properly tuned  

---

## ✅ Conclusion

- Decision Trees are highly interpretable and suitable for medical datasets  
- Parameter tuning (`max_depth`, `min_samples_leaf`) is essential  
- Ensemble methods can further improve performance  
- This project provides a strong foundation for understanding tree-based models  

---

## 📁 Files in Repository

- `Heart_Disease_Decision_Tree.ipynb` – Complete implementation  
- `heart.csv` – Dataset  
- `README.md` – Project documentation  

---

## 🚀 Future Improvements

- Try **Random Forest** or **Gradient Boosting**  
- Perform **cross-validation**  
- Add **feature importance analysis**  
