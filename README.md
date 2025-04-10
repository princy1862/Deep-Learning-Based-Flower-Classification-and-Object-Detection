
# Deep Learning-Based Flower Classification and Object Detection

## Overview

This project focuses on using deep learning techniques for **flower classification** and **automobile object detection**. The goal is to create a convolutional neural network (CNN) for classifying flower species and implement an object detection method using a sliding window approach for vehicle detection.

## Features

- **Flower Classification**: A custom CNN is trained on a 10-class flower dataset to classify images of different flower species.
- **Car Object Detection**: A sliding window method is used to detect automobile objects in images with a pre-trained model for bounding box regression.

## Technologies Used

- **Deep Learning** (CNNs for image classification)
- **Python** (for model implementation)
- **Keras/TensorFlow** (for CNN model training)
- **Sliding Window Technique** (for object detection)

## Dataset

- **Flower Dataset**: The dataset includes images of 10 flower species (such as lilies, roses, etc.). Each image is normalized and resized to 300×300 pixels.
- **Car Object Detection**: A custom dataset with cars annotated using bounding boxes.

## Model Architecture

### Flower Classification CNN:
- **3 Convolutional Layers** with Max-Pooling
- **Dropout for Regularization**
- **Dense Layer** for classification
- **Softmax Activation** for multi-class output

### Car Object Detection:
- Uses a **sliding window technique** for detecting automobiles.
- A pre-trained model for bounding box regression is used with a **50-pixel stride**.

## Results

- **Flower Classification**: Achieved a **71.7% validation accuracy**. Overfitting was observed after 15 epochs.
- **Car Object Detection**: Achieved an **average Intersection over Union (IoU)** of **0.72**.

## Challenges and Future Directions

- **Overfitting** in flower classification can be mitigated by using advanced **regularization techniques** and **data augmentation**.
- The **sliding window approach** for object detection is **computationally expensive** and prone to missing objects, with potential improvements using **region-based techniques** like **YOLO** or **Faster R-CNN**.
- Future work will focus on improving the **generalization** of the model and enhancing **computational efficiency**.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

