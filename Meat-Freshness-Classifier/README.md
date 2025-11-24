# 🥩 Meat Freshness Classifier Using Convolutional Neural Networks (CNN)

This project implements a deep learning-based image classifier that predicts the **freshness level of meat** using Convolutional Neural Networks (CNNs).  

The model categorizes images into:

- **Fresh**
- **Half-Fresh**
- **Spoiled**

This project is crucial in food safety — detecting spoilage early prevents contamination and supports quality control in the food supply chain.

---

# 📘 Dataset
- **Meat Freshness Image Dataset (Kaggle, 2022)**
- 2,226 labeled images across 3 classes
- Images resized to **128 × 128 pixels** for training   

---

# 🧱 CNN Architecture Overview

### 🌀 Convolutional Layers
- Three convolution blocks  
- Filters: **32 → 64 → 128**  
- Kernel: **3×3**, activation: **ReLU**  


### 🧊 Max Pooling Layers
- MaxPooling2D after every conv layer
- Pool size: **2×2**
- Reduces feature map while preserving important patterns  


### 🔁 Dropout & Fully Connected Layers
- Dropout: 0.2 and 0.25 after early conv layers  
- Dense(128, ReLU)  
- Dense(3, Softmax)  


### 🧩 Model Summary
- Flatten → Dense → Dropout → Dense → Softmax  

---

# 🛠 Implementation Details  

Includes:

- Data preprocessing  
- Label encoding  
- Loading + verifying training/test split  
- Data augmentation  
- CNN model creation  
- Training loop  

---

# 📈 Model Training

### Hyperparameters
- Optimizer: **Adam (learning rate = 0.0001)**  
- Batch size: **32**  
- Epochs tested: 10, 50, 100 → **50 chosen**  


### Overfitting Solutions
- Data augmentation (rotation, flip, zoom)  
- Early stopping (patience = 10)  


---

# 🧪 Evaluation Metrics

### ✔ Accuracy: **88.69%**  

### ✔ Precision, Recall, F1-score  
- Precision: 89.32%  
- Recall: 88.69%  
- F1-score: 88.80%  

---

# 🧠 Key Learnings

Through this project, I practiced:

- Building CNNs from scratch  
- Choosing correct kernel sizes (3×3) for feature extraction  
- Using pooling layers for dimensionality reduction  
- Applying data augmentation  
- Preventing overfitting using dropout & early stopping  
- Evaluating ML models using multiple metrics  
- Implementing a full workflow: preprocessing → training → evaluation → visualization  

This project strengthened my understanding of **computer vision**, **deep learning**, and **neural network architecture design**.

---

# 🎉 Final Notes
This CNN model demonstrates how AI can be used in real-world food safety applications—helping classify meat freshness accurately, with potential industrial impact.



