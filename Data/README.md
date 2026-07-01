```markdown
# 🎬 IMDB Dataset of 50K Movie Reviews

A benchmark dataset for **Sentiment Analysis** using IMDb movie reviews.

![Dataset](https://img.shields.io/badge/Dataset-50K_Reviews-blue)
![Task](https://img.shields.io/badge/Task-Sentiment_Analysis-green)
![Language](https://img.shields.io/badge/Language-English-orange)
![Format](https://img.shields.io/badge/Format-CSV-red)
![License](https://img.shields.io/badge/Source-Kaggle-yellow)

---

## 📌 Overview

The **IMDb Dataset of 50K Movie Reviews** is a widely used benchmark dataset for **binary sentiment classification**. It contains **50,000** movie reviews collected from IMDb, where each review is labeled as either **positive** or **negative**.

The dataset is perfectly balanced, making it suitable for training and evaluating machine learning and deep learning models.

---

## 📊 Dataset Information

| Attribute | Value |
|-----------|-------|
| Dataset Name | IMDb Dataset of 50K Movie Reviews |
| Total Samples | 50,000 |
| Positive Reviews | 25,000 |
| Negative Reviews | 25,000 |
| Task | Binary Classification |
| Language | English |
| Format | CSV |

---

## 📂 Dataset Structure

```

IMDB_Dataset.csv
│
├── review
└── sentiment

````

---

## 📝 Features

| Column | Description |
|--------|-------------|
| `review` | Full text of the movie review |
| `sentiment` | Review sentiment (`positive` or `negative`) |

---

## 📈 Class Distribution

| Sentiment | Samples |
|-----------|---------|
| 😀 Positive | 25,000 |
| 😞 Negative | 25,000 |

The dataset is **balanced**, reducing the risk of bias during model training.

---

## ⚙️ Preprocessing

Common preprocessing steps include:

- Convert text to lowercase
- Remove HTML tags
- Remove punctuation
- Remove numbers
- Remove stop words
- Tokenization
- Stemming

---

## 💻 Usage

### Load Dataset

```python
import pandas as pd

df = pd.read_csv("IMDB_Dataset.csv")

print(df.head())
````

### Dataset Shape

```python
print(df.shape)
```

### Class Distribution

```python
print(df["sentiment"].value_counts())
```

---

## ⭐ Acknowledgements

Special thanks to:

* Stanford AI Lab
* IMDb
* Kaggle Community

---
