# 🧠 Brain Tumor Detection Using CNN (Torchvision)

## 🚀 Overview
This project aims to automate the detection of brain tumors in CT scan images using a Convolutional Neural Network (CNN) built with PyTorch. The model classifies input brain scans as either **Tumor** or **Healthy**, helping reduce diagnostic time and error in medical imaging.

---

## 🎯 Purpose
Manual diagnosis of brain tumors from MRI/CT scans is time-consuming and prone to subjectivity. This project introduces an AI-powered pipeline that aids radiologists in detecting tumors with high confidence.

---

## 🧠 Model Architecture
- Custom **Convolutional Neural Network (CNN)** with:
  - 3 Conv2D blocks + MaxPooling
  - Batch Normalization & Dropout
  - Fully Connected Dense Layers
- Trained using `CrossEntropyLoss` and optimized with `Adam` and `ReduceLROnPlateau`.

---

## 📊 Results
- **Validation Accuracy**: ~97%
- **Dataset Size**: ~2,500 CT images
- **Confusion Matrix & Classification Report** show <2% false negatives (crucial for real-world deployment).

---

## 🛠 Libraries Used
- `PyTorch`, `torchvision`
- `numpy`, `matplotlib`, `seaborn`
- `splitfolders` for dataset management
- `sklearn` for evaluation metrics

---

## 🧪 How to Run

```bash
# Install dependencies
pip install -r requirements.txt

# Prepare the data (if needed)
python prepare_data.py

# Train the model
python train.py

# Evaluate
python evaluate.py
