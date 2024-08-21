# Dogs vs. Cats Classification using Convolutional Neural Networks (CNN)

## Overview

This project classifies images into two categories: Dogs and Cats, using a Convolutional Neural Network (CNN). The dataset for this classification task is provided by Kaggle.

## Dataset

The dataset used is the "Dogs vs. Cats" dataset from Kaggle. It contains a total of **25,000 labeled images** of dogs and cats. The dataset is divided into the following categories:

- **Training Set**: 25,000 images, equally split between dogs and cats.
- **Test Set**: Not provided in this dataset; only the training images are included.

### Download and Setup

1. **Setup Kaggle API Credentials**:
    - Create a Kaggle account and download your API token from the [Kaggle API page](https://www.kaggle.com/account).
    - Place the `kaggle.json` file in the `.kaggle` directory:

    ```bash
    !mkdir -p ~/.kaggle
    !cp kaggle.json ~/.kaggle/
    ```

2. **Download the Dataset**:

    ```bash
    !kaggle datasets download -d salader/dogs-vs-cats
    ```

3. **Extract the Dataset**:

    ```bash
    !unzip dogs-vs-cats.zip -d data/
    ```

### Dataset Details

- **File Structure**: After extraction, the dataset is organized into a single directory with a mix of images. You may need to organize the images into separate directories for dogs and cats for ease of processing.

- **Image Details**: The images are in JPEG format, and they come in various resolutions. They are intended for training a binary classification model where each image is labeled either as a dog or a cat.

## Requirements

To run this project, you'll need:

- Python 3.x
- TensorFlow/Keras
- NumPy
- pandas
- Matplotlib
- scikit-learn
- OpenCV or PIL

Install the required libraries using pip:

```bash
pip install tensorflow numpy pandas matplotlib scikit-learn opencv-python


