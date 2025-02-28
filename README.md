# Multi-Class Image Classification with CNN, ResNet50, and MobileNetV2

This project implements and compares three deep learning models—custom CNN, ResNet50, and MobileNetV2—for multi-class image classification. It uses a dataset stored in Google Drive, preprocesses images, trains the models with optional data augmentation, evaluates their performance, and saves the best model (MobileNetV2) for inference. A prediction function is also provided to classify new images into one of three categories: "abdur", "yash", or "sanjay".

## Features
- **Data Preprocessing:** Loads and normalizes images from Google Drive, resizes to 224x224.
- **Models:** Custom CNN, pretrained ResNet50, and pretrained MobileNetV2 with transfer learning.
- **Training:** Includes data augmentation (rotation, flip, zoom) and 10-epoch training with validation.
- **Evaluation:** Compares model accuracy on a test set.
- **Inference:** Predicts the category of a new image using the saved model.

## Dataset
- **Location:** `/content/drive/My Drive/classification_model`
- **Structure:** Subfolders named "0", "1", and "2" containing images for each class.
- **Size:** 56 images total (split into 44 train, 12 test).

## Requirements
- Google Colab environment with GPU support
- Python 3.11
- Libraries:
  - `tensorflow`
  - `opencv-python` (cv2)
  - `numpy`
  - `sklearn`
- Google Drive access for dataset
