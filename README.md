# 📊 Student Performance Prediction - Machine Learning Project

## 📖 Project Overview
This machine learning project aims to predict student academic performance based on various socio-economic and educational factors. The project includes both regression (predicting scores) and classification (predicting pass/fail) tasks.

**University**: Université Chouaib Doukkali - Ecole Nationale des Sciences Appliquées d'El Jadida  
**Supervisor**: Pr. Benkirane Fatima Ezzahra  
**Team**: Ariri Abdelaziz, Bardaoui Mohammed, Ettaqafi Ossama, El Attar Fahd

## 🎯 Objectives
- Predict student exam scores (Math, Reading, Writing) using regression models
- Classify students into Pass/Fail categories
- Identify key factors influencing academic performance
- Create an interactive dashboard for performance visualization

## 📁 Dataset
**Student Performance in Exams Dataset** (from Kaggle)
- **1000 student records**
- **Features**:
  - Categorical: Gender, Race/Ethnicity, Parental Education Level, Lunch Type, Test Preparation Course
  - Numerical: Math Score, Reading Score, Writing Score

## 🔧 Methodology

### 1. Data Exploration & Preprocessing
- **Exploratory Data Analysis (EDA)**
- **Data Cleaning**: Handling missing values and outliers
- **Feature Engineering**:
  - Created `verbal_score` (average of reading + writing)
  - Created `pass` column (threshold: average score ≥ 50)
- **Data Encoding**: Label Encoding, One-Hot Encoding, Ordinal Encoding
- **Data Normalization**: StandardScaler
- **Train/Test Split**

### 2. Machine Learning Models

#### 📈 Regression Models (Score Prediction)
- Support Vector Regression (SVR)
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- K-Nearest Neighbors Regressor
- Decision Tree Regressor

#### 🏷️ Classification Models (Pass/Fail Prediction)
- K-Nearest Neighbors (KNN)
- Support Vector Classifier (SVC)
- Decision Trees
- Logistic Regression
- AdaBoost
- XGBoost
- Naive Bayes
- Random Forest
- Multi-Layer Perceptron

### 3. Advanced Techniques
- **Feature Selection** using Random Forest importance
- **Dimensionality Reduction** with PCA
- **Handling Class Imbalance** with SMOTE, ADASYN, SMOTE-TOMEK
- **Hyperparameter Tuning** with GridSearchCV

## 📊 Results & Performance

### Regression Results
- Best performing models achieved R² scores up to 0.979 for total score prediction
- Lowest RMSE values across different score types

### Classification Results
- Multiple datasets tested (original, feature-selected, PCA-transformed)
- Various resampling methods compared
- Best models achieved accuracy up to 89.5%
- Comprehensive metrics tracking (precision, recall, F1-score)

## 📈 Data Visualization
Interactive Tableau dashboard created with:
- Overall performance metrics
- Score breakdown by gender and parental education
- Impact of test preparation courses
- Pass rates by ethnic groups
- Mention distribution analysis

**Dashboard Link**: [Tableau Public Visualization](https://public.tableau.com/app/profile/ossama.ettaqafi/viz/VisutalisationProjectML2_v2024_3/Dashboard)

## 🔍 Key Insights
- **Test Preparation**: Students who completed preparation courses scored significantly higher
- **Gender Differences**: Girls outperformed boys in verbal scores, boys in math
- **Parental Education**: Higher parental education levels correlated with better student performance
- **Lunch Type**: Standard lunch (vs free/reduced) associated with better results
- **Ethnic Groups**: Gradual improvement in pass rates from Group A to Group E

## 🛠️ Technologies Used
- Python (Pandas, NumPy, Scikit-learn, XGBoost)
- Jupyter Notebook
- Tableau for visualization
- WandB for experiment tracking
- SMOTE, ADASYN for data resampling

## 📁 Project Structure
<img width="469" height="484" alt="image" src="https://github.com/user-attachments/assets/a0f53b00-5087-4b55-a231-81e593a97de3" />

## 🚀 Getting Started
1. Clone the repository
2. Install required packages: `pip install -r requirements.txt`
3. Run Jupyter notebooks in sequence:
   - Data Exploration & Preprocessing
   - Regression Models
   - Classification Models
4. Explore the Tableau dashboard for visual insights

## 👥 Contributors
- Ariri Abdelaziz
- Bardaoui Mohammed  
- Ettaqafi Ossama
- El Attar Fahd

## 🙏 Acknowledgments
We thank Pr. Benkirane Fatima Ezzahra for her guidance and supervision throughout this project.
