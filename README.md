# Dragon Fruit Classification (EfficientNetB-0 & MobileNetV2)

## 🐉 Dragon Fruit Quality Classification using Deep Learning 
This repository contains a deep learning project designed to automate the quality assessment of Dragon Fruit by utilizing state-of-the-art **Convolutional Neural Networks (CNNs)**. The system classifies images into dalawang categories: **Healthy** and **Rotten**.

---

### 📌 Project Overview
The goal of this project is to provide a reliable tool for farmers and distributors to identify spoiled dragon fruit, minimizing post-harvest losses. The project compares two lightweight but powerful architectures—**EfficientNet-B0** and **MobileNetV2**—to find the best balance between predictive accuracy and computational efficiency.

---

### 📊 Dataset Description

<div align="center">

| Source | Healthy Images | Rotten Images | Sub-total |
| :--- | :---: | :---: | :---: |
| **Local Data (Field Samples)** | 520 | 444 | **964** |
| **Internet Data (Kaggle/Web)** | 1,219 | 1,154 | **2,373** |
| **Total** | **1,739** | **1,598** | **3,337** |

</div>

#### **Preprocessing Steps:**
* **Standardization:** All images were resized to **300x300 pixels**.
* **Augmentation:** Applied offline techniques (Horizontal/Vertical Flipping and 180° Rotation) to the minority class to achieve a balanced **52:48 distribution**.
* **Normalization:** Pixel values were rescaled using model-specific preprocessing functions.

---

### 🏗️ Model Architectures
* **EfficientNet-B0:** Used for its superior feature extraction capabilities through compound scaling.
* **MobileNetV2:** Tested for its efficiency on mobile and edge devices.
* **Transfer Learning:** Both models were initialized with **ImageNet** weights.
* **Fine-tuning:** Custom classifier heads were added with **Dropout (0.3)** and **Sigmoid** activation.

---

### 🛠️ Tech Stack
* **Language:** ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
* **Frameworks:** ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)
* **Libraries:** OpenCV, PIL, Pandas, Matplotlib, Scikit-learn
* **Platform:** Google Colab / Google Drive for Cloud Training

---

### 🚀 How to Use
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Ceilemarie/DrafonfruitClassification_EfficientNetB-0-MobileNetV2.git](https://github.com/Ceilemarie/DrafonfruitClassification_EfficientNetB-0-MobileNetV2.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
3.  **Run the notebook:**
    Open the `.ipynb` file in Google Colab or Jupyter Notebook to train/evaluate the models.
