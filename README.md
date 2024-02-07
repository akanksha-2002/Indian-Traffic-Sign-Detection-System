# Indian Traffic Sign Detection and Recognition System
This project aims to develop a real-time Indian traffic sign detection and recognition system using state-of-the-art deep learning models, specifically YOLOv8 and RCNN. The system is designed to accurately detect and classify traffic signs in dynamic scenarios, providing precise localization and scoring mechanisms for adaptability.

## Overview
The system is implemented using the following components:

### Dataset:
- The dataset used for training and testing the models is sourced from [Kaggle](https://www.kaggle.com/datasets/neelpratiksha/indian-traffic-sign-dataset), consisting of Indian traffic sign images.
- The images are preprocessed, including grayscale conversion, standardized lighting, and resizing.

### Model Architecture:

- **YOLOv8** : The YOLOv8 model is utilized for real-time object detection. It employs the **Darknet-53** architecture and predicts bounding boxes, object scores, and class scores at multiple scales.
- **RCNN** : Region-based Convolutional Neural Networks are used for fine-grained localization and recognition of traffic signs.
  
### Training:

- The models are trained on **Google Colab**, leveraging GPU acceleration for faster training.
- The training process involves iterating over **15,000 epochs** with an average loss of 0.5 and a learning rate of 0.001.
- Weights are saved periodically during training for further testing and evaluation.
  
### Annotation:

Bounding box annotations for traffic signs are generated using the **OpenLabeling** tool. Annotations are stored in TXT files following a specific format.
