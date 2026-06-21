# 🍎 Fruit Classification using VGG16, Keras, and TensorFlow

## Overview

This project implements a **Fruit Classification System** using Deep Learning and Transfer Learning techniques. The model is built using the pre-trained **VGG16** convolutional neural network as the feature extraction backbone, while **Keras** and **TensorFlow** are used to create and train the classification layers.

The objective of this project is to accurately identify and classify different types of fruits from images, demonstrating the effectiveness of transfer learning for image recognition tasks.

---

## Features

* Transfer Learning using VGG16
* Image classification of multiple fruit categories
* Custom classification layers built with Keras
* TensorFlow-based model training and optimization
* Image preprocessing and data augmentation
* High accuracy with reduced training time
* Scalable architecture for adding new fruit categories

---

## Technologies Used

* Python
* TensorFlow
* Keras
* VGG16 (Pre-trained on ImageNet)
* NumPy
* Matplotlib
* Scikit-learn
* OpenCV

---

## Project Architecture

The model uses a pre-trained VGG16 network for feature extraction and custom Keras layers for fruit classification.

```text
Input Fruit Image
        ↓
Image Preprocessing
        ↓
Pre-trained VGG16
        ↓
Flatten Layer
        ↓
Dense Layer(s)
        ↓
Dropout Layer
        ↓
Output Layer (Softmax)
        ↓
Predicted Fruit Class
```

---

## Dataset

The dataset consists of labeled fruit images belonging to multiple categories such as:

* Apple
* Banana
* Orange
* Mango
* Grapes
* Pineapple
* Watermelon
* Other fruit classes

Each image is associated with a corresponding fruit label used for supervised learning.

---

## Data Preprocessing

To improve model performance and generalization, the following preprocessing techniques were applied:

* Image resizing
* Pixel normalization
* Data augmentation:

  * Rotation
  * Horizontal flipping
  * Zooming
  * Width and height shifting
  * Shearing

These techniques help the model learn robust features and reduce overfitting.

---

## Model Development

### Base Model: VGG16

The pre-trained VGG16 model was used as the feature extraction backbone.

Benefits of VGG16:

* Trained on the large-scale ImageNet dataset
* Learns powerful visual features
* Reduces training time
* Performs well on image classification tasks

### Custom Classification Layers

Additional Keras layers were added on top of VGG16 to adapt the model for fruit classification.

Typical layers include:

* Flatten Layer
* Dense Layer(s)
* Dropout Layer
* Softmax Output Layer

---

## Training Workflow

```text
Fruit Dataset
      ↓
Data Preprocessing
      ↓
Data Augmentation
      ↓
Feature Extraction using VGG16
      ↓
Custom Keras Layers
      ↓
Model Training
      ↓
Validation
      ↓
Fruit Prediction
```

---

## Evaluation Metrics

The model was evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

These metrics provide insights into the classification performance across different fruit categories.

---

## Results

The VGG16-based transfer learning model successfully classified fruit images with high accuracy while significantly reducing training time compared to training a convolutional neural network from scratch.

### Key Observations

* Transfer learning accelerated model convergence.
* VGG16 extracted meaningful visual features from fruit images.
* Data augmentation improved model generalization.
* Keras and TensorFlow enabled efficient model development and training.

---

## Applications

* Automated fruit recognition systems
* Smart agriculture solutions
* Grocery store inventory management
* Fruit sorting and grading systems
* Educational computer vision projects

---

## Future Enhancements

* Experiment with modern architectures such as EfficientNet, ResNet50, and Vision Transformers (ViT).
* Increase dataset diversity to improve robustness.
* Implement real-time fruit classification using webcams.
* Deploy the model as a web or mobile application.
* Add fruit freshness and quality assessment features.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/fruit-classifier.git

cd fruit-classifier
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Train the model:

```bash
python train.py
```

Run predictions:

```bash
python predict.py --image sample_fruit.jpg
```

---

## Project Structure

```text
Fruit-Classifier/
│
├── dataset/
├── models/
├── notebooks/
├── train.py
├── predict.py
├── requirements.txt
├── README.md
└── saved_model/
```

---

## Conclusion

This project demonstrates the use of **Transfer Learning** for fruit image classification by combining the powerful feature extraction capabilities of **VGG16** with custom classification layers built using **Keras** and **TensorFlow**. The resulting model provides an efficient and accurate solution for recognizing different fruit categories from images, making it suitable for agricultural, retail, and educational applications.

---

## Author

**Roselyn Miriam Sunil**

*Fruit Classification using VGG16, Keras, and TensorFlow* 🍎🍌🍇🥭🚀
