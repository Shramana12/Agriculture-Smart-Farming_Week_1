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


# 🚀 Week 3: Transfer Learning & Hyperparameter Tuning

🚧 Project Status: Week 3 Completed

---

## 🎯 Objective

This week, we improved our model to get **better accuracy**.
We used a smarter method instead of building everything from scratch.

---

## 🧠 Model

We used a pre-trained model:

* **MobileNetV2**

👉 This model is already trained on **ImageNet dataset**, so it already knows basic image patterns.

---

## ✔ What we did

* Loaded pre-trained model
* Froze all base layers
* Added our own layers on top
* Trained only the top layers first

---

## ⚙️ Training

### Phase 1

* Base model frozen
* Trained only new layers

### Phase 2

* Unfroze last few layers
* Used very low learning rate

👉 This helped improve accuracy.

---

## 🔧 Hyperparameter Tuning

We tested different learning rates:

* 0.001
* 0.0001

👉 Selected the best one automatically.

---

## 🛑 Overfitting Control

We used:

* Dropout
* EarlyStopping
* ReduceLROnPlateau

👉 This helped the model not overfit.

---

## 📈 Monitoring

* Checked accuracy graph
* Checked loss graph

👉 To see how the model is learning.

---

## 📊 Evaluation

* Accuracy
* Precision
* Recall
* Confusion Matrix

---

## 📊 Result

* Accuracy improved from Week 2
* Model learned faster
  
---

## 💡 Conclusion

Transfer Learning helped us build a **better and faster model**.
The model can now detect crop diseases more accurately.


---

# 🚀 Week 4: Evaluation, Inference & Deployment

🚧 Project Status: Week 4 Completed

---

# 🎯 Objective

In this week, we checked how well our final model works.
We also saved the model and created a prediction system for new unseen images.

---

# 🧠 Model Evaluation

We tested the model performance using different evaluation methods.

✔ We checked:

* Accuracy
* Precision
* Recall
* Confusion Matrix

👉 These helped us understand model performance better.

---

# 📊 Confusion Matrix

We created a Confusion Matrix to see which diseases are predicted correctly and which diseases are getting confused with other similar diseases.

✔ Observation

* Most diseases were predicted correctly
* Some similar diseases were slightly confused

👉 This helped us find model mistakes easily.

---

# 💾 Saving the Model

We saved:

* Final trained model
* Model weights

👉 So the model can be used later without training again.

---

# 🖼️ Inference System

We created an inference script for testing new images.

✔ The script can:

* Take a new image
* Predict the disease name
* Show confidence score

👉 This makes the project ready for real-world use.

---

# ⚙️ Project Organization

We organized the project files properly.

✔ Repository includes:

* Training notebooks
* Saved model
* Inference script
* Result graphs
* README file

👉 This makes the project clean and easy to understand.

---

# 📈 Monitoring

We checked:

* Accuracy graph
* Loss graph
* Confusion Matrix

👉 These graphs helped us understand model learning.

---

# 📊 Final Observation

* Model performance improved a lot
* Transfer Learning helped increase accuracy
* Model worked well on unseen images
* Some similar diseases were still slightly confusing

---

# 💡 Conclusion

In Week 4, we successfully completed the final testing and deployment preparation of our project.

The model can now predict plant leaf diseases from new images and also provide confidence scores.

----
