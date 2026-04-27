# 🧠 Emotion Detection from Text (NLP Project)

This project explores **emotion classification from text** using multiple Natural Language Processing approaches. The goal is to compare traditional machine learning methods with modern neural and transformer-based approaches, and to perform a detailed error analysis.

---

## 📌 Project Overview

Emotion detection is a multi-class text classification task where the model predicts the emotional state expressed in a given sentence (e.g., joy, sadness, anger, fear, etc.).

The project investigates how different NLP techniques perform on this task and what types of linguistic phenomena each method handles well or poorly.

---

## 🎯 Objectives

The main objectives of this project are:

- Select and preprocess a labeled emotion detection dataset
- Train and evaluate at least **three different NLP approaches**
- Compare their performance using consistent evaluation metrics
- Perform a detailed **error analysis**
- Present findings in a structured final presentation

---

## 📊 Dataset

**Emotion Detection from Text (Kaggle)**  
https://www.kaggle.com/datasets/pashupatigupta/emotion-detection-from-text

### Labels include (typical):
- joy
- sadness
- anger
- fear
- love
- surprise

### Input:
- Short text sentences

### Output:
- Emotion label (multi-class classification)

---

## 🧪 Methodology

We compare three main approaches:

### 1. Bag-of-Words (Baseline Model)
- TF-IDF vectorization
- Logistic Regression / Linear SVM
- Captures keyword-level signals

---

### 2. Static Word Embeddings
- Word2Vec or GloVe embeddings
- Sentence representation via averaging embeddings
- Classifier: Logistic Regression / MLP

---

### 3. Contextual Embeddings (Transformer-based)
- BERT / DistilBERT fine-tuning
- Captures context, negation, and compositional meaning

---

### (Optional Extension)
- Zero-shot classification using LLM prompting (e.g., GPT-style model)
- Ensemble methods (BERT + TF-IDF voting)

---

## 📈 Evaluation Metrics

Models are evaluated using:

- Accuracy
- Macro F1-score (important due to class imbalance)
- Confusion matrix analysis

---

## 🔍 Error Analysis

We systematically analyze model failures across:

- **Negation handling**
  - “I am not happy” misclassified as joy in simpler models

- **Ambiguous phrases**
  - “I’m fine” (neutral vs sadness)

- **Sarcasm and irony**
  - “Great… just perfect 🙃”

- **Rare classes**
  - fear, surprise often underrepresented

- **Short / vague text**
  - “ok”, “fine”, “whatever”

- **Contextual dependence**
  - same phrase different meaning depending on context

---

## 🧱 Project Structure
