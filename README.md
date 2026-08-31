# 🧠 Brain Tumor Detection

An AI-powered medical image classification system that detects brain tumors from **MRI scans** using a **Convolutional Neural Network (CNN)**. The project combines a **React** frontend, **FastAPI** backend, and **TensorFlow/Keras** model to deliver real-time predictions through a simple and intuitive web interface.

---

## 📋 Project Overview

Brain Tumor Detection is a full-stack deep learning application designed to classify MRI brain images as **Tumor** or **No Tumor**. Users upload an MRI scan through the React application, the FastAPI server preprocesses the image, performs inference using a trained CNN model (`my_model.h5`), and returns the prediction instantly.

---

## ✨ Key Features

### 1. CNN-Based Tumor Detection

Classifies MRI brain scans using a trained Convolutional Neural Network built with TensorFlow and Keras.

### 2. Real-Time Prediction API

FastAPI provides a lightweight REST API for image preprocessing and model inference.

### 3. Interactive React Interface

Users can upload MRI images and receive prediction results with a clean, responsive UI.

### 4. End-to-End AI Pipeline

Complete workflow from image upload → preprocessing → CNN inference → prediction response.

### 5. Model Training Included

Includes the Jupyter Notebook used for dataset preprocessing, training, and model experimentation.

---

## 🛠️ Tech Stack

| **Layer**             | **Technologies**          |
| --------------------- | ------------------------- |
| **Frontend**          | React, JavaScript, CSS3   |
| **Backend**           | FastAPI, Python           |
| **Deep Learning**     | TensorFlow, Keras, CNN    |
| **Image Processing**  | Pillow (PIL), NumPy       |
| **API Communication** | REST API                  |
| **Model Format**      | HDF5 (`my_model.h5`)      |
| **Development Tools** | Jupyter Notebook, Uvicorn |

---

## 🚀 Setup & Run

### Clone the Repository

```bash
git clone https://github.com/MachaVivek/Brain_Tumor_Detection.git
cd Brain_Tumor_Detection
```

### Backend Setup

```bash
cd fastapi_backend

pip install fastapi uvicorn tensorflow pillow numpy

uvicorn main:app --reload
```

### Frontend Setup

```bash
cd react_frontend

npm install
npm start
```

### Application URLs

```text
Frontend : http://localhost:3000
Backend  : http://localhost:8000
```

---

## 📁 Project Structure

```text
Brain_Tumor_Detection/
├── brain-tumor-detection-cnn.ipynb
├── fastapi_backend/
│   ├── main.py
│   ├── my_model.h5
│   └── about/
├── react_frontend/
│   ├── src/
│   ├── public/
│   └── package.json
└── README.md
```

---

## 🔄 Prediction Workflow

1. Upload an MRI brain image from the React application.
2. FastAPI receives and preprocesses the image.
3. The trained CNN model performs inference.
4. The prediction is returned as **Tumor** or **No Tumor**.
5. The result is displayed instantly on the frontend.

---

## 🌐 API Endpoint

| **Method** | **Endpoint** | **Purpose**                             |
| ---------- | ------------ | --------------------------------------- |
| POST       | `/predict`   | Upload MRI image and receive prediction |

---

## 🔬 Model Information

* **Architecture:** Convolutional Neural Network (CNN)
* **Framework:** TensorFlow / Keras
* **Input:** Brain MRI Image
* **Output:** Tumor / No Tumor
* **Model File:** `my_model.h5`

---

## 🚧 Future Enhancements

* Multi-class brain tumor classification
* Confidence score for predictions
* Grad-CAM heatmap visualization
* Patient report generation
* Model performance dashboard

---

## 📄 License

This project is developed for educational and portfolio purposes.

---

## 👨‍💻 Author

**Vivek Macha**

GitHub: https://github.com/MachaVivek
