#  Logistic Regression on Heart Disease Dataset

This project demonstrates the use of **Logistic Regression** to predict the presence of heart disease based on various patient attributes using Python. The dataset used is `Heart.csv`, and the model is trained and evaluated using Scikit-learn.

---

#  Dataset Description

The dataset contains various features related to patient medical history. Key columns include:

- `Age`: Age of the patient  
- `Sex`: Gender  
- `ChestPain`: Type of chest pain  
- `RestBP`: Resting blood pressure  
- `Chol`: Serum cholesterol  
- `Fbs`: Fasting blood sugar > 120 mg/dl  
- `RestECG`: Resting electrocardiographic results  
- `MaxHR`: Maximum heart rate achieved  
- `ExAng`: Exercise-induced angina  
- `Oldpeak`: ST depression induced by exercise  
- `Slope`: Slope of peak exercise ST segment  
- `Ca`: Number of major vessels colored by fluoroscopy  
- `Thal`: Thalassemia  
- `AHD`: Presence of heart disease (target variable)

---

#  Technologies Used
  
- Pandas  
- Scikit-learn    
- StandardScaler (for feature scaling)

---

#  Steps Performed

1. **Data Loading**  
   Loaded the dataset from CSV using `pandas`.

2. **Data Cleaning & Encoding**  
   - Dropped unnecessary columns like `Unnamed: 0`  
   - Encoded categorical variables (`ChestPain`, `Thal`, `AHD`) using `.astype('category').cat.codes`  
   - Removed null values

3. **Feature Selection**  
   - Features (X): All columns except `AHD`  
   - Target (Y): `AHD`

4. **Data Splitting**  
   - Split the data into training and testing sets (70:30 ratio)

5. **Feature Scaling**  
   - Applied `StandardScaler` to normalize the features

6. **Model Training**  
   - Trained a `LogisticRegression` model with the training data

7. **Model Evaluation**  
   - Achieved ~**85.17% accuracy** on training data  
   - Achieved ~**86.67% accuracy** on test data

---

#  Results

The logistic regression model is effective in predicting heart disease using key health indicators. Accuracy metrics suggest a well-generalized model for this classification task.

---
