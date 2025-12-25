# Skin Lesion Classification using ResNet50 (HAM10000)

This repository contains the implementation of my MSc Computer Science
final year dissertation submitted to the University of Greenwich.

## 📌 Project Overview
Skin cancer diagnosis is a critical medical challenge. This project
implements a **transfer learning–based ResNet50 model** for
multi-class classification of dermatoscopic images from the HAM10000 dataset.

- Framework: PyTorch
- Architecture: ResNet50 (ImageNet pretrained)
- Classes: 7 skin lesion categories
- Test Accuracy: 84.52%

⚠️ This project is **for academic research only** and not for clinical use.

## 📂 Dataset
The HAM10000 dataset is **not included** due to licensing restrictions.

Download it from:
https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

After downloading, place it in:

## 🧠 Methodology
- Stratified train/validation/test split
- Class imbalance handled via oversampling
- Data augmentation (flip, rotation, color jitter)
- Adam optimiser + LR scheduling
- Early stopping

## 📊 Results
- Overall accuracy: **84.52%**
- Strong performance on benign and malignant classes
- Common confusion between melanoma and nevi (clinically realistic)

## ▶️ How to Run
```bash
pip install -r requirements.txt
python src/train.py
python src/evaluate.py
