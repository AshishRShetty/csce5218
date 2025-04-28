# 🖼️ Image Captioning with Flickr30k Dataset

This repository contains two separate but related projects for **image caption generation** using the **Flickr30k** dataset:

---

## 📄 1. Baseline Model

- Built using a **ResNet18 Encoder** and a **simple LSTM Decoder**.
- Used **scheduled sampling**, **mixed precision training**, and **beam search** for generating captions.
- Evaluated using **BLEU-1 to BLEU-4** scores.

---

## 🚀 2. Advanced Model

- Built using a **ResNet101 Encoder** and a **layer-normalized LSTM Decoder with Attention**.
- Incorporated **scheduled sampling**, **gradient clipping**, **mixed precision**, and **beam search decoding**.
- Evaluation included **BLEU**, **ROUGE-L**, and **METEOR** metrics for a more comprehensive performance check.
- Produced noticeably **higher-quality captions** compared to the baseline.
- **Training** stopped after 50 epochs once the loss plateaued, to avoid unnecessary computation.

---

## 🧠 Why Two Separate Models?

I intentionally executed the **Baseline** and **Advanced** models **separately** to keep the work **structured and easy to follow**.  
Each notebook walks through the full pipeline — from data preprocessing, model building, training, to evaluation — making it easier for anyone reviewing the project to understand the improvements step-by-step.

---

## ✅ Summary

- Both models were fully trained and evaluated successfully.
- The **Advanced Model** clearly outperforms the baseline, both qualitatively (better captions) and quantitatively (higher metric scores).
- The baseline model serves as a solid foundation, while the advanced model shows the benefits of deeper encoders, attention mechanisms, and optimization techniques.

---

# 📂 Files Overview

| File | Description |
|:----|:-------------|
| `My_model(Baseline).ipynb` | Baseline model using ResNet18 + simple LSTM. |
| `My_model(Advanced).ipynb` | Advanced model using ResNet101 + attention-based LSTM. |

---

# 📌 Requirements

- Python 3.8+
- PyTorch
- Hugging Face Transformers
- Datasets library
- NLTK
- ROUGE-Score
- Evaluate

(You can install all requirements easily via pip.)

---

# 📬 Contact

Feel free to reach out if you have any questions or suggestions!

---
