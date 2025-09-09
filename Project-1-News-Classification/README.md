# 📰 News Topic Classifier using DistilBERT

## 📍 Objective
Build and fine-tune a transformer model (DistilBERT) to classify **AG News headlines** into four categories:  
- **World** 🌍  
- **Sports** 🏅  
- **Business** 💼  
- **Sci/Tech** 🔬  

The model is deployed using **Gradio** for interactive inference.

---

## 📊 Dataset
- **AG News Dataset** (from Hugging Face `datasets`)  
- ~120K training samples, 7.6K test samples  
- Each sample: `Title`, `Description`, `Class Index`

---

## ⚙️ Methodology
1. **Preprocessing**
   - Combine Title + Description  
   - Map labels (`Class Index → 0-3`)  
   - Tokenize with `DistilBertTokenizerFast`  

2. **Model Training**
   - Pretrained: `distilbert-base-uncased`  
   - Fine-tuned using Hugging Face **Trainer API**  
   - Optimizer: AdamW with LR=2e-5  
   - Metrics: Accuracy, Precision, Recall, F1  

3. **Evaluation**
   - Macro F1 & Accuracy on test split  
   - Example predictions tested with Gradio UI  

4. **Deployment**
   - Gradio interface for real-time text classification  

---

## ✅ Results
- **Accuracy:** ~85–90% (subset training)  
- **Macro F1:** ~0.85  
- Model performs well across all 4 categories.

---
