# Handwritten Digit Classification using Deep Learning


🎯 Overview -

This project builds a Convolutional Neural Network (CNN) to automatically recognize handwritten digits (0–9) using the MNIST dataset. The aim is to demonstrate how deep learning models can learn visual patterns from images and perform accurate multiclass classification.

The MNIST dataset contains:

• 60,000 training images

• 10,000 test images

Each image is 28 × 28 pixels in grayscale.



🧹 Dataset Exploration & Visualization -

• Imported the MNIST dataset using keras.datasets.mnist.

• Visualized sample images using Matplotlib.

• Displayed pixel intensity distributions using Seaborn heatmaps.

• Plotted the first 9 images along with their labels to understand digit patterns.



📁 Data Preprocessing -

• Normalized pixel values from 0–255 to 0–1 to improve training performance.

• Converted class labels into one-hot encoded vectors using to_categorical for multiclass classification.

• Reshaped images to match CNN input format: (28, 28, 1).



🛠 Model Architecture -

A Sequential CNN model was built using Keras with the following layers:

1.Input Layer: 28×28×1 grayscale images

2.Convolution Layer:

• 32 filters

• Kernel size: 3×3

• Activation: ReLU

3.Max Pooling Layer: Reduces spatial dimensions

4.Flatten Layer: Converts 2D feature maps to 1D

5.Dropout Layer: Prevents overfitting

6.Dense Output Layer:

• 10 neurons

• Softmax activation for digit classification



📌 Model Training - 

• Optimizer: Adam

• Loss Function: Categorical Cross-Entropy

• Metrics: Accuracy

• Epochs: 15

• Validation Split: 20%

The training process tracked accuracy and loss across epochs to evaluate learning performance.



🧹Results & Performance -

• The CNN successfully learned patterns in handwritten digits.

• Achieved high classification accuracy on validation data.

• Demonstrated the effectiveness of CNNs for image recognition tasks.



🛠Tools & Technologies -

• Python

• TensorFlow / Keras

• CNN

• MNIST Dataset

• Matplotlib & Seaborn



📌Business/Practical Impact -

This model can be applied in:

• OCR systems

• Automated form processing

• Bank cheque digitization

• Postal code recognition

It shows how deep learning can automate image-based classification tasks with high reliability.

