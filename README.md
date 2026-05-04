# 🌸 Flower Species Classifier — EfficientNetB3

A 5-class flower image classifier built using EfficientNetB3 transfer learning with two-phase fine-tuning, achieving **94% validation accuracy** on 860 validation samples.

## 📊 Results

| Class      | Precision | Recall | F1-Score |
|------------|-----------|--------|----------|
| Daisy      | 0.94      | 0.96   | 0.95     |
| Dandelion  | 0.98      | 0.95   | 0.96     |
| Rose       | 0.96      | 0.90   | 0.93     |
| Sunflower  | 0.96      | 0.94   | 0.95     |
| Tulip      | 0.89      | 0.97   | 0.93     |
| **Overall**| **0.95**  | **0.94**| **0.94**|

## 🛠️ Tech Stack
- Python, TensorFlow, Keras
- EfficientNetB3 (ImageNet pre-trained)
- Two-phase training: frozen base → fine-tune top 60 layers
- Data augmentation: rotation, zoom, brightness, shear, horizontal flip
- Callbacks: EarlyStopping, ReduceLROnPlateau

## 📁 Dataset
[Flowers Dataset — Kaggle](https://www.kaggle.com/datasets/alxmamaev/flowers-recognition)

## ▶️ Run on Google Colab
Open `FlowerSpecies_EfficientNetB3_Classifier.ipynb` in Google Colab and upload the dataset zip when prompted.




## 🔢 Confusion Matrix
<img width="702" height="722" alt="Screenshot 2026-05-04 122634" src="https://github.com/user-attachments/assets/0447a829-abec-4061-8969-1a66e1162dd2" />


Evaluated on 860 validation samples — dandelion and tulip performed best, overall accuracy 94%.


## 📂 Dataset Distribution
<img width="661" height="536" alt="Screenshot 2026-05-04 122541" src="https://github.com/user-attachments/assets/259c7a0c-ab75-46da-9042-f93340b45008" />


5-class balanced dataset — dandelion (24.4%), tulip (22.8%), rose (18.2%), daisy (17.7%), sunflower (17.0%).


## 📈 Training Curves
<img width="935" height="327" alt="Screenshot 2026-05-04 122616" src="https://github.com/user-attachments/assets/47a26b57-85d2-4387-8be5-7ebb690b6aab" />


EfficientNetB3 trained in two phases — validation accuracy reached ~94% after fine-tuning top 60 layers.
