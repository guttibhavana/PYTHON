# 😊 Real-Time Face Detection Using Python & OpenCV

A real-time face detection application built with Python and OpenCV. The program captures live video from the webcam, detects human faces using the Haar Cascade Classifier, and draws bounding boxes around detected faces.

---

## 📌 Features

- Detects faces in real time using the webcam.
- Uses OpenCV's pre-trained Haar Cascade Classifier.
- Draws rectangles around detected faces.
- Displays a "Face Detector" label above each detected face.
- Press **Q** to quit the application.

---

## 🛠️ Technologies Used

- Python 3
- OpenCV (`cv2`)
- Haar Cascade Classifier

---

## 💻 Source Code

```python
import cv2

# Haar Cascade - Pre-trained face detection model
face_cascade = cv2.CascadeClassifier(
    cv2.data.haarcascades + "haarcascade_frontalface_default.xml"
)

camera = cv2.VideoCapture(0)

if not camera.isOpened():
    print("Error: Could not open camera.")
    exit()

while True:
    success, frame = camera.read()

    if not success:
        print("Failed to capture frame.")
        break

    gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

    faces = face_cascade.detectMultiScale(
        gray,
        scaleFactor=1.1,
        minNeighbors=5,
        minSize=(90, 90)
    )

    for (x, y, w, h) in faces:
        cv2.rectangle(
            frame,
            (x, y),
            (x + w, y + h),
            (0, 255, 0),
            2
        )

        cv2.putText(
            frame,
            "Face Detector",
            (x, y - 10),
            cv2.FONT_HERSHEY_COMPLEX,
            0.7,
            (0, 255, 0),
            2
        )

    cv2.imshow("Face Detection Using Python", frame)

    if cv2.waitKey(1) & 0xFF == ord("q"):
        break

camera.release()
cv2.destroyAllWindows()
```

---

## 📸 Sample Output

- The webcam opens and starts capturing live video.
- Faces are detected automatically.
- A **green rectangle** is drawn around each detected face.
- The label **"Face Detector"** appears above every detected face.
- Press **Q** to close the application.

---

## 🧠 How It Works

1. Loads OpenCV's pre-trained Haar Cascade face detection model.
2. Opens the system's default webcam.
3. Captures video frames continuously.
4. Converts each frame to grayscale for efficient processing.
5. Detects faces using the Haar Cascade classifier.
6. Draws a green rectangle and label around each detected face.
7. Displays the processed video until the user presses **Q**.

---

## 📚 Concepts Used

- Computer Vision
- OpenCV
- Haar Cascade Classifier
- Webcam Video Capture
- Image Processing
- Face Detection
- Loops and Conditional Statements

---

## 📦 Required Libraries

Install OpenCV before running the project:

```bash
pip install opencv-python
```
