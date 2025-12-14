# Emotion Classification

This repository contains an NLP project for **emotion classification on short text (tweets)**.  
The goal is to compare classical and deep learning approaches for multi-class emotion detection.

## Project Overview

The project explores and evaluates three different modeling approaches:

- **TF-IDF + Logistic Regression** (strong classical baseline)
- **Word2Vec + BiLSTM** (sequence-based neural model)
- **BERT Fine-Tuning** (transformer-based model)

Each model is trained and evaluated on the same dataset using **Accuracy**, **Macro F1**, and **Weighted F1** to account for class imbalance.

## Emotion Classes

The dataset includes the following emotion labels:

- sadness  
- joy  
- love  
- anger  
- fear  
- surprise  

## Key Results (Test Set)

| Model | Accuracy | Macro F1 | Weighted F1 |
|------|---------|----------|-------------|
| TF-IDF + Logistic Regression | ~0.90 | ~0.85 | ~0.90 |
| Word2Vec + BiLSTM | ~0.78 | ~0.74 | ~0.78 |
| BERT Fine-Tuning | **~0.93** | **~0.88** | **~0.92** |

BERT fine-tuning achieves the best overall performance and the most balanced results across emotion classes.

## Repository Contents

- Jupyter Notebook(s) containing:
  - Data preprocessing and cleaning
  - Exploratory Data Analysis (EDA)
  - Feature engineering
  - Model training and evaluation
  - Performance comparison and conclusions
- `README.md` – project description and summary

## Tools & Libraries

- Python
- scikit-learn
- NLTK
- Gensim
- PyTorch
- Hugging Face Transformers
- Matplotlib / Seaborn

## Conclusion

- Classical models remain strong baselines for short-text classification.
- BiLSTM struggles with limited data and class imbalance.
- **BERT fine-tuning provides the best performance**, capturing contextual and semantic nuances in informal text.

## Author

**Ta Anh Tuan**  
Course: *M508C – Big Data Analytics*  
GitHub: tuan-ta-digit-sense
