# 📰 Fake News Detection Using Machine Learning
This project implements a Fake News Detection System using multiple machine learning classifiers. It leverages a labeled news dataset from Kaggle and applies NLP preprocessing and TF-IDF vectorization to classify news as Fake or Real.

📂 Dataset

Dataset Name: Fake News Detection
Source: Kaggle
Author: Jain Pooja

Dataset ID: jainpooja/fake-news-detection

The dataset contains two CSV files:
Fake.csv – fake news articles
True.csv – real news articles
Each record includes news text along with metadata such as title, subject, and date.


# 📥 Download Dataset Using kagglehub
This project uses kagglehub to download the dataset programmatically.

🔧 Install kagglehub
pip install kagglehub

📌 Download Code
import kagglehub

# Download latest version
path = kagglehub.dataset_download("jainpooja/fake-news-detection")
print("Path to dataset files:", path)
After running this code:
The dataset is downloaded locally
path contains the directory location of Fake.csv and True.csv

👉 Place these CSV files in the same directory as fake news detector.py or update the file paths in the script.


# 📁 Project Structure
Fake-News-Detection/
│
├── fake news detector.py   # Main Python script
├── Fake.csv                # Fake news dataset
├── True.csv                # Real news dataset
├── README.md               # Project documentation


# ⚙️ Technologies Used

Python
Pandas, NumPy
Scikit-learn
TF-IDF Vectorizer
Logistic Regression
Decision Tree
Random Forest
Gradient Boosting


# 🧠 Machine Learning Workflow
Load Dataset (Fake.csv, True.csv)
Label Encoding
Fake → 0
Real → 1
Text Cleaning & Preprocessing
Lowercasing
Removing URLs, punctuation, numbers
TF-IDF Vectorization
Train-Test Split
Model Training
Logistic Regression
Decision Tree
Gradient Boosting
Random Forest
Evaluation
Accuracy score
Classification report
Manual News Testing
User inputs custom news text
Model predicts Fake or Real


# ▶️ How to Run the Project
python "fake news detector.py"
Then enter a news article when prompted to get predictions from all models.


# 📊 Output Example
LR Prediction: Fake News
DT Prediction: Fake News
GB Prediction: Not a Fake News
RF Prediction: Fake News


# 🚀 Future Enhancements

Use deep learning models (LSTM, BERT)
Deploy as a Flask / FastAPI web app
Add confusion matrix & ROC curves
Perform cross-dataset validation
Support multilingual fake news detection


# 📜 Credits & License
Dataset credits belong to the original Kaggle author
Intended for educational and research purposes
