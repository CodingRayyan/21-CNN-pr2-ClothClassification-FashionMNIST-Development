![image](https://github.com/user-attachments/assets/1b573f7c-955d-4c72-a475-551dfac48837)

# 🧥 FashionMNIST Classification with TensorFlow

This repository contains a simple neural network model built using TensorFlow and Keras to classify images from the FashionMNIST dataset.

## 📂 Dataset
The FashionMNIST dataset is a collection of 28x28 grayscale images of 10 fashion categories, including T-shirts, trousers, and shoes. It is imported directly from TensorFlow datasets.

## 🔍 Data Analysis
- Inspected training and test set shapes
- Visualized sample images
- Checked class labels and distribution

## 🧹 Data Cleaning
- Normalized pixel values to range [0, 1]
- No missing values present
- Reshaping handled automatically using `Flatten` layer

## 🏗️ Model Training
- Used `Sequential` model with:
  - `Flatten` layer
  - One `Dense` hidden layer with ReLU
  - Output layer with 10 units (for 10 classes)
- Tuned:
  - Number of units in hidden layer
  - Learning rate using Keras Tuner (Hyperband)

## 🔮 Prediction
- Predictions generated using `model.predict()`
- Converted logits to class labels using `np.argmax()`

## 📊 Evaluation
- Evaluated model using:
  - Accuracy
  - Classification Report (Precision, Recall, F1-Score)

## 🛠️ Tools Used
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- scikit-learn
- Keras Tuner

## 📈 Output
- Classification report with detailed metrics
- Model summary
- Tuned hyperparameters for best performance

---

Feel free to fork the repo or raise an issue if you have suggestions or improvements!
