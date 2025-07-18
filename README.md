# Melanoma Detection using Deep Learning

This repository contains Jupyter Notebooks demonstrating the application of various deep learning architectures for the classification of melanoma (skin cancer) from images. The project explores the effectiveness of EfficientNet, ResNet-18, VGG-16, and Vision Transformer models on a melanoma dataset.

## Table of Contents

* Project Overview

* Dataset

* Models Implemented

* Installation

* Usage

* Results

* Contributing

* License

## Project Overview

Melanoma is a serious form of skin cancer. Early detection is crucial for successful treatment. This project aims to build and compare several deep learning models for accurate classification of skin lesions as either benign or malignant. The goal is to identify which architecture performs best on the given dataset, providing a foundation for potential clinical applications.

## Dataset

The dataset used in this project is the "[Melanoma Cancer Dataset](https://www.kaggle.com/datasets/bhaveshmittal/melanoma-cancer-dataset)" available on Kaggle. It contains images categorized into 'Benign' and 'Malignant' classes.
* **Source:** Kaggle: Melanoma Cancer Dataset (Please ensure you have access to this dataset or download it as instructed in the notebooks).

The notebooks include steps to download and extract this dataset.

## Models Implemented

The following deep learning architectures have been implemented and evaluated:

1. **EfficientNet:** (`EfficientNetMelanomaDetection.ipynb`)

   * A family of models that scale neural networks more efficiently, achieving better accuracy with fewer parameters.

2. **ResNet-18:** (`ResNet_18MelanomaDetection.ipynb`)

   * A Residual Network with 18 layers, known for its ability to train very deep networks by using skip connections to combat the vanishing gradient problem.

3. **VGG-16:** (`VGG_16MelanomaDetection.ipynb`)

   * A classic convolutional neural network with 16 layers, characterized by its simple and uniform architecture using 3x3 convolutional filters.

4. **Vision Transformer (ViT):** (`VisionTransformerMelanomaDetection.ipynb`)

   * An innovative model that applies the Transformer architecture, originally designed for natural language processing, directly to images.

## Installation

To run these notebooks, you'll need to set up a Python environment with the necessary libraries.

1. **Clone the repository:**

git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
cd YOUR_REPOSITORY_NAME


(Replace `YOUR_USERNAME` and `YOUR_REPOSITORY_NAME` with your actual GitHub details.)

2. **Install dependencies:**
The notebooks use `pip` to install required packages. You can install them manually or run the first cell of each notebook.

pip install kaggle torch torchvision numpy matplotlib seaborn shap lime opencv-python datasets transformers


*Note: Some packages might have specific versions or dependencies. Refer to the `!pip install` commands in each notebook for exact requirements.*

3. **Kaggle API Key:**
To download the dataset, you'll need a Kaggle API key.

* Go to your Kaggle account settings (`https://www.kaggle.com/<YOUR-KAGGLE-USERNAME>/account`).

* Under the "API" section, click "Create New API Token" to download `kaggle.json`.

* Upload this `kaggle.json` file to your Colab environment (as shown in the notebooks) or place it in `~/.kaggle/` on your local machine.

* Ensure the permissions are set correctly: `chmod 600 ~/.kaggle/kaggle.json`.

## Usage

Each notebook (`.ipynb` file) can be opened and run in Google Colab, Jupyter Lab, or Jupyter Notebook.

1. **Open the desired notebook:**

* **Google Colab:** Upload the notebook directly to Colab or open it from GitHub.

* **Local Jupyter:** Navigate to the repository directory in your terminal and run `jupyter notebook` or `jupyter lab`.

2. **Run all cells:** Execute the cells sequentially to download the dataset, preprocess images, define and train the models, and evaluate their performance.

## Results

Each notebook provides detailed training logs, evaluation metrics (e.g., accuracy, precision, recall, F1-score), and visualizations (e.g., confusion matrices, ROC curves). The performance of each model on the melanoma classification task can be compared to determine the most effective approach.

*Further details on specific model performance can be found within each respective notebook.*

## Contributing

Contributions are welcome! If you have suggestions for improvements, new model implementations, or bug fixes, please open an issue or submit a pull request.

## License

This project is open-sourced under the MIT License. This project is open-sourced under the MIT License. See the `LICENSE` file for more details.
