# 🇰🇭 Khmer Stop-word Removal System

## 📌 Project Overview

This project focuses on building a **Khmer Stop-word Removal System** to improve text processing performance in Natural Language Processing (NLP) tasks.

### 💡 Motivation

The main reason for this project is to **prove that stopword removal has a significant impact** on text analysis and machine learning performance.

In Khmer NLP, this problem is even more critical due to:
- No explicit word spacing  
- Complex script and morphology  
- Limited NLP resources  
- High proportion of low-information words (30–50%)  

👉 Many Khmer texts contain a large number of **stopwords** that add noise and reduce model performance.

---

## 🎯 Objectives

- Build a **custom Khmer stopword list**
- Design a **preprocessing pipeline**
- Evaluate the impact of stopword removal
- Prove its effectiveness through experiments

---

## 🧠 Methodology

### 1. Dataset
- Source: Khmer News Classification (CADT-IDRI, HuggingFace)
- Total: 7,344 articles  
- Categories: Politics, Economic, Entertainment, Life, Sport, Technology  

### 2. Preprocessing
- Sentence splitting (។ ៕ ! ?)
- Remove non-Khmer characters
- Remove Khmer numerals (០–៩)
- Tokenization using `khmernltk`

### 3. Stopword Creation
- 510 manually validated stopwords  
- Organized into 10 linguistic categories  
  (pronouns, conjunctions, particles, etc.)

---

## ⚙️ Pipeline
Raw Text → Cleaning → Tokenization → Stopword Removal → Feature Extraction → Model

---

## 📊 Experiments

### 🔬 TF-IDF Analysis

- Stopword removal helps:
  - Reduce noise  
  - Highlight meaningful words  
  - Improve feature quality  

### 🤖 Classification Results

| Model | Accuracy (Raw → Cleaned) |
|------|--------------------------|
| Naive Bayes | 0.876 → 0.873 |
| Logistic Regression | 0.918 → 0.919 |
| Linear SVC | **0.926 → 0.929** |

### ✅ Key Insight

- Stopword removal **improves performance in advanced models**
- Slight decrease in Naive Bayes (due to reliance on word frequency)
- Overall, it proves that **stopwords significantly affect model performance**

---

## 🚀 Key Results

- ~29% of text identified as noise  
- ~30% faster processing  
- Improved Precision & Recall  
- Maintained high retrieval quality (Recall@10 ≈ 0.97)

---

## 🧩 Conclusion

This project successfully demonstrates that:

👉 **Stopword removal has a significant and measurable impact** on Khmer NLP tasks.

- It improves model performance  
- It reduces computational cost  
- It enhances feature quality  

---

## 🔮 Future Work

- Khmer embeddings  
- Transformer models (BERT-style)  
- Domain-specific stopwords  
- Real-time preprocessing API  

---

## 👥 Team

- Ty Kana  
- Theary Sreyneath  
- Chantha Thaitheang  

---

## 📎 Repository

https://github.com/Nagamiji/khmer_stopword_removal_system
