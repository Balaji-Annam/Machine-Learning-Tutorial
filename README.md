# Data Augmentation for CNNs: A Comparative Study on CIFAR-10

## Overview
This repository contains the complete code, figures, and written tutorial for the assignment titled “Data Augmentation for Convolutional Neural Networks.” The project investigates how different augmentation strategies—horizontal flip, rotation, shift–zoom, and a heavy combined augmentation—affect the performance of a CNN trained on the CIFAR-10 dataset. All models use an identical architecture so that differences in performance can be attributed solely to the augmentation technique applied.

## Repository Structure
The repository is organised as follows:


24074613_ML_Code.ipynb – Jupyter notebook containing complete runnable code
24074613_ML_Report.pdf – Final written tutorial submitted for assessment
figures/ – Folder containing all exported figures used in the tutorial
- loss_curves.png
- accuracy_curves.png
- test_accuracy_bar.png
- cm_baseline.png
- cm_flip.png
- cm_rotation.png
- cm_shiftzoom.png
- cm_heavy.png
README.md – This file
LICENSE – MIT license



## Installation

To install required dependencies, run:

pip install tensorflow numpy matplotlib scikit-learn

Running the Notebook

To launch the notebook:

jupyter notebook - 24074613_ML_Code.ipynb

The notebook will:

- Load and preprocess CIFAR-10
- Train five CNN models (baseline, flip, rotation, shift–zoom, heavy)
- Generate learning curves (training/validation loss and accuracy)
- Produce a bar chart comparing test accuracies
- Compute classification reports and confusion matrices
- Save all plots into the figures/ directory

All figures included in the PDF tutorial can be reproduced by running the notebook.

## Summary of Results

Baseline – 0.7686
Flip – 0.7634
Rotation – 0.7487
Shift–Zoom – 0.7379
Heavy – 0.7190

## Key Insight:

Light augmentation such as horizontal flipping performs almost as well as the baseline model, while stronger geometric transformations—especially rotation and combined heavy augmentation—reduce accuracy. The study demonstrates that augmentation must encode meaningful invariances present in the dataset; otherwise, it acts as noise and degrades performance.

## Accessibility Considerations

This project follows recommended accessibility guidelines:

- Colour-blind-safe palettes were used in all plots
- High-contrast axis labels and tick marks
- Alt-text descriptions provided for every figure in the tutorial
- Legends include markers/shapes, not only colour
- Tables designed to remain readable without colour
- Clear heading levels for screen reader compatibility

## References

Bengio, Y., Goodfellow, I., & Courville, A. (2016). Deep Learning. MIT Press.
Krizhevsky, A. (2009). Learning Multiple Layers of Features from Tiny Images.
Perez, L., & Wang, J. (2017). The effectiveness of data augmentation in image classification.
Shorten, C., & Khoshgoftaar, T. M. (2019). A survey on image data augmentation for deep learning.

Additional references are included in the full PDF tutorial.

## Citation

if you use this repository in academic or instructional work, please cite it as:

[Annam Balaji] (2025). "Data Augmentation for CNNs: A Comparative Study on CIFAR-10."

Github Repository: https://github.com/Balaji-Annam/Machine-Learning-Tutorial.git

## License

This repository is licensed under the MIT License, allowing reuse, modification, and distribution with proper attribution.
