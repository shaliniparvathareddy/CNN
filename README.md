# CNN Image Classification using CIFAR-10

## Shiv Nadar University Chennai

### CS3807 – Deep Learning Laboratory

**Experiment 3: Implementation of Convolutional Neural Networks (CNNs) for Image Classification**

---

## 1. Objective

The objective of this experiment is to understand the working principle of Convolutional Neural Networks (CNNs) by implementing convolution, pooling, feature map visualization, and image classification using TensorFlow/Keras.

---

## 2. Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pandas
- Scikit-learn
- Seaborn
- CIFAR-10 Dataset

---

## 3. Dataset

The CIFAR-10 dataset is used for image classification.

The dataset contains:

- 50,000 training images
- 10,000 testing images
- 10 classes
- Image size: 32 × 32 × 3
- RGB color images

### CIFAR-10 Classes

1. Airplane
2. Automobile
3. Bird
4. Cat
5. Deer
6. Dog
7. Frog
8. Horse
9. Ship
10. Truck

---

## 4. CNN Architecture

The CNN used in this experiment follows the architecture:

Input
↓
Convolution
↓
ReLU
↓
Max Pooling
↓
Convolution
↓
ReLU
↓
Max Pooling
↓
Flatten
↓
Dense
↓
Softmax
↓
Output

### Model Configuration

- Conv1: 32 filters, 3 × 3 kernel
- Conv2: 64 filters, 3 × 3 kernel
- Activation: ReLU
- Pooling: Max Pooling
- Optimizer: Adam
- Epochs: 20
- Batch size: 32
- Output classes: 10

---

## 5. Experiment Tasks

The experiment consists of the following tasks:

### Task 1 – Dataset Analysis

- Load the CIFAR-10 dataset.
- Display sample images.
- Print dataset dimensions.
- Plot class distribution.

### Task 2 – Convolution

Compare convolution using:

- 3 × 3 kernel
- 5 × 5 kernel
- 7 × 7 kernel

Record and compare the resulting feature-map sizes.

### Task 3 – Stride and Padding

Study the effect of:

- Stride = 1
- Stride = 2
- Same padding
- Valid padding

on the output feature-map dimensions.

### Task 4 – Feature Map Visualization

Visualize at least eight feature maps produced by the first convolutional layer.

### Task 5 – Pooling Comparison

Compare:

- Max Pooling
- Average Pooling

using a 2 × 2 pooling window.

Compare their output dimensions and classification accuracy.

### Task 6 – CNN Classification

Construct and train the CNN using:

- Adam optimizer
- 20 epochs
- Batch size of 32

### Task 7 – Model Evaluation

Evaluate the trained CNN using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

---

## 6. Generated Figures

The experiment generates the following figures:

- `sample_images.png`
- `class_distribution.png`
- `feature_maps_comparison.png`
- `kernel_vs_featuremap_size.png`
- `stride_padding_comparison.png`
- `first_layer_feature_maps.png`
- `maxpool_vs_avgpool_featuremaps.png`
- `pooling_accuracy_comparison.png`
- `trainingaccuracy vs epoch.png`
- `validationvsepoch.png`
- `feature_map.png`
- `correlation.png`

These figures are used in the experiment report to visualize the results.

---

## 7. Results

The CNN achieved the following performance:

| Metric | Value |
|---|---:|
| Training Accuracy | 82.39% |
| Testing Accuracy | 69.83% |
| Precision | 70.28% |
| Recall | 69.83% |
| F1-score | 69.84% |
| Parameters | 60,362 |

The model achieved approximately 69.83% accuracy on the CIFAR-10 test dataset.

---

## 8. Observations

### Kernel Size

As the kernel size increases from 3 × 3 to 7 × 7, the spatial dimensions of the feature map decrease when valid padding is used.

### Stride

Increasing the stride reduces the spatial dimensions of the output feature map.

### Padding

Same padding preserves the spatial dimensions, whereas valid padding reduces the spatial dimensions.

### Pooling

Both Max Pooling and Average Pooling reduce the spatial dimensions of the feature map.

In this experiment, Max Pooling achieved better test accuracy than Average Pooling.

### Training and Testing Accuracy

The training accuracy is higher than the testing accuracy. This indicates that the model performs better on the data it was trained on than on unseen data and suggests some degree of overfitting.

---

## 9. Installation

Clone the repository:

```bash
git clone <repository-url>
