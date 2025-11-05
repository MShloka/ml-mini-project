# ml-mini-project
ML mini project for semester 5

# Author: Shloka Anil Mengade

# 🗾 Japanese Sentence Level Classifier

A mini Machine Learning project that predicts the **JLPT difficulty level (N5–N1)** of a given Japanese sentence.  
Built using **Python, Scikit-Learn, Fugashi**, and **Gradio**.

---

## Overview
This project classifies Japanese sentences into JLPT levels based on their vocabulary and grammar complexity.  
It tokenizes the text using `fugashi`, transforms it into TF-IDF features, and trains a **Multinomial Naive Bayes** model.

---

## Features
- Tokenization of Japanese text using **MeCab (Fugashi)**
- Text vectorization using **TF-IDF**
- JLPT Level classification (N5–N1)
- Interactive web demo built with **Gradio**
- Simple, lightweight, and fast to train

---

## Tech Stack
- Python  
- Pandas, Scikit-Learn, Fugashi, Joblib, Gradio  
- Jupyter / Google Colab  

---

## Project Sturucture
Japanese-Level-Classifier/
│
├── data/
│   └── japanese.csv
│
├── models/
│   ├── japanese_level_model.joblib
│   └── vectorizer.joblib
│
├── JLPT_Level_Classifier.ipynb
├── requirements.txt
└── README.md


---

## Model Performance
- Algorithm: **Multinomial Naive Bayes**  
- Vectorizer: **TF-IDF (max_features=3000)**  
- Dataset size: 50 sentences (custom CSV)  
- Accuracy: *Varies due to small dataset, but demonstrates full ML pipeline*  

---

## Demo
### 🔗 [Try the Gradio Live App](https://1a72f484d62159fbed.gradio.live/)  
*(Note: The link expires after each session)*  

---

## Future Scope
- Expand dataset for better accuracy
- Add support for automatic level estimation from longer texts or dialogues
- Deploy the Gradio app permanently on Hugging Face Spaces or Streamlit

---

## 🪜 How to Run Locally
```bash
# 1. Clone the repo
git clone https://github.com/MShloka/ml-mini-project.git
cd ml-mini-project

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the notebook
jupyter notebook ML-mini-project.ipynb
