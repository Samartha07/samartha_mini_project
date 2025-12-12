# 🚀 Deepfake Detection System using MobileNetV2

A lightweight AI-based system to detect whether an **image or video is REAL or FAKE**, built using **MobileNetV2**, **PyTorch**, **OpenCV**, and **Streamlit**.

---

## 📌 **Features**

* 🖼️ **Image Deepfake Detection**
* 🎥 **Video Deepfake Detection (Frame-based analysis)**
* 🧠 **MobileNetV2-based deep learning model**
* ⚡ **Fast & lightweight — runs on CPU**
* 🌐 **Streamlit GUI for easy interaction**
* 🔍 **Frame sampling + Majority voting for video classification**
* 📊 **Binary classification: REAL vs FAKE**

---

## 🧠 **Model Used**

* **MobileNetV2** pretrained on ImageNet
* Fine-tuned for deepfake binary classification
* Uses depthwise separable convolutions for efficient performance
* Ideal for real-time CPU inference

---

## 🛠️ **Tech Stack**

| Component                | Technology            |
| ------------------------ | --------------------- |
| Model                    | MobileNetV2 (PyTorch) |
| GUI                      | Streamlit             |
| Image & Video Processing | OpenCV, PIL           |
| Backend                  | Python                |
| Deployment               | Streamlit / Local Run |

---

## 📂 **Project Structure**

```
Deepfake_GUI/
│── app.py                     # Streamlit frontend
│── mobilenet_model.py         # Model architecture + loading
│── detect_image.py            # Image detection pipeline
│── detect_video.py            # Video detection pipeline
│── requirements.txt           # Dependencies
│── sample_inputs/             # Sample images/videos
│── saved_model/               # Trained MobileNetV2 weights (optional)
│── README.md                  # Project documentation
```

---

## 🔧 **Installation**

### 1️⃣ Clone the repository
git clone https://github.com/<your-username>/Deepfake-Detection.git
cd Deepfake-Detection

### 2️⃣ Install dependencies
pip install -r requirements.txt


### 3️⃣ Run the Streamlit App
streamlit run app.py


The browser will automatically open the GUI.

---

## 🧪 **How It Works**

### 🔹 Image Detection

1. User uploads an image
2. Image is resized to **224×224**
3. Preprocessed and passed into MobileNetV2
4. Model outputs REAL / FAKE

### 🔹 Video Detection

1. User uploads a video
2. Frames are extracted using OpenCV
3. Every Nth frame is passed to the model
4. Majority voting determines final verdict
5. Output displayed as REAL/FAKE

---

## 📊 **Output Examples**

✔ Real Image → *"REAL"*
❌ Deepfake Image → *"FAKE"*
🎥 Video → Final label based on majority frame predictions

---

## 🚀 **Future Improvements**

* Train exclusively on DFDC / FaceForensics++ datasets
* Add face detection (MTCNN / RetinaFace)
* Include attention-based models (EfficientNet, Vision Transformers)
* Provide probability/confidence scoring
* Add real-time webcam deepfake detection

---

## 🧑‍💻 **Author**

**Samartha (1AM23AI049),
Jignesh (1AM23AI044),
Tafazul(1AM23AI046)**
Deepfake Detection Project – Lightweight AI Prototype
Guided by: *Asst. Prof. C Subhashri (Dept. of AIML, AMCEC)*

