# 📰 Fake News Detection using BiLSTM and BERT Tokenizer

This project is focused on detecting **fake** vs **real** news using deep learning. It combines the power of **BERT tokenization** with a **Bidirectional LSTM** neural network to effectively classify news articles based on their content.

---

## 🚀 Project Overview

In an era where misinformation spreads rapidly, fake news detection has become critical. This project aims to build an efficient binary text classifier that distinguishes between **fake** and **real** news using:

- A dataset containing labeled news articles
- BERT-based tokenization to capture context
- A BiLSTM model trained on encoded text
- Evaluation using classification metrics

---

## 📁 Dataset

The dataset consists of two merged files: one containing **fake** news and the other containing **real** news. Each entry contains:

- `title`: The headline of the article
- `text`: The body of the article
- `label`: Binary label (0 = Fake, 1 = Real)

Example:

| title                      | text                    | label |
|---------------------------|-------------------------|-------|
| "BREAKING: ... "          | "Donald Trump's White…" | 0     |
| "California AG pledges…"  | "SAN FRANCISCO (Reut…"  | 1     |

---


---

## 🧠 Model Architecture

- **Input**: Token IDs (from BERT tokenizer)
- **Embedding**: Trainable embedding layer
- **BiLSTM**: Bidirectional LSTM layer (128 units)
- **Dense**: Fully connected hidden layer
- **Output**: Softmax layer with 2 classes (Fake/Real)

---

## 🧪 Training & Evaluation

- Tokenization: `bert-base-uncased` from Hugging Face
- Loss: `sparse_categorical_crossentropy`
- Optimizer: `Adam`
- Evaluation Metrics: Accuracy, Precision, Recall, F1-Score

Sample Results:
Accuracy: 99.89%
Precision: 99.89%
Recall: 99.89%
F1 Score: 99.89%


---

## 📌 How to Use

### 🔧 Step 1: Install Requirements

```bash
pip install -r requirements.txt

✅ Features
🔎 BERT tokenizer for high-quality input representation

🔁 BiLSTM to capture sequential context from both directions

⚖️ Class weighting to handle imbalance

📊 Robust evaluation using sklearn metrics


📌 Future Improvements
Add attention layer to BiLSTM

Experiment with RoBERTa or DistilBERT embeddings

Integrate with FastAPI or Streamlit for UI

Augment dataset with real-time scraped news

Add adversarial robustness testing



