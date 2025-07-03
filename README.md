# parkinsons-disease-detection
# 🧠 Parkinson's Disease Detection using Machine Learning

This project detects Parkinson's disease based on voice measurements using a Decision Tree and Random Forest classifier. The goal is to predict whether a person has Parkinson's disease by analyzing various biomedical voice features.

## 📂 Dataset
- Source: [UCI Machine Learning Repository - Parkinson’s Dataset](https://archive.ics.uci.edu/ml/datasets/parkinsons)
- Contains biomedical voice measurements from 31 individuals (23 with Parkinson’s disease).
- Key Features:
  - Voice frequency measures (Fo, Fhi, Flo)
  - Jitter and Shimmer metrics (frequency and amplitude variations)
  - Noise-to-Harmonics Ratio (NHR), Harmonics-to-Noise Ratio (HNR)
  - Advanced nonlinear dynamical complexity measures (PPE, RPDE, etc.)
  - 
## ✅ Project Workflow

1. **Data Cleaning & Preprocessing**
   - Removed non-informative columns (`name`).
   - Checked for missing values & duplicates.
   - Split data into features (`X`) and target (`y`).
   - Train-test split for evaluation.

2. **Model Building**
   - Trained **Decision Tree Classifier**.
   - Trained **Random Forest Classifier** with 500 trees for robustness.
   - Both models achieved ~92% accuracy.

3. **Evaluation**
   - Accuracy Score, Confusion Matrix, and Classification Report used for evaluation.
   - Decision Tree visualized for interpretability.

4. **Model Saving**
   - Saved trained model using `joblib` for future predictions.
   - Model ready for deployment in batch or real-time environments.
     
 📊 Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn (Decision Tree, Random Forest, Model Evaluation, Scaling)
- Matplotlib & Seaborn (Visualization)
- Joblib (Model Saving)

 ✅ Results
- Both Decision Tree and Random Forest models achieved **~92% accuracy** on test data.
- Key predictive feature: **PPE (Pitch Period Entropy)**, which measures pitch variability.
- The models performed well due to strong predictive features and clean data.

 

