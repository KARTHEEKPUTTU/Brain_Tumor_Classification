# 🧠 Brain Tumor Classification with Explainable Deep Learning

## 📌 Overview
This project focuses on **classifying brain MRI images** into multiple tumor categories using **deep learning models** and presenting predictions through an **interactive Streamlit web application**.

In addition to classification, the system provides **visual explanations using saliency maps** and generates **human-readable medical explanations** using a Large Language Model (LLM).

---

## 🧠 Problem Statement
Accurate and interpretable brain tumor classification from MRI scans is critical for medical decision support.  
This project aims to:
- Classify MRI scans into tumor categories
- Compare transfer learning with a custom CNN
- Provide explainability to support trust in predictions

---

## 🗂️ Project Structure

```
Brain_Tumor_Classification/
│
├── *.ipynb # Data loading, EDA, training & evaluation
├── app.py # Streamlit web application
├── cnn_model.h5 # Custom CNN model
├── xception_model.weights.h5 # Transfer learning model weights
├── saliency_maps/ # Generated saliency visualizations
├── .env # API key configuration
└── README.md
```


---

## 📊 Dataset
- **Source:** Kaggle – Brain Tumor MRI Dataset
- **Classes:**
  - Glioma
  - Meningioma
  - Pituitary Tumor
  - No Tumor
- Dataset split into **training, validation, and testing** sets

---

## 🔍 Exploratory Data Analysis
- Class distribution analysis
- Visualization of MRI samples
- Train / validation / test balance checks

---

## 🤖 Modeling Approaches

### 1️⃣ Transfer Learning (Xception)
- Pre-trained on ImageNet
- Custom classification head
- Global max pooling
- Achieved strong generalization performance

### 2️⃣ Custom CNN
- Multiple convolutional layers
- Dropout & regularization
- Used as a baseline comparison model

---

## 📈 Model Evaluation
- Accuracy
- Precision
- Recall
- Confusion matrix
- Class-wise performance analysis
- Training vs validation metric visualization

---

## 🔎 Explainability with Saliency Maps
- Gradient-based saliency mapping
- Highlights regions influencing predictions
- Visual overlay on MRI scans
- Helps interpret model focus areas

---

## 🌐 Streamlit Web Application

### Features
- Upload MRI image
- Select model (Xception / CNN)
- Real-time tumor classification
- Confidence scores per class
- Saliency map visualization
- Interactive probability charts

---

## 🧠 LLM-Based Medical Explanation
- Uses a **Generative AI model**
- Generates concise medical-style explanations
- Explains:
  - Model prediction
  - Saliency-based reasoning
- Keeps explanations non-technical and human-readable

---

## 🚀 How to Run the Application

```bash
pip install -r requirements.txt
streamlit run app.py
```
Ensure API keys are configured in the .env file.

🧪 Skills Demonstrated
- Computer Vision
- Deep Learning (CNNs)
- Transfer Learning
- TensorFlow / Keras
- Explainable AI
- Streamlit deployment
- Saliency mapping
- Applied Generative AI

🔮 Future Enhancements
- Grad-CAM visualizations
-Cloud deployment
-Model optimization for inference
-Multi-modal clinical data integration

📌 Project Type
- Computer Vision
- Deep Learning
- Explainable AI
- Applied Machine Learning

👤 Author

**Kartheek Puttu**
