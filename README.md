# Pancreatic Cancer Segmentation using U-Net (CT Imaging)

Deep learning-based segmentation of pancreatic regions from CT scan images for improved early detection of pancreatic cancer.

---

##  Domain
**Deep Learning in Medical Imaging (AI in Healthcare)**

---

##  Problem Statement
Pancreatic cancer is difficult to detect early due to the complex structure and low contrast of the pancreas in CT images. Accurate segmentation of the pancreas is a critical step for diagnosis and treatment planning. This project focuses on automating pancreas segmentation using deep learning.

---

##  Model Architecture
This project uses a **U-Net based convolutional neural network**, designed for biomedical image segmentation.

- Encoder-decoder structure  
- Skip connections for spatial feature preservation  
- Pixel-wise prediction for segmentation masks  

---

##  Project Structure
data
/models
/notebooks
/utils
/results

---

## Dataset
- Dataset: *(Add your dataset name here — e.g., Medical Segmentation Decathlon / Kaggle dataset)*  
- Modality: CT Scan Images  
- Input size: *(e.g., 128x128 / 256x256)*  
- Number of samples: *(add if known)*  

---
## Tech Stack
- Python  
- TensorFlow / PyTorch *(whichever you used)*  
- OpenCV  
- NumPy, Matplotlib

---

##  Methodology

### 1. Data Preprocessing
- Image resizing  
- Normalization  
- *(Optional: Data augmentation if you used it — rotation, flipping, etc.)*

### 2. Model Training
- Architecture: U-Net  
- Loss Function: *(Dice Loss / BCE + Dice — fill this)*  
- Optimizer: *(Adam / SGD)*  
- Epochs: *(add number)*  

### 3. Evaluation Metrics
- Dice Coefficient
- Precision
- Accuracy 
- Loss curves  

---

##  Pipeline
- CT Scan → Preprocessing → U-Net Model → Segmentation Mask → Evaluation
  
---

##  Results
23/23 ━━━━━━━━━━━━━━━━━━━━ 35s 1s/step
--- Dual-Head Performance ---
1. Segmentation Head (Spatial Dice): 0.4502
2. Classification Head (Detection Dice): 0.4824

--- Detailed Clinical Breakdown ---
              precision    recall  f1-score   support

     Healthy       0.54      0.77      0.63       350
       Tumor       0.64      0.39      0.48       371

    accuracy                           0.57       721
   macro avg       0.59      0.58      0.56       721
weighted avg       0.59      0.57      0.56       721

---

##  Sample Outputs
<img width="1180" height="1197" alt="image" src="https://github.com/user-attachments/assets/5a000cbd-834b-4187-aa6c-747cc9c9c4dd" />
<img width="1218" height="407" alt="image" src="https://github.com/user-attachments/assets/325c88d5-4bd8-430e-8fd9-5f25cb4faf6d" />
---
##  Future Work
- Improve dice score and segmentation accuracy using Attention U-Net / UNet++  
- Integrate biomarker-based clinical data with imaging  
- Hyperparameter tuning for better generalization  
- Extend model for tumor detection and classification  

---

##  Author
Arpita Padekar  
B.Tech Bioengineering  

---

