# 🔐 sql_injection_attack_prediction
### Vulnerability Detection Web App (Django + ML Ensemble)

This project is a web-based vulnerability detection system built with Django and integrated with machine learning models. It allows users to upload CSV datasets and uses an ensemble classifier (Naive Bayes, SVM, and KNN) to detect potential vulnerabilities in the data.

## 🚀 Features

- 📁 CSV file upload and preprocessing
- 🧠 Ensemble learning using:
  - Gaussian Naive Bayes
  - Support Vector Machine
  - K-Nearest Neighbors
- 📊 Evaluation metrics: Accuracy, Precision, Recall, F1 Score
- 💾 Model persistence with automatic retraining if needed
- ⚠️ Handles version mismatches with robust model loading/training logic

## 🛠️ Tech Stack

- **Backend**: Django
- **ML Libraries**: scikit-learn, pandas, pickle
- **Storage**: Local filesystem for model caching


## ⚙️ Setup Instructions

1. Clone the repository:
```bash
   git clone https://github.com/your-username/vulnerability-detection-django.git
   cd vulnerability-detection-django
```

2.Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the Django development server: run.py

5. Visit http://127.0.0.1:8000/index.html in your browser.


📌 Notes
Trained models are saved to the model/ directory.
A new model is trained automatically if no model is found or the version is incompatible.
Ensure your uploaded dataset includes a Label column for supervised learning.
