# 🚀 PathGenie: Skill-Based Job Recommendation System

Live URL: http://pathgenie-job-recommendeation-system44.streamlit.app/

**PathGenie** is an AI-powered, end-to-end job recommendation platform that leverages supervised and unsupervised machine learning, resume parsing with NLP, and neural networks to recommend the most suitable career paths based on individual skill sets.

> Built with `Streamlit`, `scikit-learn`, `TensorFlow`, and `spaCy`.

---

## 🔍 Features

### ✅ Supervised Learning – Job Role Prediction
- Predicts job roles using input like skills, domain, and experience.
- Outputs recommended job titles with confidence scores.
- Models used: `Logistic Regression`, `Random Forest`, etc.

### ✅ Unsupervised Learning – Candidate Clustering
- Clusters similar candidates using `K-Means` / `DBSCAN`.
- Reveals natural groupings in skills and domains.
- Suggests trending jobs for each cluster group.

### ✅ NLP-Based Resume Parsing
- Extracts skills, education, and experience from `.pdf` and `.docx` resumes.
- Uses `spaCy`/`NLTK` pipelines and entity matching for precise parsing.

### ✅ Neural Network – Match Score Prediction
- Compares resume vectors with job descriptions.
- Uses a `Feedforward Neural Network` (ANN) in TensorFlow/Keras.
- Calculates a compatibility score between profile and job role.

### ✅ Model Evaluation Dashboard
- Confusion Matrix, Classification Reports
- Precision-Recall Curve
- Training vs. Validation Accuracy graphs (for ANN)

---

## 🧱 Tech Stack

| Layer        | Tools/Libraries                                                                 |
|--------------|----------------------------------------------------------------------------------|
| **Frontend** | `Streamlit`, `HTML`, `CSS`, `Bootstrap`, `Jinja2` (if Flask used previously)    |
| **Backend**  | `Python`, `Flask`, `pandas`, `NumPy`, `Plotly`                                  |
| **ML/NLP**   | `scikit-learn`, `TensorFlow/Keras`, `spaCy`, `NLTK`, `joblib`                   |
| **File IO**  | `PyPDF2`, `python-docx`                                                         |
| **Deployment** | Render / Heroku / Localhost                                                   |

---

## 📁 Project Structure

PathGenie/
├── main.py
├── requirements.txt
│


├── dataset/
│ ├── job_skills_dataset_corrected.csv
│ ├── learning_resources_dataset.csv
│ └── unique.txt
│


├── supervised/
│ ├── logistic_regression_model.pkl
│ ├── random_forest_model.pkl
│ └── ...
│


├── unsupervised/
│ ├── cluster_predictor.py
│ └── cluster_labels.pkl
│


├── neural_network/
│ ├── ann2.ipynb
│ └── match_score_model.h5
│


├── pages/
│ ├── dashboard.py
│ └── resume_parser.py

Install dependencies
pip install -r requirements.txt
Run the Streamlit app

