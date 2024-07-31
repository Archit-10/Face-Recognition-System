# Face-Recognition-using-PCA

This project involves creating a basic facial recognition system using Principal Component Analysis (PCA). The system projects face images onto a feature space, known as the "face space," which represents the variations among distinct faces. This face space is defined by "Eigenfaces," which are the eigenvectors of the set of faces.
Overview

The goal of this project is to recognize a person's face by comparing it to a pre-existing database of faces and identifying the closest match. We use the AT&T face dataset, which contains grayscale images of 40 subjects, with 10 images per subject.
Dataset

    AT&T Face Dataset: The dataset consists of grayscale images with dimensions 92x112, organized into 40 directories (one for each subject). Each directory contains ten images of the subject taken under varying conditions (lighting, facial expressions, etc.). The dataset can be downloaded from here.

Steps to Complete the Project
1. Load Dataset and Split into Training and Test Sets

    Data Loading: Load the images from the dataset and organize them into a format suitable for processing.
    Train-Test Split: Divide the dataset into training and testing sets to evaluate the performance of the face recognition system.

2. Implement PCA Algorithm from Scratch

    PCA Implementation: Implement the PCA algorithm to reduce the dimensionality of the face images and find the principal components (Eigenfaces).

3. Image Reconstruction using Eigen Projections

    Reconstruction: Reconstruct the images using the eigen projections and visualize the differences for different numbers of principal components.

4. Visualize the Mean Face (Eigenface)

    Mean Face: Calculate and visualize the mean face generated from the dataset.

5. Face Recognition Module

    Recognition Accuracy: Implement a face recognition module to identify the closest match from the training set for a given test image. Evaluate the accuracy for different numbers of principal components.

Prerequisites

    Python 3.x
    Required Libraries: numpy, scipy, matplotlib, opencv-python

Instructions

    Clone the Repository:

    sh

git clone <repository_url>
cd <repository_directory>

Install Dependencies:

sh

pip install -r requirements.txt

Download Dataset:

    Download the AT&T face dataset from the provided link and place it in the data directory.

Run Data Loading and Preprocessing:

    Load and preprocess the dataset.

sh

python data_preprocessing.py

Implement PCA:

    Implement the PCA algorithm from scratch.

sh

python pca_implementation.py

Image Reconstruction and Visualization:

    Reconstruct images using different numbers of principal components and visualize the results.

sh

python image_reconstruction.py

Face Recognition Module:

    Implement the face recognition module and evaluate accuracy.

sh

python face_recognition.py
