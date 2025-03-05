# Scream Detection System with GUI

## 📌 Overview
The **Scream Detection System** is an AI-powered application designed to detect screams in real time using machine learning. Upon detecting a scream, the system sends an emergency alert with a live location to a predefined WhatsApp contact. The system features a **GUI-based interface** built with Tkinter for user interaction.

## 🚀 Features
- 🎤 **Real-time scream detection** using a pre-trained deep learning model.
- 📍 **Live GPS location tracking** using `geocoder`.
- 📩 **Automatic emergency alert via WhatsApp** using `pywhatkit`.
- 🖥️ **User-friendly GUI** with buttons to start and stop detection.

## 🛠️ Installation
### 🔹 Prerequisites
Ensure you have Python installed (version 3.8+ recommended). You also need the following dependencies:

Download the dataset
https://www.kaggle.com/datasets/whats2000/human-screaming-detection-dataset

```sh
pip install sounddevice numpy librosa tensorflow pywhatkit geocoder tkinter
```

### 🔹 Clone the Repository
```sh
git clone https://github.com/mounika-muthyamaina/scream-detection-and-crime-prevention.git
cd scream-detection-and-crime-prevention
```

## 🎯 How to Use
1. **Run the script**
   ```sh
   python scream_detection_gui.py
   ```
2. Click on the **"Start Detection"** button to begin listening for screams.
3. If a scream is detected, an emergency message with a **live location** will be sent via WhatsApp.
4. Click **"Stop Detection"** to halt the process.

## 🏗️ Project Structure
```
scream-detection/
│── backend/
│   │── train_model.py  # Train and save the model
│   │── predict.py      # Load model and predict scream
│   │── features.csv    # Extracted dataset features
│   │── scream_detector_model.h5  # Pre-trained model
│── gui/
│   │── real_time_detection.py  # GUI application
│── dataset/
│   │── (Raw audio files for training)
```

## 🔍 Model Details
- The model is trained using **MFCC features** extracted from audio recordings.
- A deep learning architecture is used to classify sounds as **screams or non-screams**.

## 📌 Future Enhancements
- 🔹 **Integration with security systems** (CCTV, IoT devices, etc.).
- 🔹 **Improved accuracy** using advanced audio classification models.



