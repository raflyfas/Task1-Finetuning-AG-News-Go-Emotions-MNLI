# Final Term Deep Learning — Multi-Task NLP with Transformers

Repository ini berisi notebook Final Term mata kuliah Deep Learning yang mengerjakan 3 task NLP berbeda menggunakan model Transformer (DistilBERT).  
Setiap task menggunakan dataset yang berbeda dan memiliki tujuan klasifikasi masing-masing.

Notebook utama:  
`Task 01.ipynb`

---

## Group 6 – Deep Learning

| Nama | NIM |
|---------|------|
| Rahmanda Afebrio Yuris Soesatyo | 1103223024 |
| Rafly Fasha Purnomo Putra | 1103223050 |

---

## Environment & Tools

- Python 3.x  
- PyTorch  
- HuggingFace Transformers  
- HuggingFace Datasets  
- Scikit-learn  
- Matplotlib / Seaborn  

Model utama:
- DistilBERT (`distilbert-base-uncased`)

---

## Overview Task

Notebook ini terdiri dari 3 task utama, masing-masing berbasis dataset yang berbeda.

---

## Data 1 — News Topic Classification (AG News)

### Dataset
- AG News Dataset  
- Kelas:
  - World
  - Sports
  - Business
  - Sci/Tech

### Tujuan
Melakukan klasifikasi topik berita berdasarkan isi teks.

### Tahapan
- Visualisasi distribusi kelas
- Tokenisasi teks menggunakan DistilBERT tokenizer
- Fine-tuning DistilBERT untuk klasifikasi 4 kelas
- Evaluasi performa model

---

## Data 2 — Emotion Classification (Go Emotions)

### Dataset
- Go Emotions Dataset
- Dataset multi-class untuk klasifikasi emosi teks

### Tujuan
Mengklasifikasikan emosi yang terkandung dalam teks.

### Tahapan
- Visualisasi distribusi label emosi
- Preprocessing dan tokenisasi teks
- Fine-tuning DistilBERT untuk emotion classification
- Evaluasi performa model

---

## Data 3 — Natural Language Inference (MNLI)

### Dataset
- Multi-Genre Natural Language Inference (MNLI)

### Tujuan
Menentukan hubungan antara pasangan kalimat (premise dan hypothesis) dengan label:
- Entailment
- Contradiction
- Neutral

### Tahapan
- Visualisasi distribusi kelas MNLI
- Preprocessing pasangan kalimat
- Fine-tuning DistilBERT untuk task NLI
- Evaluasi performa model yang digunakan

---

## Model & Training Strategy

- Pre-trained model: DistilBERT
- Fine-tuning dilakukan secara terpisah untuk setiap task
- Training menggunakan HuggingFace Trainer API
- Evaluasi berdasarkan loss dan accuracy

---

## Visualisasi

Notebook menyertakan visualisasi distribusi data serta monitoring proses training dan evaluasi model.
