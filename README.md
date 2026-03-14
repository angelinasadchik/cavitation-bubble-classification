# cavitation-bubble-classification

Cavitation Bubble Classification using CNN

This project explores whether cavitation bubble patterns
in sparkling liquids contain enough visual information
to classify the liquid type.

Dataset
Frames were extracted from publicly available cavitation
videos using FFmpeg. Images were labeled according
to the corresponding liquid.

Method
A small convolutional neural network was trained
for binary image classification.

Training setup:
- train / validation split: 80 / 20
- optimizer: Adam
- loss: cross entropy
- data augmentation

Results
The model achieved ~0.91 validation accuracy
on the held-out validation set.

Future work
Future experiments will include:
- larger datasets
- temporal models using video sequences
- deeper CNN architectures
