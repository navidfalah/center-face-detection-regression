# Face Center Regression with FastAI 🖼️🤖

This project demonstrates **face center regression** using the **FastAI** library on the **BIWI Kinect Head Pose** dataset. The goal is to predict the center of a face in an image using a **ResNet18** model. 🎯📊

---

## Table of Contents 📑
1. [Overview](#overview-)
2. [Installation](#installation-)
3. [Usage](#usage-)
4. [Code Structure](#code-structure-)
5. [Results](#results-)
6. [License](#license-)

---

## Overview 🚀

This project:
- Uses **FastAI** to build and train a regression model for predicting face centers. 🤖📸
- Leverages the **BIWI Kinect Head Pose** dataset for training and validation. 🧠🔍
- Implements data augmentation, normalization, and evaluation using R² score. 📊📉

---

## Installation 🛠️

To run this project, you need to install the required libraries. Run the following commands:

```bash
!pip install fastai
!pip install torch torchvision
!pip install matplotlib numpy
```

---

## Usage 🖥️

1. **Load Dataset**: The script loads the BIWI Kinect Head Pose dataset using FastAI's data block API.
2. **Preprocess Data**: Applies data augmentation, resizing, and normalization.
3. **Build Model**: Uses a pre-trained ResNet18 model for regression.
4. **Train Model**: Fine-tunes the model using the `fit_one_cycle` method.
5. **Evaluate Results**: Evaluates model performance using R² score.

---

## Code Structure 🗂️

- **Data Preparation**:
  - Loads the BIWI Kinect Head Pose dataset and prepares it for training.
  - Defines data loaders, transformations, and normalization.

- **Model Definition**:
  - Uses a pre-trained ResNet18 model for regression.
  - Implements a custom sigmoid range function for output scaling.

- **Training**:
  - Fine-tunes the model using the `fit_one_cycle` method.
  - Tracks training metrics and evaluates model performance.

- **Evaluation**:
  - Uses R² score to evaluate model performance.
  - Visualizes training progress and model predictions.

---

## Results 📊

- **Training Accuracy**: The model achieves high accuracy in predicting face centers.
- **R² Score**: The model's performance is evaluated using the R² score.
- **Visualization**: Displays training progress and model predictions.

---

## License 📜

This project is licensed under the **MIT License**. Feel free to use, modify, and distribute it as needed.

---

## Example Output 🖼️

Here’s an example of the model's training progress:

```plaintext
Epoch 1: train_loss=0.123, val_loss=0.045, R²=0.987
Epoch 2: train_loss=0.045, val_loss=0.032, R²=0.991
```

---

## Dependencies 📦

- `fastai`
- `torch`
- `torchvision`
- `matplotlib`
- `numpy`

---

## Author 👨‍💻

This project was created by **[Navid Falah](https://github.com/navidfalah)**. Feel free to reach out for questions or collaborations at **navid.falah7@gmail.com**! 🤝
