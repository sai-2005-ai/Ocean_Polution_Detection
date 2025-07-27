🧠 Deep Learning Workflow: Image Classification & Anomaly Detection

Welcome! This repository contains an end-to-end deep learning pipeline built using Python and TensorFlow in Google Colab. It covers everything from data preprocessing, visualization, and augmentation to model training using CNNs and anomaly detection using Variational Autoencoders (VAE).


✅ Dataset Loading & Visualization

    Mount Google Drive and load images/labels

    Show sample images and bounding boxes

    Plot class distributions using seaborn

✅ YOLO Label Decoding & Visualization

    Parse .txt label files and draw bounding boxes

    Map class IDs to class names from data.yaml

✅ Preprocessing

    Resize and normalize images (416×416 or 224×224)

    Histogram equalization for grayscale images

✅ Data Augmentation

    Apply real-time transformations like:

        Rotation, flipping, zooming, shifting

    Save augmented images and labels to a new directory

    Generate a CSV file with augmented metadata

✅ CNN Classification

    Built using Conv2D, MaxPooling, Dense, and Dropout

    Uses binary cross-entropy for classification

    Trains on augmented dataset

✅ Variational Autoencoder (VAE)

    Encoder-decoder structure with custom KL-divergence loss

    Adds Gaussian noise to input images and reconstructs clean versions

    Used for anomaly detection via reconstruction error

✅ Evaluation

    Visualize model performance using:

        Accuracy/Loss curves

        Confusion matrix and classification report

        ROC Curve and AUC

📊 Visualization Samples

    📷 Sample image with bounding boxes

    📈 Class distribution bar plot

    🧼 Clean vs. Noisy image comparison

    🔁 Training vs. Validation Accuracy/Loss

    📉 ROC Curve and AUC

    🔥 Confusion matrix heatmap

🛠️ Technologies Used

    Python (NumPy, Pandas, OpenCV, Matplotlib, Seaborn)

    TensorFlow / Keras

    Google Colab (for training and visualization)

    YOLO-format annotations

    ImageDataGenerator (Keras)

💡 How to Use

    Clone this repository or upload your own dataset to Google Drive.

    Make sure your dataset path and structure match what’s shown above.

    Run each cell in the notebook step by step:

        Mount Drive

        Visualize and explore data

        Train CNN and/or VAE

        Evaluate and visualize metrics

📌 Results

    CNN model achieved an accuracy of ~100%.
