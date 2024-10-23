# Bone-Fracture-Classification
A deep learning model that detects fractures in bone X-ray images using a fine-tuned ResNet50 architecture. The model achieves 85% accuracy in classifying whether an X-ray image contains fractures or not.

## Overview

This project implements a binary classification model to detect the presence of fractures in X-ray images. It utilizes transfer learning with a pre-trained ResNet50 model, fine-tuned on the FracAtlas dataset.

## Dataset

The model is trained on the [FracAtlas](https://www.nature.com/articles/s41597-023-02432-4) dataset, which contains X-ray images of bones labeled as either:
* Fractured
* Non-fractured

## Technical Stack

* **Framework:** TensorFlow
* **Base Model:** ResNet50 (pre-trained on ImageNet)
* **Python Version:** 3.x
* **Key Libraries:**
  * tensorflow
  * numpy
  * pandas
  * matplotlib
  * scikit-learn

## Model Performance

* **Accuracy:** 85%
* **Architecture:** Fine-tuned ResNet50
* **Training Setup:** Transfer Learning


## Model Training

The model was trained using the following approach:
1. Load pre-trained ResNet50 with ImageNet weights
2. Fine-tune on FracAtlas dataset
3. Train with data augmentation for better generalization
4. Implement early stopping to prevent overfitting


## Acknowledgments
* FracAtlas dataset team for providing the training data
* ResNet50 authors for the base architecture
