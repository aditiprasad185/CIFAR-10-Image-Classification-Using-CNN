# CIFAR-10 Image Classification Using CNN

## Overview
This project uses a Convolutional Neural Network (CNN) to classify images into 10 categories from the CIFAR-10 dataset.

## Dataset
- **Dataset:** CIFAR-10
- **Total images:** 60,000
- **Image size:** 32 × 32 pixels
- **Image type:** RGB
- **Classes:** Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, and Truck

## Technologies
- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Key Features
- Image preprocessing and normalization
- CNN model development and training
- Multiclass image classification
- Model evaluation using test data
- Visualization of training performance and classification results

## Project Workflow
1. Load the CIFAR-10 dataset.
2. Preprocess the images and labels.
3. Build and train the CNN model.
4. Evaluate the model on test data.
5. Visualize the results.

## Installation
Install the required libraries:

```bash
pip install tensorflow numpy matplotlib scikit-learn jupyter
```

## How to Run
1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `CIFAR10_CNN_Image_Classification.ipynb`.
5. Run the notebook cells in order.

## Evaluation
The model's performance can be assessed using test accuracy, loss curves, and a confusion matrix, where implemented in the notebook.

## Future Improvements
- Experiment with deeper CNN architectures.
- Apply data augmentation.
- Tune hyperparameters to improve generalization.
- Compare performance across different model configurations.
