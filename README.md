# AWS SageMaker and TensorFlow Tyre Condition Classifier

![Tyre Condition Classifier](img1)

## Introduction

This repository provides a solution for classifying the condition of tires using AWS SageMaker and TensorFlow. The goal is to build a machine learning model that can predict whether a tire is in good or defective condition based on image data.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Dataset](#dataset)
- [Setup](#setup)
- [Inference](#inference)
- [Model Evaluation](#model-evaluation)
- [Deploying the Model](#deploying-the-model)
- [References](#references)

## Prerequisites

Before getting started, ensure you have the following prerequisites in place:

- [AWS Account](https://aws.amazon.com/)
- [AWS SageMaker](https://aws.amazon.com/sagemaker/)
- [Python](https://www.python.org/) (3.7 or later)
- [TensorFlow](https://www.tensorflow.org/) (2.x)
- [AWS Command Line Interface (CLI)](https://aws.amazon.com/cli/)

## Dataset

The tire condition dataset consists of images of tires in various conditions: good, fair, and poor. You can obtain this dataset from [Kaggle](https://www.kaggle.com/datasets/warcoder/tyre-quality-classification). The dataset is organized as the same structure used for and AWS image classifcation dataset.

## Training

