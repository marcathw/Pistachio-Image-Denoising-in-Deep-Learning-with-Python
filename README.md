# 🌰 Pistachio Image Denoising and Quality Enhancement with Autoencoders

This project focuses on building and evaluating deep learning autoencoder models to denoise and improve the visual quality of **pistachio images**. It details a robust pipeline from initial data exploration and preprocessing to advanced model architectures and training strategies.

---

## 🔗 Dataset Access

[![Download Dataset](https://img.shields.io/badge/Download%20Dataset-003366?style=for-the-badge)](https://drive.google.com/file/d/11PltRpmCYG3xc8T8MsHyRxuLzhHsAJX0/view?usp=sharing)

---

## 🔧 Features

* **Comprehensive Pistachio Image Data Analysis (EDA)**
    * Detection of corrupted, duplicated, and low-quality (blurry) pistachio images.
    * Detailed analysis of pistachio image resolution, aspect ratio, data types, file formats, color channels, brightness, contrast, and color distribution.
* **Advanced Image Preprocessing**
    * Automated removal of identified blurry images for improved training data quality.
    * Data splitting into train, validation, and test sets for the pistachio dataset.
    * Essential image transformations including resizing, normalization, and controlled **Gaussian noise** injection for denoising task preparation.
* **Deep Learning Autoencoder Architectures**
    * Implementation and evaluation of a **Baseline Convolutional Autoencoder**.
    * Development of a **Modified U-Net inspired Autoencoder** incorporating deeper convolutional layers, **Dropout** for regularization, and **skip connections** for enhanced detail preservation.
* **Optimized Model Training**
    * Training conducted over extended epochs (up to 200) with **EarlyStopping** to prevent overfitting and achieve optimal model convergence.
* **Rigorous Model Evaluation**
    * Quantitative assessment using the **Structural Similarity Index (SSIM)** to measure reconstruction quality against original images.
    * Qualitative visual analysis of denoised images to identify improvements in sharpness and fine detail recovery.

---

## 🧠 Concepts Used

* **Image Denoising**: The process of recovering clean images from noisy inputs.
* **Convolutional Autoencoders**: Neural networks designed for unsupervised feature learning and dimensionality reduction, particularly effective for image data reconstruction.
* **U-Net Architecture**: A specialized convolutional network renowned for its effectiveness in image-to-image translation tasks, leveraged here for its ability to preserve spatial details through **skip connections**.
* **Data Preprocessing**: Fundamental steps to prepare raw image data for effective deep learning model training.
* **Gaussian Noise**: A common type of additive noise used to simulate real-world imperfections in images and train models for noise reduction.
* **Early Stopping**: A powerful regularization technique that prevents model overfitting by halting training when performance on a validation set no longer improves.
* **Structural Similarity Index (SSIM)**: A perception-based metric that provides a more accurate measure of image quality degradation than traditional pixel-difference metrics, focusing on structure, luminance, and contrast.
