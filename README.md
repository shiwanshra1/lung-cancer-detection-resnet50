# Lung Cancer Detection using ResNet50

This project focuses on detecting lung cancer from medical images using a pre-trained ResNet50 Convolutional Neural Network (CNN). The dataset used for this task includes CT scans of patients diagnosed with lung cancer, classified into benign, malignant, and normal cases.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Preprocessing](#preprocessing)
- [Training the Model](#training-the-model)
- [Evaluation](#evaluation)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Lung cancer is one of the leading causes of cancer-related deaths globally. Early detection plays a critical role in reducing mortality rates. This project leverages deep learning techniques, specifically the ResNet50 model, to classify lung cancer images into three categories: benign, malignant, and normal. 

## Dataset
We used the [IQ-OTH/NCCD Lung Cancer Dataset](https://www.kaggle.com/datasets/hamdallak/the-iqothnccd-lung-cancer-dataset), which contains CT scan images categorized into three classes:
- Benign
- Malignant
- Normal

To augment the dataset, various image preprocessing techniques like rotation, flipping, and scaling were applied.

## Model Architecture
The ResNet50 architecture is known for its deep layers and the use of residual blocks to solve vanishing gradient problems. In this project, the pre-trained ResNet50 model is fine-tuned to classify medical images into the three categories. A custom classifier layer is added at the end for classification.

## Preprocessing
Images are resized to 224x224 pixels and normalized for optimal performance. Data augmentation techniques such as flipping, zooming, and rotation are applied to improve the model's generalization and reduce overfitting.

## Training the Model
The model is trained using the following configurations:
- **Optimizer**: Adam
- **Loss Function**: Categorical Crossentropy
- **Batch Size**: 32
- **Epochs**: 20-50 (based on experimentation)

## Evaluation
The model is evaluated using several metrics including:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

These metrics help understand the classification performance across different categories.

## Installation
To run this project locally, follow these steps:

1. Clone this repository:
    ```bash
    git clone https://github.com/shiwanshra1/lung-cancer-detection-resnet50.git
    ```

2. Navigate to the project directory:
    ```bash
    cd lung-cancer-detection-resnet50
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
To start training the model:
1. Ensure that the dataset is downloaded and placed in the appropriate folder as specified in the code.
2. Run the notebook or Python scripts in the repository to train and evaluate the model.

## Results
The ResNet50 model demonstrated high accuracy and precision in classifying lung cancer images, with detailed results available in the notebook.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request with any improvements or fixes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
