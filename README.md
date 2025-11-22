# 🎭 Real-Time Facial Emotion Detection (Desktop-Based App)

A Python desktop application that performs real-time facial emotion detection using deep learning. The system captures video from a webcam, detects faces with OpenCV, and classifies emotions using a CNN model trained on facial expression datasets such as FER-2013.

---

## 🚀 Project Overview
This project aims to build a fast, customizable, and offline emotion detection system suitable for research, personal applications, and real-time monitoring. Cloud APIs are avoided to ensure privacy, local control, and no external dependencies.

Key emotions detected:
- Happy
- Sad
- Angry
- Neutral  
*(More emotions can be added depending on dataset.)*

---

## 🧠 Features
- Real-time webcam-based face detection  
- CNN-based emotion classification  
- Local-only processing for improved privacy  
- Custom model training from datasets  
- Desktop-based usage (no cloud required)  
- Expandable for more emotion categories  

---

## 📦 Tech Stack
- **Python**
- **TensorFlow / Keras** (CNN model)
- **OpenCV** (face detection + real-time frame processing)
- **NumPy / Pandas** (data handling)
- **FER-2013 / CK+** dataset support

---

## 🔍 Methodology

### 1. **Dataset Preparation**
Datasets such as FER-2013 and CK+ were used for training. Images were preprocessed (grayscale, resizing, normalization) for consistent model input.  
*(Dataset sources listed in proposal :contentReference[oaicite:2]{index=2})*
# Emotion_Detection_CNN

Data Set Link - https://www.kaggle.com/jonathanoheix/face-expression-recognition-dataset

### 2. **Model Development**
A Convolutional Neural Network (CNN) was designed using:
- Convolution layers  
- Pooling layers  
- Dense fully-connected layers  
- Softmax for emotion classification  

The model learns facial patterns associated with each emotion.

### 3. **Model Training**
- Trained on prepared emotion-labeled images  
- Evaluated using accuracy, precision, recall  
- Model saved for real-time inference  

### 4. **Real-Time Integration**
OpenCV handles:
- Webcam capture  
- Face detection (Haar Cascade / DNN)
- Frame-by-frame model prediction

The application displays:
- Detected face  
- Predicted emotion label  

### 5. **Desktop Implementation**
A Python script (`main.py`) integrates:
- Trained CNN model  
- OpenCV capture  
- On-screen emotion display  

---

## 📂 Folder Structure (Recommended)

