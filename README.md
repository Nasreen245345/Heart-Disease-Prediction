# Heart-Disease-Prediction

## Project Overview
This project is a binary classification ML model to predict if a person has heart disease based on medical features. The dataset used is the UCI Heart Disease Dataset.

---

## Dataset Features

| Feature | Description |
|---------|-------------|
| Age | Age of the patient |
| Sex | Gender (0 = Female, 1 = Male) |
| ChestPainType | Type of chest pain |
| BloodPressure | Resting blood pressure (mm Hg) |
| Cholesterol | Serum cholesterol (mg/dl) |
| FBS_Over_120 | Fasting blood sugar > 120 mg/dl (1 = True; 0 = False) |
| EKG_Results | Resting electrocardiographic results |
| MaxHeartRate | Maximum heart rate achieved |
| ExerciseAngina | Exercise-induced angina (1 = Yes; 0 = No) |
| ST_Depression | ST depression induced by exercise relative to rest |
| Slope_ST | Slope of the peak exercise ST segment |
| NumVesselsFluro | Number of major vessels (0–3) colored by fluoroscopy |
| Thallium | Thallium stress test result |
| HeartDisease | Target variable (0 = Absence, 1 = Presence) |

---

## Project Steps

1. Load dataset using pandas.  
2. Rename columns to remove spaces.  
3. Encode target column HeartDisease (Presence → 1, Absence → 0).  
4. Standardize features using StandardScaler.  
5. Exploratory Data Analysis (EDA):  
   - Target distribution plot  
   - Correlation heatmap  
6. Split data into train (80%) and test (20%).  
7. Train Logistic Regression model.  
8. Make predictions and probability estimates.  
9. Evaluate model:  
   - Accuracy  
   - Classification report  
   - Confusion matrix  
   - ROC curve and AUC  
   - Feature importance plot  

---

## Technologies Used

- Python  
- Pandas & NumPy  
- Matplotlib & Seaborn  
- Scikit-learn (Logistic Regression, Train/Test Split, StandardScaler, Metrics)

---

## How to Run

bash
git clone https://github.com/<your-username>/AI-ML-Internship-Task3-Heart-Disease-Prediction.git
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook HeartDiseasePrediction.ipynb

## Results

- **Logistic Regression Accuracy:** 0.91 (~91%)
- **Classification Report:**

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.91      | 0.94   | 0.93     | 33      |
| 1     | 0.90      | 0.86   | 0.88     | 21      |

- **Macro Average:** Precision 0.91, Recall 0.90, F1-Score 0.90  
- **Weighted Average:** Precision 0.91, Recall 0.91, F1-Score 0.91  
- Confusion matrix and ROC curve show good prediction performance

---

## Future Improvements

- Try models: Random Forest, XGBoost, SVM
- Hyperparameter tuning for better accuracy
- Add cross-validation
- Deploy as a web application for real-time prediction
