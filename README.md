#  ML Model Deployment System

An end‑to‑end machine learning deployment project for **student placement prediction**. This system covers the full lifecycle: **data preprocessing, model training, evaluation, inference, and deployment via Flask**, with a styled web interface and Docker support.

---

##  Features
- **Data Preprocessing**: Cleans and encodes student datasets.
- **Model Training**: RandomForest classifier trained on student placement data.
- **Evaluation**: Accuracy, precision, recall, and F1‑score metrics.
- **Inference**: Batch predictions from CSV or single record predictions.
- **Deployment**: Flask API + HTML frontend with custom CSS styling.
- **Containerization**: Dockerfile for reproducible deployment.
- **Experiment Tracking**: MLflow integration for model logging.

---

##  Project Structure
ML MODEL DEPLOYMENT SYSTEM/
│
├── data/                          # Datasets
│   ├── students.csv               # Training dataset with student records
│   └── new_students.csv           # Sample dataset for inference
│
├── mlruns/                        # MLflow experiment tracking logs
│
├── models/                        # Saved models
│   └── model.pkl                  # Trained RandomForest model
│
├── src/                           # Core ML pipeline scripts
│   ├── preprocess.py              # Data preprocessing (cleaning, encoding)
│   ├── train.py                   # Model training script
│   ├── evaluate.py                # Model evaluation (metrics, reports)
│   └── inference.py               # Batch & single inference logic
│
├── templates/                     # Frontend templates (Flask Jinja2)
│   └── index.html                 # Web interface for predictions
│
├── static/                        # Static assets (CSS, JS, images)
│   └── style.css                  # Custom styling for the web interface
│
├── app.py                         # Flask application (serves API + frontend)
│
├── requirements.txt               # Python dependencies
│
├── Dockerfile                     # Containerization setup
│
├── venv/                          # Virtual environment (local dependencies)
│
└── README.md                      # Project documentation
