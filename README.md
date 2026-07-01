# 🎬 Sentiment Analysis on IMDb Movie Reviews using Word Embedding

> A Deep Learning project for binary sentiment classification using Word Embedding and Neural Networks.

---

## 📖 Project Overview

This project aims to classify IMDb movie reviews into **positive** and **negative** sentiments using **Word Embedding** techniques and a Deep Learning model.

Instead of traditional feature extraction methods such as Bag of Words or TF-IDF, this project learns dense vector representations of words through an **Embedding Layer**, allowing the model to capture semantic relationships between words.

---

## 🎯 Objectives

- Perform sentiment analysis on movie reviews.
- Convert text into dense vector representations using Word Embedding.
- Train a Deep Learning model for binary classification.
- Evaluate model performance.

---

## 📂 Project Structure

```text
Sentiment-Analysis-WordEmbedding/
│
├── Data/
│   └── IMDB_Dataset.csv
│
├── Notebooks/
│   └── IMDB_embedding.ipynb
│
├── Requirements.txt
└── README.md
```

---

## ⚙️ Workflow

```text
Load Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Text Tokenization
      │
      ▼
Padding Sequences
      │
      ▼
Word Embedding Layer
      │
      ▼
Deep Learning Model
      │
      ▼
Training
      │
      ▼
Evaluation

```

---

## 🧹 Text Preprocessing

The following preprocessing steps are applied:

- Convert text to lowercase
- Remove HTML tags
- Remove punctuation
- Remove numbers
- Remove stopwords (optional)
- Tokenization
- Sequence encoding
- Padding sequences

---

## 🧠 Model Architecture

The proposed model combines **Word Embedding** with a **Convolutional Neural Network (CNN)** for binary sentiment classification. The Embedding layer learns dense vector representations of words, while the convolutional layer extracts local contextual features from the embedded sequences.

### Network Architecture

```text
Input (Padded Sequences)
          │
          ▼
Embedding Layer
(output_dim = 50)
          │
          ▼
Dropout (0.5)
          │
          ▼
Conv1D
(32 Filters, Kernel Size = 4, ReLU)
          │
          ▼
Dropout (0.25)
          │
          ▼
MaxPooling1D
(Pool Size = 2)
          │
          ▼
Flatten
          │
          ▼
Dense (64, ReLU)
          │
          ▼
Dropout (0.5)
          │
          ▼
Dense (1, Sigmoid)
          │
          ▼
Sentiment Prediction
```

### Layer Description

| Layer | Purpose |
|-------|---------|
| **Input** | Receives padded integer-encoded review sequences. |
| **Embedding** | Learns 50-dimensional dense word vectors during training. |
| **Dropout (0.5)** | Reduces overfitting by randomly disabling neurons. |
| **Conv1D** | Extracts local semantic patterns using 32 filters with a kernel size of 4. |
| **Dropout (0.25)** | Improves model generalization after feature extraction. |
| **MaxPooling1D** | Downsamples feature maps while retaining the most informative features. |
| **Flatten** | Converts feature maps into a one-dimensional feature vector. |
| **Dense (64, ReLU)** | Learns higher-level representations for classification. |
| **Dropout (0.5)** | Provides additional regularization before the output layer. |
| **Dense (1, Sigmoid)** | Outputs the probability of the review being positive. |

### Model Summary

- **Input:** Integer-encoded padded review sequences
- **Embedding Dimension:** 50
- **Feature Extractor:** 1D Convolutional Neural Network (CNN)
- **Hidden Layer:** Dense (64 neurons, ReLU)
- **Output Layer:** Sigmoid activation for binary classification
- **Loss Function:** Binary Crossentropy
- **Prediction:** Positive or Negative Sentiment

---

## 📈 Evaluation

The model is evaluated using:

<img width="831" height="75" alt="image" src="https://github.com/user-attachments/assets/6b4d574c-49e1-4063-ad79-66618d56a916" />

- BinaryCrossentropy
- Evaluate

---

## 🚀 Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

---

## 💻 Installation

Clone the repository:

```bash
git clone https://github.com/Ramin0036/Sentiment-Analysis-WordEmbedding.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
jupyter notebook
```

---

## 📌 Example Prediction

<img width="527" height="121" alt="Screenshot 2026-07-01 022744" src="https://github.com/user-attachments/assets/3ca3fc9a-119f-4c95-aa4d-51db23051b1e" />

---

## 👨‍💻 Author : Ramin Allahverdizadeh

GitHub: https://github.com/Ramin0036

---
