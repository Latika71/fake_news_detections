 📰 Fake News Detection System

An AI-powered web app that detects whether a news article is Real or Fake using Machine Learning and NLP techniques.

## 🔗 Live Demo
[👉 Click here to open app](https://fakenewsdetections-rbmkwetqlkkv65rrbah3gx.streamlit.app)

## ⚠️ Important — Dataset Limitation
This model is trained on **2017–2018 news articles** only.

- It works best on news from that era
- For recent news (2020–2026), predictions may not be accurate
- This is a known ML problem called **Distribution Shift** — when real-world data differs from training data
- For better results on modern news, the model would need to be retrained on newer datasets

## 🛠️ Tech Stack
- Python
- Scikit-learn — Logistic Regression
- TF-IDF Vectorizer — Text to numbers conversion
- Streamlit — Web app UI
- Plotly — Analytics charts
- Jupyter Notebook — Model training

## 📊 Dataset Details
| Property | Details |
|----------|---------|
| Source | Fake.csv + True.csv (Kaggle) |
| Total Articles | 44,898 |
| Fake News | 23,481 articles |
| Real News | 21,417 articles |
| Time Period | 2017 – 2018 |
| Topics | US Politics, World News |

## 🔄 How It Works
1. User pastes a news article
2. Text is cleaned — lowercase, URLs removed, punctuation removed
3. TF-IDF Vectorizer converts text into numbers
4. Logistic Regression model predicts Real or Fake
5. Confidence score is shown

## 📈 Model Performance
| Metric | Score |
|--------|-------|
| Accuracy | 98.1% |
| Precision | 98% |
| Recall | 98% |
| F1-Score | 98% |

## 🗂️ Project Structure
ake-news-detector/
├── app.py                    ← Streamlit web app
├── model.pkl                 ← Trained Logistic Regression model
├── vectorizer.pkl            ← Trained TF-IDF Vectorizer
├── fake_news_detection.ipynb ← Training notebook
└── requirements.txt          ← Python dependencies

## Author
**Latika Chaudhary**
