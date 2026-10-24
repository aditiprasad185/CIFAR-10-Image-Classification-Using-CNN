CIFAR-10 Image Classification using Convolutional Neural Networks (CNN)

📌 Project Overview

This project implements an image classification model using a **Convolutional Neural Network (CNN)** and TensorFlow/Keras to classify images from the CIFAR-10 dataset into 10 different categories.

The model learns visual features from color images and predicts the category to which each image belongs. The project also evaluates model performance using test accuracy, a confusion matrix, and a classification report.

🎯 Objectives

- Build a CNN model for multi-class image classification.
- Load and preprocess the CIFAR-10 dataset.
- Normalize image pixel values for efficient training.
- Train the model using TensorFlow and Keras.
- Evaluate model performance on unseen test images.
- Visualize training progress and classification results.
- Save the trained model for future use.

📂 Dataset

The project uses the **CIFAR-10 dataset**, which contains 60,000 color images divided into 10 classes.

- Training images: 50,000
- Testing images: 10,000
- Image dimensions: 32 × 32 pixels
- Image channels: 3 (RGB)
- Number of classes: 10

Classes

1. Airplane
2. Automobile
3. Bird
4. Cat
5. Deer
6. Dog
7. Frog
8. Horse
9. Ship
10. Truck

The dataset is loaded directly using `keras.datasets.cifar10.load_data()`.

🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

🧠 Model Architecture

The CNN is implemented using the Keras Sequential API.

The architecture consists of:

1. Input Layer: Accepts RGB images of size 32 × 32 × 3.
2. Convolutional Layer: 32 filters with a 3 × 3 kernel and ReLU activation.
3. Max Pooling Layer: Reduces spatial dimensions.
4. Convolutional Layer: 64 filters with a 3 × 3 kernel and ReLU activation.
5. Max Pooling Layer: Further reduces spatial dimensions.
6. Convolutional Layer: 128 filters with a 3 × 3 kernel and ReLU activation.
7. Max Pooling Layer: Reduces spatial dimensions further.
8. Flatten Layer: Converts feature maps into a one-dimensional vector.
9. Dense Layer: 128 neurons with ReLU activation.
10. Dropout Layer: Dropout rate of 0.4 to help reduce overfitting.
11. Output Layer: 10 neurons with Softmax activation for classification.

Training Configuration

- Optimizer: Adam
- Loss function: Sparse categorical cross-entropy
- Evaluation metric: Accuracy
- Maximum epochs: 20
- Batch size: 128
- Validation split: 20%
- Early stopping patience: 3 epochs
- Model checkpoint: Saves the best model based on validation loss

⚙️ Installation and Setup

1. Clone the repository

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

2. Install the required libraries

```bash
pip install tensorflow numpy matplotlib scikit-learn jupyter
```

3. Launch Jupyter Notebook

```bash
jupyter notebook
```

4. Run the notebook

Open `CIFAR10_CNN_Image_Classification.ipynb` and execute the cells sequentially.

The CIFAR-10 dataset will be downloaded automatically when it is first loaded, if it is not already available locally.

🚀 Project Workflow

1. Import the required libraries.
2. Load the CIFAR-10 training and testing datasets.
3. Visualize sample images and their class labels.
4. Normalize pixel values to the range 0–1.
5. Build the CNN model.
6. Compile the model using Adam and sparse categorical cross-entropy.
7. Train the model with validation data.
8. Apply early stopping and model checkpointing.
9. Plot training and validation accuracy and loss.
10. Evaluate the model on the test dataset.
11. Generate a confusion matrix and classification report.
12. Visualize actual versus predicted labels.
13. Save the trained model.

📊 Model Evaluation

The project evaluates performance using:

- Test Accuracy: Measures the proportion of correctly classified test images.
- Test Loss: Measures the model's prediction error.
- Confusion Matrix: Shows correct and incorrect predictions across all 10 classes.
- Classification Report: Provides precision, recall, and F1-score for each class.
- Training and Validation Curves: Help monitor learning progress and potential overfitting.
- Prediction Visualization: Compares actual and predicted labels for sample test images.

The numerical results depend on the actual training run. Run the notebook to obtain the final test accuracy and evaluation metrics.

💾 Saved Models

The notebook saves the trained model in Keras format:

- `cifar10_cnn_best.keras` — Best checkpoint based on validation loss.
- `cifar10_cnn_final.keras` — Model saved at the end of the notebook.

📁 Repository Structure

```text
CIFAR10-CNN-Image-Classification/
│
├── CIFAR10_CNN_Image_Classification.ipynb
├── README.md
├── cifar10_cnn_best.keras       # Generated during training
└── cifar10_cnn_final.keras      # Generated when the notebook finishes
```

The model files will appear after the relevant notebook cells execute. They do not need to be committed to GitHub unless you intend to share the trained weights.

🔮 Future Improvements

- Experiment with deeper CNN architectures.
- Apply data augmentation to improve generalization.
- Tune hyperparameters such as learning rate, batch size, and dropout rate.
- Compare performance with transfer learning models.
- Build a simple web application for image prediction.

👩‍💻 Author

Aditi Prasad

This project is available for educational and learning purposes. Add a suitable open-source license if you intend to distribute the code.
