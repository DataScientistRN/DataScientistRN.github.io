---
title: Brain Tumor Classification with CNNs
summary: A custom convolutional neural network that classifies brain MRIs as glioma, meningioma, pituitary tumor or normal with 97% accuracy, served through a Flask web app.
tags: [Deep Learning, CNN, TensorFlow, Flask]
github: https://github.com/DataScientistRN/Brain-Tumor-Classification-with-CNN-Fall-2025
icon: brain
color: mint
order: 3
---

*CSCI E-89 Deep Learning · Fall 2025*

Radiologists sometimes miss brain cancers on MRI, which makes AI a promising second reader. This project trains a CNN from scratch on the Kaggle Brain Tumor MRI dataset to tell apart normal scans from gliomas, meningiomas and pituitary tumors.

The network has four convolution and max-pooling layers, dropout and two dense layers with a softmax output, trained for 50 epochs. It reached 97% accuracy, precision and recall, and was deployed with Flask so a user can upload a scan and get a prediction.
