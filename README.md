# AiMl-internship
# Titanic Dataset Preprocessing Project 🚢

This project demonstrates how to clean and prepare a real-world dataset (Titanic dataset) for machine learning and analysis. It includes key data preprocessing steps using Python and pandas in Jupyter Notebook.

---

## 📂 Dataset Overview

The dataset used in this project is the **Titanic - Machine Learning from Disaster** dataset from [Kaggle](https://www.kaggle.com/competitions/titanic/data).

It contains information about passengers on the Titanic and whether they survived. This dataset is commonly used for classification problems.

**Key columns include:**
- `PassengerId` — Unique ID
- `Pclass` — Ticket class (1st, 2nd, 3rd)
- `Name` — Passenger name
- `Sex` — Gender
- `Age` — Age in years
- `SibSp` — Number of siblings/spouses aboard
- `Parch` — Number of parents/children aboard
- `Ticket` — Ticket number
- `Fare` — Ticket price
- `Cabin` — Cabin number (many missing values)
- `Embarked` — Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- `Survived` — Survival (0 = No, 1 = Yes)

---

## 🧼 Data Preprocessing Steps

The following preprocessing steps are performed:

1. **Importing and Exploring the Dataset**
   - Checking null values
   - Understanding data types

2. **Handling Missing Values**
   - Filled missing `Age` and `Fare` using mean/median
   - Filled missing `Embarked` using mode
   - Dropped `Cabin` due to too many missing values

3. **Encoding Categorical Variables**
   - Converted `Sex` into binary (0: female, 1: male)
   - One-hot encoded `Embarked` (C, Q, S → new columns)

4. **Normalization**
   - Scaled numerical columns (`Age`, `Fare`, `SibSp`, `Parch`) using `MinMaxScaler`

5. **Outlier Detection & Removal**
   - Used **boxplots** to visualize outliers
   - Removed outliers using **IQR method**

---

## 🔧 Tools Used

- Python 3.x
- Jupyter Notebook
- pandas
- matplotlib
- scikit-learn

---

## 📊 Sample Output

Cleaned dataset with numerical and encoded columns, ready for machine learning models like:
- Logistic Regression
- Decision Trees
- KNN
- SVM

---

## 📁 Files in this Repository

- `Titanic_Project.ipynb` — Jupyter notebook with full preprocessing code
- `titanic.csv` — Raw dataset (if included)
- `README.md` — Project overview and documentation

---

## 🧠 Future Improvements

- Handle `Cabin` column with feature engineering
- Apply advanced imputation (e.g., KNNImputer)
- Train and evaluate machine learning models

---
# 🧠 Logistic Regression - Breast Cancer Classification

This project demonstrates how to use **Logistic Regression** to classify breast cancer tumors as **malignant (M)** or **benign (B)** using the [Breast Cancer Wisconsin (Diagnostic) Data Set](https://www.kaggle.com/uciml/breast-cancer-wisconsin-data). The model is built with **scikit-learn** and evaluated using accuracy, confusion matrix, classification report, and ROC curve.

---

## 📌 Project Tasks

- ✅ Load and clean the dataset
- ✅ Encode categorical labels (M/B) into numerical values (1/0)
- ✅ Standardize features using `StandardScaler`
- ✅ Split dataset into train and test sets
- ✅ Train a Logistic Regression model
- ✅ Evaluate the model using metrics and ROC curve
- ✅ Perform threshold tuning

---

## 📊 Dataset Information

- **Target Column**: `diagnosis`
- **Target Classes**:
  - `M`: Malignant (1)
  - `B`: Benign (0)
- **Features**: 30 numeric features like radius, texture, area, smoothness, etc.
- **Dropped Columns**: `id`, `Unnamed: 32` (not relevant for prediction)

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- scikit-learn

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name


## 🙌 Credits

Dataset from [Kaggle Titanic Competition](https://www.kaggle.com/competitions/titanic)

---

