# Deep Learning Project: Identifying Pneumonia Diagnosis by CNN Classifier

## Project Overview

This project focuses on developing a deep learning model to aid in the diagnosis of pneumonia using chest X-ray images. The model aims to assist clinicians by automating the initial detection of potential pneumonia cases, thereby reducing the likelihood of missed diagnoses due to high workload or clinician fatigue.

## Motivation

Pneumonia is a leading cause of death among children under five years old globally. Accurate diagnosis is challenging, requiring the review of chest radiographs (CXR) by highly trained specialists. This project leverages deep learning to help mitigate the burden on clinicians and improve diagnostic accuracy.

## Data

### Dataset

<img width="332" alt="image" src="https://github.com/ColleenJung/Deep-Learning-Project-Identifying-Pneumonia-diagnosis-by-CNN-Classifier/assets/119357849/448af652-a7ee-4f73-b3b7-8893ca375d3c">

<img width="404" alt="image" src="https://github.com/ColleenJung/Deep-Learning-Project-Identifying-Pneumonia-diagnosis-by-CNN-Classifier/assets/119357849/a872dbda-6cec-43d4-925c-a25886701172">

- **Source**: Chest X-ray images.
- **Number of Observations**: 5,800 images.
- **Features**: Images labeled as Normal or Pneumonia.
- **Splits**: Training, Testing, Validation.

### Data Characteristics

- **Image Format**: JPEG
- **Dimensions**: 5700 x 3800 pixels
- **Color**: Grayscale (Black for Air, White for Bone, Grey for Tissue/Fluid)

## Methodology

### Model Architecture

The Convolutional Neural Network (CNN) is used for image classification. The base model utilized is VGG16, which is fine-tuned to enhance performance.

### Feature Engineering

- **Regularization**: L2 Regularization to encourage small weights and reduce overfitting.
- **Dropout**: Applied at different stages (30% after the Flatten layer, 20% after a Dense layer) to prevent overfitting.

### Model Layers

- **Flatten Layer**
- **Dropout (30%)**
- **Dense Layer (ReLU activation)**
- **Dropout (20%)**
- **Dense Layer (Sigmoid activation)**

## Results

<img width="462" alt="image" src="https://github.com/ColleenJung/Deep-Learning-Project-Identifying-Pneumonia-diagnosis-by-CNN-Classifier/assets/119357849/4300f873-2192-4a04-b88f-1a164406eb58">

<img width="462" alt="image" src="https://github.com/ColleenJung/Deep-Learning-Project-Identifying-Pneumonia-diagnosis-by-CNN-Classifier/assets/119357849/f04cdd9f-5e5e-48bb-b7dd-cee3a421caac">

- **Accuracy**: The CNN model achieved an accuracy of 93.7% in diagnosing pneumonia from chest X-rays.
- **Training Loss**: Decreased continuously over epochs.
- **Validation Loss**: Lowest at epoch 6 (0.1935).
- **Validation Accuracy**: Peaked at epoch 3 (93.75%).

### Example AI Report

The model provides a detailed diagnosis report indicating the presence of pneumonia with high confidence.

## Future Work

### Data Improvement

- Collect more varied data from different demographics and X-ray equipment to enhance model robustness.

### Model Tuning

- Experiment with different CNN architectures or newer models like EfficientNet or ResNets for better performance.

### Platform Design

- Develop a user-friendly interface for non-technical users such as radiologists to facilitate easier adoption of the technology.

### Clinical Integration

- Conduct a pilot study in a clinical setting to gather real-world data on model performance and acceptance among healthcare professionals.

## Funding and Resources

- Estimated $1.2M required for computational resources, high-quality data acquisition, and operational runway for the next 6 months.


