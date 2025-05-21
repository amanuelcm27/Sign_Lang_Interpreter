# ASL Hand Sign Recognition using Deep Learning

This project is a deep learning-based system that recognizes American Sign Language (ASL) hand signs from images and real-time webcam input. It uses a supervised learning approach with a convolutional neural network (CNN) model built and trained using TensorFlow/Keras.

## 📌 Features

- Trained on labeled ASL images (A–Z, space, nothing, delete)
- Preprocessed images to 64x64 resolution for training
- Used `model.fit()` with validation split to monitor training
- Added real-time hand sign detection via webcam
- Predicted hand sign is printed live on screen
- Saved trained model in modern `.keras` format for reuse

## 🧠 Model Details

- **Architecture:** Deep Neural Network with multiple Conv2D + MaxPooling2D layers
- **Batch Size:** 32
- **Epochs:** 10+
- **Loss:** Categorical crossentropy (multi-class classification)
- **Optimizer:** Adam

## 🧪 Testing

- Tested with labeled `.jpg` images placed in a test directory
- Converted raw model output to readable sign names (e.g., 0 → A, 27 → "nothing")
- Achieved good accuracy in identifying clear ASL signs

## 🎥 Real-Time Application

- Integrated OpenCV to capture webcam feed
- Processed frames in real time to predict ASL hand signs
- Displayed predicted sign on terminal/output

## 💾 Model Persistence

- Trained model is saved as `asl_model.keras`
- Can be reloaded for future use without retraining

## 📚 Applications

- Assistive technology for the hearing/speech impaired
- Educational tools for learning sign language
- Gesture recognition systems
- Potential integration into mobile or embedded platforms

---

## ✅ Requirements

- Python 3.x
- TensorFlow / Keras
- OpenCV
- NumPy
- A labeled ASL image dataset

## 🚀 How to Run

1.  load the saved model (asl_model.keras)
2. Run the real-time prediction script with your webcam
3. Show ASL signs to the camera and see the predictions live!

