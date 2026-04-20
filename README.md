# 📧 Spam Mail Detection

A machine learning project that automatically classifies emails as **spam** or **ham (not spam)** using Natural Language Processing (NLP) techniques in Python.

---

## 🚀 Demo

> Paste a sample email → get an instant prediction: **Spam** or **Ham**

---

## 📌 Features

- ✅ Classifies emails as Spam or Ham with high accuracy
- ✅ Text preprocessing pipeline (cleaning, tokenization, stopword removal)
- ✅ Feature extraction using TF-IDF / Bag of Words
- ✅ Trained and evaluated on a real-world email dataset
- ✅ Clean and simple Python codebase

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core language |
| Pandas & NumPy | Data manipulation |
| Scikit-learn | ML model & vectorization |
| NLTK / re | Text preprocessing |
| Matplotlib / Seaborn | Data visualization |
| Jupyter Notebook | Experimentation & EDA |

---

## 📁 Project Structure

```
spam-mail-detection/
│
├── dataset/
│   └── mail_data.csv
│
├── notebooks/
│   └── spam_detection.ipynb
│
├── src/
│   ├── preprocess.py
│   ├── train.py
│   └── predict.py
│
├── model/
│   └── spam_model.pkl
│
├── requirements.txt
└── README.md
```
## ⚙️ Installation & Setup

### 1. Clone the repository
git clone https://github.com/your-username/spam-mail-detection.git
cd spam-mail-detection

### 2. Create a virtual environment
python -m venv venv
source venv/bin/activate

### 3. Install dependencies
pip install -r requirements.txt

---

## ▶️ Usage

### Run the Jupyter Notebook
jupyter notebook notebooks/spam_detection.ipynb

### Predict on a custom email
from src.predict import predict_email

email = "Congratulations! You've won a $1,000 gift card. Click here to claim now."
result = predict_email(email)
print(result)  # Output: SPAM

---

## 📊 Model Performance

| Metric    | Score |
|-----------|-------|
| Accuracy  | ~97%  |
| Precision | ~98%  |
| Recall    | ~96%  |
| F1-Score  | ~97%  |

> Results may vary slightly based on train/test split and dataset version.

---

## 📂 Dataset

This project uses the SMS Spam Collection Dataset (https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)
which contains 5,572 labeled messages (spam & ham).

- label → spam or ham
- text  → raw message content

---

## 🔍 How It Works

Raw Email Text
     ↓
Text Preprocessing  (lowercase, remove punctuation, stopwords)
     ↓
Feature Extraction  (TF-IDF Vectorizer)
     ↓
ML Classifier       (e.g., Logistic Regression / Naive Bayes)
     ↓
Prediction: SPAM or HAM

---

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (git checkout -b feature/your-feature)
3. Commit your changes (git commit -m 'Add your feature')
4. Push to the branch (git push origin feature/your-feature)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License — see the LICENSE file for details.

---

## 👤 Author

Your Name
- GitHub: https://github.com/your-username
- LinkedIn: https://linkedin.com/in/your-linkedin

---

⭐ If you found this project helpful, please give it a star on GitHub!
