# 🦷 OralAI Check – Oral Disease Classification Web App

OralAI Check is a deep learning–based web application developed as part of my Final Year Project:

**“Deep Learning for Oral Disease Classification & Teeth Segmentation.”**

The system performs multi-class oral disease classification using a trained CNN model and allows users to upload intraoral images for AI-powered screening.

⚠️ Important: The classifier is limited to 6 predefined oral disease categories only.

---

## 🌐 Website Overview

OralAI Check provides a simple 3-step workflow:

1. Upload intraoral image  
2. Analyze using trained deep learning model  
3. View result with confidence score and recommendation  

The system is designed for educational and research purposes only and does not replace professional dental diagnosis.

---

## 📌 Supported Disease Categories (6 Classes Only)

The model can classify images into the following categories:

- Calculus  
- Caries  
- Gingivitis  
- Ulcer  
- Hypodontia  
- Tooth Discoloration  

The system will always output one of these six classes only.

---

## 🚀 How to Use the Website

### Step 1 – Upload Image

- Drag and drop your intraoral image into the upload box  
  OR  
- Click **Select Image** to browse from your device  

Recommended:
- Clear intraoral photo  
- Good lighting  
- Focused on teeth and gums  
- No heavy blur or obstruction  

---

### Step 2 – Analyze Image

- Click **Analyze Image**
- The image is sent to the deployed model API
- The system performs preprocessing and inference

---

### Step 3 – View Results

The system will display:

- Predicted Disease Category  
- AI Confidence Level (%)  
- Recommendation Message  

Example output:

Analysis Result: Calculus  
AI Confidence Level: 59%  
Recommendation: Possible Calculus. Visit a dentist for visual examination.

You may click **Analyze Again** to test another image.

---

## 🧠 Model Information

The classification model was developed and trained as part of my thesis research.

- Architecture: ResNet50V2 + Channel Attention
- Training Strategy: Transfer Learning (ImageNet-pretrained backbone)
- Enhancements: Data Augmentation + Channel Attention Mechanism
- Task: 6-class Oral Disease Classification
- Best Test Accuracy: 93.15%

### Why ResNet50V2 + Channel Attention?

ResNet50V2 was selected for its strong feature extraction capability and stable training behavior in deep architectures.

Channel Attention was integrated to:
- Reweight important feature channels
- Enhance discriminative oral disease features
- Suppress irrelevant background information

This combination produced the best overall performance in the ablation study conducted in the thesis.

---

## ⚠️ Limitations

- The system only recognizes 6 specific oral disease categories  
- It does not detect multiple diseases in a single image  
- It does not replace clinical examination  
- Performance depends on image quality  
- Not suitable for radiographs or non-intraoral images  

---

## 🔒 Disclaimer

This tool is developed for educational and research purposes only.

It does not provide medical diagnosis and should not be used as a substitute for professional dental advice. Always consult a licensed dentist for proper examination and treatment.

---

## 💻 Tech Stack

Frontend:
- HTML
- CSS
- JavaScript

Backend:
- Python
- TensorFlow / Keras
- Google Cloud REST API Deployment

---

## 👩‍💻 Author

Keisha Althea Halim's Final Year Project  
Bachelor of Engineering (Honours) in Data Science  
Xiamen University Malaysia
