# Classify Tyre Conditions with AWS SageMaker 

![Tyre Condition Classifier](./readMeImages/cover.png)

## Introduction

This repository provides a solution for classifying the condition of tires using AWS SageMaker and TensorFlow. The goal is to build a machine learning model that can predict whether a tire is in good or defective condition based on image data.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Dataset](#dataset)
- [Training Model](#training-model)
- [Model Evaluation](#model-evaluation)

## Prerequisites

Before getting started, ensure you have the following prerequisites in place:

- [AWS Account](https://aws.amazon.com/)
- [AWS SageMaker](https://aws.amazon.com/sagemaker/)
- [Python](https://www.python.org/) (3.7 or later)
- [TensorFlow](https://www.tensorflow.org/) (2.x)
- [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/)

## Dataset

The tire condition dataset consists of images of tires in various conditions: good, fair, and poor. You can obtain this dataset from [Kaggle](https://www.kaggle.com/datasets/warcoder/tyre-quality-classification). The dataset is organized as the same structure used for and AWS image classification dataset.

## Training Model

This model was trained using [Swin Transformer model](https://tfhub.dev/sayakpaul/swin_base_patch4_window7_224/1) pre-trained on ImageNet-21k (14 million images, 21,841 classes) at resolution 224x224, suitable for off-the-shelf classification. The "Swin-Base-Patch4-Window7-224" computer vision model is a moderately sized Swin Transformer architecture that processes input images divided into non-overlapping 4x4 pixel patches, uses a 7x7 window for self-attention, and is designed to work with images of 224x224 pixels. This model is suitable for various computer vision tasks and has demonstrated strong performance in the field of deep learning-based image analysis.

## Model Evaluation
![Training Chart](./readMeImages/chart_image.png)

Training 6 models with different learning rates, we can see all of the models achieved a validation accuracy of around 95%. A computer vision image classification model with a validation accuracy of 95% is already quite impressive, indicating that the model is doing a good job at correctly classifying images. However, there is always room for improvement. For instance, we can apply data augmentation techniques like rotation, scaling, and flipping to artificially increase the variety of training samples. This can help the model become more robust to different image variations.
