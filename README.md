# 🇬🇧➡️🇳🇵 English to Nepali Language Translator (LSTM + Attention)

This project implements an English-to-Nepali language translation system using an LSTM-based Encoder-Decoder architecture with Attention. The model is built from scratch in Python using deep learning libraries and trained on a parallel corpus of over **100,000 English–Nepali sentence pairs**.

> 🚀 Final Year Bachelor's Project — Natural Language Processing & Machine Translation

---

## 🧠 Project Overview

- **Goal**: Translate English sentences to Nepali using a sequence-to-sequence (Seq2Seq) model.
- **Architecture**: LSTM Encoder-Decoder with Attention Mechanism.
- **Embedding**: Custom Skip-Gram word embeddings (300-dim).
- **Handling Vocabulary**: Rare tokens replaced with `<UNK>`, unknown test tokens shown as `<OOV>`.
- **Training Strategy**: Uses Teacher Forcing for faster and more stable convergence.

---

## 🔧 Key Features

- ✅ Preprocessing pipeline: Tokenization, lemmatization, special token tagging (`<SOS>`, `<EOS>`)
- ✅ Rare words (frequency < 2) replaced with `<UNK>`
- ✅ Custom Skip-Gram Embedding Layer (300-dim)
- ✅ Padding applied to input/output for uniform batch training
- ✅ Bidirectional LSTM encoder and LSTM decoder with Bahdanau attention
- ✅ Probabilistic decoding of each token
- ✅ Evaluation metrics and BLEU score support

---

## 🧪 Experiments & Hyperparameter Tuning

Multiple models were trained with variations in:

- Embedding dimensions
- Hidden units
- Number of layers
- Dropout rate
- Teacher forcing ratio
- Learning rates
- Optimizers (Adam, RMSprop)

All trained models, logs, and checkpoints are available here:

📂 **[👉 Google Drive - Trained Models & Reports](https://drive.google.com/drive/folders/1Fg9hFBSpkhdGC-Wka44f6gRErmVLkwCH?usp=drive_link)**  
_(Replace with your actual link)_

---

## 📊 Evaluation

- WER score used for evaluation
- Manual comparison of translated sentences
- Loss vs. Epoch graphs for training and validation
- Sample translations:
  - EN: *"I love my country."*
  - NP: *"म आफ्नो देशलाई माया गर्छु।"*

---

