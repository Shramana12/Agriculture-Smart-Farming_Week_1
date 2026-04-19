# 🌿 Crop Disease Detection using Deep Learning

🚧 **Project Status**
Ongoing Internship Project – Week 1 Completed

---

## 🎯 Objective

The goal of this project is to build a deep learning model using Computer Vision to detect plant diseases from leaf images. This helps farmers identify diseases early, take quick action, reduce crop loss, and minimize unnecessary pesticide use.

---

## 📂 Dataset

**Dataset Name:** PlantVillage Dataset

**Source:** Kaggle ([PlantVillage Dataset](https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset))

**Dataset link:**   [(PlantVillage_Dataset)](https://drive.google.com/file/d/1bl92iuLfYAmq6w9hGREkw2Btur6nmQOb/view?usp=drive_link)

**Split Files link:** [PlantVillage_Split_Dataset](https://drive.google.com/file/d/1zfKxQJHkX2W6bzg-As3xULHkaDAuB5eG/view?usp=drive_link)

* Contains images of healthy and diseased plant leaves
* Multiple crop types and disease categories

---

## 📊 Week 1: Image Acquisition, EDA & Preprocessing

### ✔ Data Loading

* Loaded dataset from local directory
* Verified folder structure (class-wise images)

### ✔ Exploratory Data Analysis (EDA)

* Visualized sample images from different classes
* Analyzed class distribution to detect imbalance

### ✔ Data Preprocessing

* Resized images to **224 × 224**
* Normalized pixel values (0–255 → 0–1)
* Split dataset into:

  * Train (70%)
  * Validation (15%)
  * Test (15%)

---

## ⚙️ Preprocessing Pipeline

* Automated data splitting
* TensorFlow dataset creation
* Applied normalization and prefetching for performance optimization

---

## 🛠️ Tools & Technologies

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib

---

## 📂 Project Structure

```
Crop-Disease-Detection/
│── PlantVillage_color/
│── PlantVillage_split/
│   ├── train/
│   ├── val/
│   └── test/
│── notebooks/
│── README.md
```

---

## 📈 Evaluation Metrics (Upcoming)

* Accuracy
* Precision
* Recall (focus on minimizing missed disease cases)

---

## 🌱 Future Work

* CNN model training
* Model optimization and accuracy improvement
* Confusion matrix & performance analysis

---

## 💡 Conclusion

This project aims to create a simple and effective system for early detection of crop diseases, supporting smart farming and improving agricultural productivity.




Sure 👍 — here is your **full Week 2 write-up with updated Next Step (Week 3)** in simple 1st-year style:

---

# 📊 Week 2: CNN Model Training

🚧 **Project Status:** Week 2 Completed

---

## 🎯 Objective

In this week, We built a **basic CNN model** to classify plant leaf diseases using images.

---

## 🧠 Model

We created a **Custom CNN model** using:

* Conv2D layers
* MaxPooling layers
* Dense layers

Also used:

* Dropout to reduce overfitting

---

## ⚙️ Training

* Loss function: `categorical_crossentropy`
* Optimizer: Adam
* Model trained on training data
* Checked performance using validation data

---

## 🛑 Overfitting Control

To avoid overfitting, We used:

* Dropout
* EarlyStopping
* ReduceLROnPlateau

---

## 📈 Monitoring

We plotted:

* Accuracy graph
* Loss graph

This helped us understand how well the model is learning.

---

## 📊 Observation

* Model started learning patterns from images
* Validation accuracy improved slowly
* Some overfitting was controlled using dropout

---

## 💡 Conclusion

In Week 2, we successfully trained a **basic CNN model**.
This is our baseline model, and we will improve it in the next weeks.

---


