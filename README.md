Chest CT Scan Classification using CNN
===================================================

This project implements a Convolutional Neural Network (CNN) in TensorFlow/Keras to classify chest CT scan images into four categories:

- squamous.cell.carcinoma
- normal
- adenocarcinoma
- large.cell.carcinoma

---------------------------------------------------

Dataset Structure:
------------------
dataset_dir/
├── train/
│   ├── squamous.cell.carcinoma/
│   ├── normal/
│   ├── adenocarcinoma/
│   └── large.cell.carcinoma/
├── test/
└── valid/

Each class folder should contain images in .jpg, .png, etc.

---------------------------------------------------

Dependencies:
-------------
Install the required libraries:
pip install tensorflow numpy matplotlib seaborn scikit-learn

---------------------------------------------------

Main Features:
--------------
1. Class Count Visualization
   - Uses dictionary or directory counts to visualize image distribution.

2. Image Loading and Labeling
   - Uses ImageDataGenerator for loading images by class.

3. Data Preparation
   - Loads images and labels into NumPy arrays and splits into train/val/test sets.

4. CNN Model
   - 3 Conv+Pooling layers, followed by Dense and Softmax layers.

5. Training and Evaluation
   - Trains for 10 epochs, batch size 32.
   - Evaluates accuracy and shows confusion matrix.

6. Prediction
   - Predicts class and confidence for an individual image.

---------------------------------------------------

Output:
-------
- Test Accuracy (e.g., Test Accuracy: 92.13%)
- Class distribution bar chart
- Sample predictions visualization
- Confusion matrix heatmap
