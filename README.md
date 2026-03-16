# cavitation-bubble-classification

# Cavitation Bubble Classification with CNNs

This project explores whether cavitation bubble patterns contain enough visual information to distinguish between different sparkling wine types using computer vision.

## Project Idea

Cavitation bubbles formed in liquids often produce complex visual patterns.  
This project investigates whether these patterns can be analyzed using deep learning models.

## Dataset

The dataset was constructed from publicly available cavitation videos.  
Video frames were extracted using FFmpeg.

Dataset statistics:

- Total images: 1495
- Classes: 2
- Pink sparkling wine: 652
- White sparkling wine: 843

## Model

A simple convolutional neural network was used:

- 3 convolutional layers
- ReLU activation
- max pooling
- fully connected classifier

## Training

- optimizer: Adam
- loss: cross-entropy
- train/validation split: 80/20
- epochs: 5

## Results

The model achieved approximately **0.91 validation accuracy**.

Example confusion matrix:

![Confusion Matrix](confusion_matrix.png)

## Motivation

This project was inspired by my participation in the National Technological Olympiad in the Infochemistry track, where I worked on applying machine learning methods to analyze scientific visual data.

## Future Work

Future work could include:

- larger datasets
- temporal modeling using video sequences
- deeper CNN architectures
