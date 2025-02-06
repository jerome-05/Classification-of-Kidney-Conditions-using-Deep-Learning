# Classification-of-Kidney-Conditions-using-Deep-Learning

---

This project classifies kidney CT scan images into four categories—**Normal, Cyst, Tumor, and Stone**—using deep learning models. The dataset is sourced from Kaggle and undergoes preprocessing, augmentation, and model evaluation.  

## 🔍 Dataset  
- **Source:** [Kaggle - CT Kidney Dataset](https://www.kaggle.com/datasets/nazmul0087/ct-kidney-dataset-normal-cyst-tumor-and-stone)  
- **Classes:** Normal, Cyst, Tumor, Stone  
- **Balancing:** Data augmentation applied to balance class distribution  

## 🛠️ Preprocessing  
- Missing values handled  
- Dataset split into **train (70%)**, **validation (15%)**, and **test (15%)**  
- Images resized to **64×64**  
- One-hot encoding applied to labels  

## 🏗️ Models Used  
1. **Artificial Neural Network (ANN)**  
2. **Convolutional Neural Network (CNN)**  
3. **ResNet50 (Pre-trained)**  
4. **VGG16 (Pre-trained)**  

## 🚀 Hyperparameter Tuning  
- **Keras Tuner (Hyperband Search)** optimized CNN architecture  
- Best model achieved **91.93% test accuracy**  

## 📊 Results  
| Model      | Test Accuracy |  
|------------|--------------|  
| ANN        | **91%**      |  
| CNN        | **92%**      |  
| ResNet50   | **89%**      |  
| VGG16      | **92%**      |  
| **Tuned CNN** | **91.93%** |  

## 📌 Usage  
### Install dependencies  
```bash
pip install -r requirements.txt
```  
### Train the Model  
```python
python train.py
```  
### Evaluate the Model  
```python
python evaluate.py
```  

## 📁 Saved Models  
- **ann_model.h5**  
- **cnn_model.h5**  
- **resnet50_model.h5**  
- **vgg16_model.h5**  
- **best_cnn_model.h5** (Tuned CNN)  

---
