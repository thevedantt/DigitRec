
# 🧠 Handwritten Digit Recognition using MNIST

This project implements a deep learning model to recognize handwritten digits using the **MNIST dataset** and custom digit images as input. The model is trained using **TensorFlow/Keras** and tested against a set of user-provided digit images (named `digit1.png`, `digit2.png`, ...).

---

### ✅ Features
- Trained on the MNIST dataset of 60,000 handwritten digits.
- Uses a deep neural network with:
  - Dense layers
  - Dropout for regularization
- Accepts external images from a folder (`/content/digits/`) and predicts their labels.
- Automatically loops through files named `digit1.png`, `digit2.png`, etc.

---

### 🧪 Model Performance

- **Training Accuracy**: ~99%  
- **Test Accuracy** on MNIST: **~98.5%**  
- **Custom Image Results**:  
  - Total digits tested: 10  
  - Correct predictions: 7  
  - Incorrect predictions: 3  

> ℹ️ Custom digit accuracy is currently **70%** — this gap is due to differences between MNIST-style images and user-supplied images.

---

### 🔧 Future Improvements
- Implement a **Convolutional Neural Network (CNN)** for better performance on real-world digit images.
- Apply **image preprocessing techniques** like thresholding, centering, and contour detection.
- Add support for **image augmentation** during training for better generalization.
- Handle skewed, rotated, or noisy digits more robustly.

---

### 📁 How to Use
1. Train the model (or use the provided `.keras` model).
2. Place images as:
   ```
   /content/digits/digit1.png
   /content/digits/digit2.png
   ...
   ```
3. Run the script – the model will automatically read and predict from all available files.
