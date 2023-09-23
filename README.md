
# Bezubaan - Image Classification with Convolutional Neural Networks for Animal Welfare

## Overview

Bezubaan is an animal welfare project with a mission to promote Sustainable Development Goal 15 (SDG 15): "Life on Land." The project leverages Artificial Intelligence (AI) to predict whether an animal is injured or not, with a focus on improving the well-being of animals in various environments. It demonstrates image classification using Convolutional Neural Networks (CNNs). In this project, we use TensorFlow and Keras to build and train a CNN model to classify images of cats and dogs. The goal is to create a model that can accurately distinguish between these two classes.

## Project Inspiration

**Project Creator**: [mahikkaaa](https://github.com/mahikkaaa)

**Tagline**: "Be Kind to All Kinds"

**Project Vision**: To be the voice (Zubaan) for the voiceless (Bezubaan) animals.

### Why Bezubaan?

As a dedicated pet parent and animal lover, I have witnessed the silent suffering of animals who cannot communicate their pain or distress to us. This inability to express their needs often leads to delayed care and treatment.

Bezubaan is my response to this issue. By harnessing the power of AI, we aim to bridge the communication gap between animals and humans, enabling early detection and intervention in cases of injury or distress.

## How Bezubaan Works

Bezubaan employs machine learning models trained on various animal behavior and health datasets to predict an animal's condition. Through image recognition and sensor data analysis, the system can provide valuable insights into an animal's well-being.


## Dataset

We used the "Dogs vs. Cats" dataset, which can be found on Kaggle [here](https://www.kaggle.com/datasets/salader/dogs-vs-cats). This dataset contains thousands of images of cats and dogs, making it suitable for training and testing our image classification model.

## Getting Started

To replicate or build upon this project, follow these steps:

1. **Data Download**: Download the "Dogs vs. Cats" dataset from Kaggle using the provided URL.

2. **Data Preparation**: Organize the dataset into a train and test split. You can follow the directory structure used in the code for easy integration.

3. **Data Preprocessing**: Normalize the image data to values between 0 and 1 for improved model training. This preprocessing step is essential for training deep learning models.

4. **Model Architecture**: We implemented a CNN model with three convolutional layers, max-pooling layers, and fully connected layers. The model is designed to learn features from the input images and make predictions.

5. **Model Training**: Compile and train the CNN model using the training dataset. We used the Adam optimizer and binary cross-entropy loss for training. You can adjust the number of epochs based on your specific requirements.

6. **Evaluation**: Evaluate the trained model on the validation dataset to assess its accuracy and performance.

## Model Summary

The CNN model architecture used in this project is summarized as follows:

```plaintext
Layer (type)                Output Shape              Param #
===============================================================
conv2d (Conv2D)             (None, 254, 254, 32)      896
max_pooling2d (MaxPooling2D) (None, 127, 127, 32)      0
conv2d_1 (Conv2D)           (None, 125, 125, 64)      18496
max_pooling2d_1 (MaxPooling2 (None, 62, 62, 64)        0
conv2d_2 (Conv2D)           (None, 60, 60, 128)       73856
max_pooling2d_2 (MaxPooling2 (None, 30, 30, 128)       0
flatten (Flatten)           (None, 115200)            0
dense (Dense)               (None, 128)               14745728
dense_1 (Dense)             (None, 64)                8256
dense_2 (Dense)             (None, 1)                 65
===============================================================
Total params: 14,847,297
Trainable params: 14,847,297
Non-trainable params: 0
```

## Usage

- **Animal Welfare Organizations**: Bezubaan can be a valuable tool for animal welfare organizations and shelters to assess the health and well-being of animals under their care.

- **Pet Owners**: As a pet owner, you can use Bezubaan to monitor the health of your furry companions and ensure they receive prompt medical attention when needed.

- **Wildlife Conservation**: In wildlife conservation efforts, Bezubaan can assist in monitoring and protecting vulnerable species by identifying injured animals in their natural habitats.

## Author

- **GitHub**: [mahikkaaa](https://github.com/mahikkaaa)

Thank you for your interest in the BeZubaan project. We believe that by combining machine learning with our collective efforts, we can work towards a brighter and safer future for animals around us!
