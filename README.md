# Assignment-9
# 🐱🐶 Image Classification using Convolutional Neural Networks (CNN)

## 📌 Objective

The objective of this project is to develop a **Convolutional Neural Network (CNN)** to automatically classify images as **Cats** or **Dogs**. The model is trained using TensorFlow/Keras on the Cats vs Dogs dataset and evaluated using various classification metrics. This project demonstrates the application of deep learning techniques for image recognition and binary image classification.

---

## 📂 Dataset Link

**Dataset Name:** Cats vs Dogs Classification Dataset

**Source:** https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset

---

## 🛠️ Libraries Used

* Python
* NumPy
* Matplotlib
* TensorFlow / Keras
* Scikit-learn
* KaggleHub

---

## ⚙️ Methodology

1. Downloaded and loaded the Cats vs Dogs dataset using KaggleHub.
2. Displayed the folder structure and sample images with their class labels.
3. Resized all images to **128 × 128 pixels**.
4. Normalized pixel values to the range **0–1**.
5. Split the dataset into **80% training** and **20% validation/testing** using `ImageDataGenerator`.
6. Built a Convolutional Neural Network (CNN).
7. Trained the model for **10 epochs**.
8. Evaluated the model using Test Accuracy, Precision, Recall, F1-Score, Confusion Matrix, and Classification Report.
9. Visualized model performance using Accuracy vs Epoch and Loss vs Epoch graphs.

---

## 🧠 CNN Architecture

| Layer            | Configuration                       |
| ---------------- | ----------------------------------- |
| **Input Layer**  | 128 × 128 × 3 RGB Images            |
| **Conv2D**       | 32 Filters, 3×3, ReLU               |
| **MaxPooling2D** | 2×2                                 |
| **Conv2D**       | 64 Filters, 3×3, ReLU               |
| **MaxPooling2D** | 2×2                                 |
| **Conv2D**       | 128 Filters, 3×3, ReLU              |
| **MaxPooling2D** | 2×2                                 |
| **Flatten**      | Converts feature maps into a vector |
| **Dense Layer**  | 128 Neurons, ReLU                   |
| **Output Layer** | 1 Neuron, Sigmoid                   |

### Model Configuration

* **Optimizer:** Adam
* **Loss Function:** Binary Crossentropy
* **Metric:** Accuracy
* **Epochs:** 10

### Evaluation

* Confusion Matrix generated successfully.
* Classification Report generated for both classes.
* Accuracy vs Epoch graph plotted.
* Loss vs Epoch graph plotted.

### Key Observations

* The CNN successfully learned distinguishing visual features of cats and dogs through convolution and pooling operations.
* Training accuracy increased while training loss decreased over successive epochs, indicating effective learning.
* The confusion matrix demonstrated that the majority of images were classified correctly, with only a few misclassifications.
* The model showed good generalization performance on unseen validation/testing images.

---

## ✅ Conclusion

This project successfully implemented a Convolutional Neural Network (CNN) for classifying cat and dog images. Image preprocessing, including resizing and normalization, prepared the data for efficient training, while convolutional and pooling layers extracted meaningful visual features automatically. The trained CNN achieved effective image classification performance and demonstrated the strength of deep learning for computer vision tasks. Compared with a traditional Artificial Neural Network (ANN), CNN is better suited for image classification because it preserves spatial information and automatically learns hierarchical image features. However, CNN models require a large amount of labeled training data and greater computational resources, making training more time-consuming than simpler machine learning algorithms.

---

## 📁 Project Structure

```text
Assignment-9/
│── Assignment-9.ipynb
│── README.md
```

---

## ▶️ How to Run

1. Open the notebook in Google Colab.
2. Install the required dependencies:

   ```bash
   pip install kagglehub tensorflow
   ```
3. Run all notebook cells in sequence.
4. The notebook will:

   * Download and load the dataset.
   * Train the CNN model.
   * Evaluate the model.
   * Display the confusion matrix, classification report, and training graphs.

---

