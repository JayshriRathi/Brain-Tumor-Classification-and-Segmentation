# 🧠 Brain Tumor Classification & Segmentation 

A complete deep learning–based medical imaging system for automatic brain tumor detection, classification, and segmentation from MRI scans.
The project integrates VGG16-based classification and U-Net-based segmentation with a Streamlit web application for real-time clinical-style analysis and reporting.


## 📌 Key Features

* 🧠 **Automatic Tumor Detection** with clear MRI scan interpretation
* 📊 **Tumor Classification** with confidence scores
* 🧩 **Tumor Segmentation** with precise area calculation
* 📦 **Bounding Box Detection** and visualization
* 📝 **Automated Clinical Notes** generated from scan findings
* 📄 **Comprehensive Medical Reports** with download options
* 👤 **Patient Information Management**
* 📈 **Quantitative Analysis** of tumor characteristics


## 🔍 Automated Scan Interpretation

* 🟢 **NORMAL SCAN:** No tumor detected
* 🔴 **ABNORMAL SCAN:** Tumor detected with tumor-type classification
* 📍 **Tumor Localization** and size estimation
* 📝 **Automatic clinical notes** generated based on predictions
* 🏥 **Professional report format** suitable for medical use


## 🧠 Models & Methodology

### 🔹 Classification Model

* **Architecture:** VGG16 (Transfer Learning)
* **Framework:** TensorFlow / Keras
* **Approach:**

  * Pretrained ImageNet weights
  * Fine-tuning of deeper convolutional layers
  * Softmax classifier for multi-class prediction

### 🔹 Segmentation Model

* **Architecture:** U-Net
* **Design:** Encoder–Decoder with skip connections
* **Loss Functions:** Dice Loss, Binary Cross-Entropy
* **Output:** Pixel-wise tumor segmentation mask


## 📂 Dataset Structure

```
DATASET/
│
├── Segmentation/
│   ├── Glioma/
│   ├── Meningioma/
│   └── Pituitary tumor/
│
└── classification/
    ├── Training/
    │   ├── glioma/
    │   ├── meningioma/
    │   ├── pituitary/
    │   └── notumor/
    │
    └── Testing/
        ├── glioma/
        ├── meningioma/
        ├── pituitary/
        └── notumor/
```


## 🖥️ Streamlit Web Application

The project includes an interactive Streamlit application that allows users to:

* Upload MRI brain scans
* Perform tumor classification and segmentation
* Visualize bounding boxes and segmentation masks
<img width="688" height="648" alt="image" src="https://github.com/user-attachments/assets/de28a4ad-f011-4e42-8072-8da8e716f03c" />

* Quantitative Analysis
<img width="433" height="153" alt="image" src="https://github.com/user-attachments/assets/85c42312-ddc7-4c58-b4e7-7ea92a5cbb57" />

* Generate automated clinical notes
* Download comprehensive medical reports
<img width="570" height="379" alt="image" src="https://github.com/user-attachments/assets/cc8f568e-f467-4e62-9eb3-a981333a55f2" />


  
## 📊 Results (Overview)

* **Classification:** High accuracy achieved using fine-tuned VGG16
<img width="388" height="207" alt="image" src="https://github.com/user-attachments/assets/4eff5bd9-bc5a-4d6a-9e2f-2916dec9c24a" />
<img width="563" height="215" alt="image" src="https://github.com/user-attachments/assets/388edacf-e538-4787-ae9c-d15fd2178e87" />
<img width="490" height="433" alt="image" src="https://github.com/user-attachments/assets/6c7c49e6-8a34-4897-a832-e53b43f2c6ff" />

* **Segmentation:** Accurate tumor boundary detection using U-Net
<img width="300" height="319" alt="image" src="https://github.com/user-attachments/assets/145f811d-0204-488c-8d91-85b056c8f720" />
<img width="657" height="254" alt="image" src="https://github.com/user-attachments/assets/655b272b-440e-4816-92fb-e818f492bb94" />
<img width="434" height="337" alt="image" src="https://github.com/user-attachments/assets/a494699a-032b-4e4f-a647-f8e01ac464ba" />

* **Visualization:** Clear and interpretable outputs suitable for demonstrations
<img width="543" height="303" alt="image" src="https://github.com/user-attachments/assets/34cb298c-e440-4cea-93c2-1cd7679850c7" />


## 🛠️ Technologies Used

* Python
* TensorFlow / Keras
* OpenCV
* NumPy, Pandas
* Matplotlib
* Streamlit


## 🔮 Future Enhancements

* Grad-CAM–based model explainability
* Attention U-Net for improved segmentation
* Cloud deployment (AWS / Hugging Face Spaces)


