# 🩺 Disease Predictor System

## 📘 Summary
The **Disease Predictor System** is a **Streamlit-based web application** that predicts the likelihood of three major diseases:
- **Diabetes**
- **Heart Disease**
- **Parkinson’s Disease**

The system provides a **binary output**:
- `True` → The person is likely diagnosed with the disease.  
- `False` → The person is not likely diagnosed with the disease.  

In addition to prediction, the system offers **personalized Do’s and Don’ts** for users who receive a positive (True) diagnosis — helping them understand lifestyle modifications and precautions to take.  

This project demonstrates the integration of **machine learning models** with an **interactive web interface** using **Streamlit**.

---

## 📂 Dataset
The project uses publicly available and well-known datasets for each disease:

| Disease | Dataset Source | Key Features | Target Variable |
|----------|----------------|---------------|------------------|
| **Diabetes** | Pima Indians Diabetes Dataset | Glucose, Insulin, BMI, Age, etc. | Outcome (0 = No, 1 = Yes) |
| **Heart Disease** | Cleveland Heart Disease Dataset | Age, Sex, BP, Cholesterol, Chest Pain, etc. | Target (0 = No, 1 = Yes) |
| **Parkinson’s Disease** | UCI Parkinson’s Dataset | Voice frequency and amplitude measures | Status (0 = Healthy, 1 = Diseased) |

Each dataset contains both numerical and categorical health indicators used to train classification models.

---

## ⚙️ Process

### 1. **Data Collection & Preprocessing**
- Collected datasets from **Kaggle/UCI repositories**.  
- Cleaned missing or invalid values.  
- Standardized features using **StandardScaler** to normalize input values.  

### 2. **Model Training**
- Built and trained separate machine learning models for each disease using:
  - **Logistic Regression**
  - **Support Vector Machine (SVM)**
- Selected the model with the **highest accuracy** for deployment.

### 3. **Web Application (Streamlit)**
- Integrated the trained models into a **Streamlit web app**.  
- Users can input their health parameters through an easy-to-use interface.  
- On submission, the app displays:
  - Disease prediction result (True/False)
  - Recommended **Do’s and Don’ts** for positive predictions.

### 4. **Output Logic**
- **True** → User is likely diagnosed with the disease.  
  → The system provides actionable tips, lifestyle changes, and dietary recommendations.  
- **False** → User is healthy with respect to that disease.  
  → The app encourages regular check-ups and healthy living.

---

## 💻 Example Workflow
1. Launch the web app using:
   ```bash
   streamlit run app.py
2. Select a disease (Diabetes / Heart / Parkinson’s).
3. Enter the required health parameters.
4. Click Predict.
5. View prediction result and health recommendations.

## 🧾 Conclusion
- The Disease Predictor System effectively predicts the likelihood of Diabetes, Heart Disease, and Parkinson’s Disease using pre-trained machine learning models.
- The system simplifies complex data-driven predictions into clear True/False outputs.
- Integration with Streamlit allows real-time, interactive, and user-friendly diagnosis.
- The Do’s and Don’ts feature enhances user engagement by providing practical guidance for disease management.
- 
