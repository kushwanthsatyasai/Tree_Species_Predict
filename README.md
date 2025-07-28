# 🌳 Tree Species Prediction using CNN

This project focuses on classifying different species of trees using deep learning, specifically a Convolutional Neural Network (CNN) implemented in Python using TensorFlow and Keras.

> 📂 Main File: [`tree_CNN.ipynb`](tree_CNN%20(1).ipynb)

---

## 🧠 Objective

The primary goal is to predict tree species based on image inputs. This project showcases a simple yet effective CNN architecture to distinguish between classes using image data.

---

## 📁 Dataset

The dataset includes images of various tree species. Images are typically preprocessed to a uniform size before being passed to the model.

- Image format: `.jpg`, `.png`
- Classes: e.g., **Neem, Mango, Peepal, Banyan**, etc.
- You can customize the dataset by updating the image folders and labels.

> **Note**: Due to file size limitations, the dataset and trained model (`Week 2_Models.zip`) are stored in a separate branch or external storage. You may request or clone the `large-files` branch for model assets.

---

## 🏗️ Model Architecture

The CNN used includes:

- 2D Convolution Layers
- MaxPooling Layers
- Flatten + Dense Layers
- Softmax output for multi-class classification

### Model files

There are three models which are downloaded with their weights and the zip file is uploaded in drive check it here:
https://drive.google.com/file/d/12d20LX4-eZ5TpfTAuoRutl5ailkTKvtw/view?usp=drive_link

### 🔧 Sample Layers:
```python
model = Sequential()
model.add(Conv2D(32, (3, 3), activation='relu', input_shape=(64, 64, 3)))
model.add(MaxPooling2D(pool_size=(2, 2)))
...
model.add(Dense(units=5, activation='softmax'))

