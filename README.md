# Advanced Facial Recognition & Spoof Detection System

An advanced AI-powered system that combines **facial recognition** with **spoof detection and liveness verification** to accurately identify users and prevent spoofing attacks (e.g., photos, masks, or video replays). This project is designed with a focus on **deep learning**, **computer vision**, **model optimization**, and **deployment on edge devices**.

---

## Project Overview

This system goes beyond traditional facial recognition by integrating **spoof detection**, enabling it to distinguish between real human faces and presentation attacks. It leverages powerful **Convolutional Neural Networks (CNNs)** and **temporal analysis techniques** to ensure the system is both accurate and robust in real-world conditions.

We use the **CelebA** dataset for facial identity learning and the **Spoof in the Wild** dataset to train the model to detect spoofed inputs. Our end goal is to **optimize the model for edge deployment** using **ONNX**, and expose it as a real-time service via **FastAPI**.

---

## Goals & Key Features

### Goals
- Perform **accurate facial recognition** using deep CNNs
- Implement **spoof detection** to counter facial presentation attacks
- Include **liveness detection** using temporal and texture-based features
- Optimize models for **low-latency inference on edge devices**
- Build and deploy a **real-time API** using FastAPI

### Key Features
- 🔍 Face identity recognition (using CelebA dataset)
- 🛡️ Anti-spoofing detection (static and temporal-based)
- 👁️ Passive liveness detection (blink/motion detection)
- ⚙️ Model export to **ONNX** for cross-platform inference
- 🚀 Real-time inference via **FastAPI REST API**
- 💡 Clean, modular PyTorch code and reusable training/eval pipelines

---

## 🧠 Technologies & Tools Used

| Category            | Tools & Frameworks                          |
|---------------------|---------------------------------------------|
| **Languages**        | Python                                      |
| **Deep Learning**    | PyTorch, TorchVision                        |
| **Computer Vision**  | OpenCV, MediaPipe, Dlib (optional)          |
| **Datasets**         | CelebA, Spoof in the Wild                   |
| **Model Export**     | ONNX, ONNX Runtime                          |
| **Web API**          | FastAPI, Uvicorn                            |
| **Deployment**       | Docker (optional), Raspberry Pi / Jetson   |
| **Others**           | Matplotlib, Scikit-learn, NumPy             |

---

## 🧪 Datasets

### 📁 CelebA Dataset
- Large-scale face attributes dataset with over 200k celebrity images
- Used for training the facial recognition model
- Includes identity, facial landmark, and attribute annotations

### 📁 Spoof in the Wild (SiW) Dataset
- Real-world spoof detection dataset with diverse spoof attack types
- Used to train the model to distinguish real vs fake faces

---

### 2. Spoof Detection Module
- Binary classification (real vs spoofed)
- Optional temporal modeling with CNN-LSTM or 3D CNN
