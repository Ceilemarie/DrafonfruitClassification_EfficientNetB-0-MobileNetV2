# DrafonfruitClassification_EfficientNetB-0-MobileNetV2
🐉 Dragon Fruit Quality Classification using Deep Learning 
This repository contains a deep learning project designed to automate the quality assessment of Dragon Fruit. 
By utilizing state-of-the-art Convolutional Neural Networks (CNNs)

the system classifies images into two categories: Healthy and Rotten.

📌 Project Overview
The goal of this project is to provide a reliable tool for farmers and distributors to identify spoiled dragon fruit, minimizing post-harvest losses. 
The project compares two lightweight but powerful architectures—EfficientNet-B0 and MobileNetV2—to find the best balance between predictive accuracy and computational efficiency.

📊 Dataset Description
<style type="text/css">
.tg  {border-collapse:collapse;border-color:#9ABAD9;border-spacing:0;}
.tg td{background-color:#EBF5FF;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#444;
  font-family:Arial, sans-serif;font-size:14px;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{background-color:#409cff;border-color:#9ABAD9;border-style:solid;border-width:1px;color:#fff;
  font-family:Arial, sans-serif;font-size:14px;font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-c3ow{border-color:inherit;text-align:center;vertical-align:top}
.tg .tg-fymr{border-color:inherit;font-weight:bold;text-align:left;vertical-align:top}
.tg .tg-7btt{border-color:inherit;font-weight:bold;text-align:center;vertical-align:top}
</style>
<table class="tg"><thead>
  <tr>
    <th class="tg-fymr">Source</th>
    <th class="tg-fymr">Healthy Images</th>
    <th class="tg-fymr">Rotten Images</th>
    <th class="tg-fymr">Sub-total</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-fymr">Local Data (Field Samples)</td>
    <td class="tg-c3ow">520</td>
    <td class="tg-c3ow">444</td>
    <td class="tg-c3ow">964</td>
  </tr>
  <tr>
    <td class="tg-fymr">Internet Data (Kaggle/Web)</td>
    <td class="tg-c3ow">1,219</td>
    <td class="tg-c3ow">1,154</td>
    <td class="tg-c3ow">2,373</td>
  </tr>
  <tr>
    <td class="tg-fymr">Total</td>
    <td class="tg-7btt">1,739</td>
    <td class="tg-7btt">1,598</td>
    <td class="tg-7btt">3,337</td>
  </tr>
</tbody>
</table>

Preprocessing Steps:
Standardization: All images were resized to 224x224 pixels.
Augmentation: Applied offline techniques (Horizontal/Vertical Flipping and 180° Rotation) to the minority class to achieve a balanced 52:48 distribution.
Normalization: Pixel values were rescaled using model-specific preprocessing functions.

🏗️ Model Architectures
EfficientNet-B0: Used for its superior feature extraction capabilities through compound scaling.
MobileNetV2: Tested for its efficiency on mobile and edge devices.
Transfer Learning: Both models were initialized with ImageNet weights.
Fine-tuning: Custom classifier heads were added with Dropout (0.3) and Sigmoid activation.

🛠️ Tech Stack
Language: Python
Frameworks: TensorFlow / Keras
Libraries: OpenCV, PIL, Pandas, Matplotlib, Scikit-learn
Platform: Google Colab / Google Drive for Cloud Training

🚀 How to Use
Clone the repository: git clone [https://github.com/YourUsername/DragonFruit-Classification.git](https://github.com/Ceilemarie/DrafonfruitClassification_EfficientNetB-0-MobileNetV2/new/main?readme=1)
Install dependencies: pip install -r requirements.txt
Run the notebook or script to train/evaluate the models.
