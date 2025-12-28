# Transformer Encoder–Based Text Classification on the Reuters Dataset

This repository contains the implementation and analysis of a Transformer encoder–based model for multi-class text classification on the Reuters dataset.  
The project is developed as part of the **Deep Learning (CDS301)** course and focuses on understanding the impact of Transformer depth, efficiency, and performance compared to traditional recurrent neural network (RNN) baselines.

---

## 📌 Project Overview

The primary objective of this project is to:
- Implement **encoder-only Transformer architectures** for text classification
- Study the effect of **varying the number of encoder blocks** (3, 5, and 7)
- Compare Transformer performance with **six baseline RNN models** implemented in Assignment-1
- Analyze **performance, parameter efficiency, and generalization behavior**

All experiments are conducted on the **Reuters newswire topic classification dataset** using **Macro F1-score** as the primary evaluation metric.

---

## 🧠 Models Considered

### Transformer Models (trained in this project)
- Transformer Encoder with **3 blocks**
- Transformer Encoder with **5 blocks**
- Transformer Encoder with **7 blocks**

### Baseline Models (from Assignment-1)
- SimpleRNN  
- LSTM  
- GRU  
- Bidirectional SimpleRNN  
- Bidirectional LSTM  
- Bidirectional GRU  

Baseline models are used as **reference baselines**, and their Macro F1-scores are compared with Transformer models.

---

## 🔬 Experimental Setup

- **Dataset:** Reuters (46 classes)
- **Vocabulary size:** 10,000
- **Sequence length:** 200
- **Embedding dimension:** 32
- **Number of attention heads:** 4
- **Training epochs:** 10
- **Evaluation metric:** Macro F1-score

The Transformer architecture includes:
- Token + positional embeddings
- Multi-head self-attention
- Feed-forward networks with residual connections and layer normalization
- Global average pooling for sequence aggregation

---

## 📊 Evaluation & Analysis

The project includes:
- Macro F1-score comparison across all models
- Confusion matrices for Transformer models (3, 5, 7 blocks)
- Comparative visualization of Transformer depth
- Parameter count vs performance analysis
- Parameter efficiency analysis (F1 per million parameters)
- Relative performance improvement over baseline models

Key observation:
> The **3-layer Transformer** achieves the best trade-off between performance and parameter efficiency, while deeper Transformer models do not yield proportional gains.

---

## 📁 Repository Structure

