# 👁️‍🗨️ Face Recognition and Detection System

A simple Python project that uses OpenCV to detect faces in both static images and real-time webcam video. It utilizes Haar Cascade Classifiers for face detection and is perfect for beginners exploring computer vision and face detection basics.

---

## 📖 Overview

This project performs two main tasks:

1. **Face Detection in Static Images**  
   Detects and highlights faces in a user-specified image.

2. **Real-Time Face Detection via Webcam**  
   Continuously detects faces using the webcam feed and highlights them in real-time.

Both features use OpenCV’s pre-trained `haarcascade_frontalface_default.xml` classifier, making the system lightweight and efficient for face detection.

---

## ✨ Features

- 📸 Detects faces in uploaded images  
- 🎥 Detects faces live via webcam feed  
- 🧠 Utilizes Haar Cascade — a classical computer vision approach  
- 🖼️ Draws bounding boxes around detected faces  
- 🧪 Beginner-friendly and easy to extend

---

## 🛠️ Technologies Used

- **Language**: Python 3.x  
- **Library**: OpenCV (`cv2`)  
- **Model**: Haar Cascade Classifier  
- **Tools**:
  - Webcam via `cv2.VideoCapture`
  - Image visualization via `cv2.imshow`

---

## 🚀 Getting Started

### 📦 Prerequisites

Install OpenCV with:

```bash
pip install opencv-python
```

### 📁 Project Structure

```
face_detection_project/
│
├── face_detection.py
├── model/
│   └── haarcascade_frontalface_default.xml
└── your_image.jpg
```

Make sure to download the Haar cascade XML file from:  
🔗 [haarcascade_frontalface_default.xml](https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml)

Place it in a `model/` folder inside your project directory.

---

### ▶️ Running the Project

1. Open `face_detection.py`
2. Replace this line:

```python
detect_faces_image(r"image_path")
```

with:

```python
detect_faces_image(r"your_image.jpg")
```

3. Then run the script:

```bash
python face_detection.py
```

- It will first show face detection on the image you provided.
- After you close the image window, the webcam feed will start for real-time detection.
- Press **`q`** to quit the webcam view.

---

## 📸 Example Output

**Image Face Detection**

🟩 Rectangles will be drawn around all detected faces in the image.

**Webcam Live Detection**

👁️ Real-time rectangles appear on all detected faces until the user quits the session.

---

## 🔧 Future Improvements

- Add GUI with Tkinter or PyQt
- Integrate face recognition (e.g., LBPH, FaceNet)
- Save and recognize known faces
- Add video file support
- Log or alert unknown faces

---
