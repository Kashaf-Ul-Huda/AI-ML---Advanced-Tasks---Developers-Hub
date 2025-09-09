
---

## 📌 **Task 5 – Auto-Tagging Support Tickets (LLM)**

# 🎫 Auto-Tagging Support Tickets using LLMs

## 📍 Objective
Automatically classify and tag support tickets into categories using **Logistic Regression (baseline)** and **DistilBERT (LLM fine-tuned)**.  

Supports **multi-class predictions** with top-3 most probable tags.

---

## 📊 Dataset
- **Custom Support Tickets Dataset** (CSV)  
- Text fields: `Ticket Subject`, `Ticket Description`  
- Target: `Ticket Type`  

---

## ⚙️ Methodology
1. **Data Preparation**
   - Combine subject + description → single text field  
   - Clean text (lowercasing, remove URLs, special chars)  
   - Handle missing/rare labels  

2. **EDA & Visualization**
   - Distribution of ticket types  
   - WordClouds + top keywords per label  
   - Ticket length distribution  

3. **Models**
   - **Baseline:** TF-IDF + Logistic Regression  
   - **LLM Approach:** DistilBERT fine-tuned with Hugging Face Trainer  

4. **Evaluation**
   - Metrics: Accuracy, Macro F1, Precision, Recall  
   - Confusion Matrix & Classification Report  

5. **Inference**
   - Single & batch prediction functions with **top-3 tag probabilities**  

---

## ✅ Results
- **Baseline (LogReg + TF-IDF):** ~70–75% accuracy, decent baseline  
- **DistilBERT Fine-tuned:** ~80–85% accuracy, higher F1 across all classes  

---
