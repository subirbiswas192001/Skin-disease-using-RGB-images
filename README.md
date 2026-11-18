# Skin Disease Classification Using Deep Learning and Hybrid CNN Feature Fusion

## Overview

Skin cancer and other skin disorders present significant global healthcare challenges. Early and accurate diagnosis is important for improving patient outcomes. This project investigates deep learning techniques for the automated classification of eight different skin disorders using convolutional neural networks (CNNs).

The study evaluates several CNN architectures:

- VGG16
- Xception
- NASNetLarge
- EfficientNetB7
- MobileNetV2
- InceptionResNetV2
- DenseNet169

In addition, a hybrid feature-fusion model is proposed. It combines features extracted from MobileNetV2, InceptionResNetV2, and DenseNet169. The fused representation is passed through different configurations of fully connected dense layers to evaluate classification performance.

## Proposed Method

The proposed hybrid architecture uses three pretrained CNN models as feature extractors:

1. **MobileNetV2** – extracts compact visual representations.
2. **InceptionResNetV2** – captures multi-scale visual features.
3. **DenseNet169** – learns rich feature representations through dense connectivity.

The extracted features are fused and passed through fully connected layers. Configurations with 1, 2, 3, and 4 dense layers are investigated.

**Workflow:**

`Input Images → Preprocessing → CNN Feature Extraction → Feature Fusion → Dense Layers → Classification`

## Datasets

The experiments use two datasets:

- **Skin-Disease-Dataset (SDD):** A local dataset used in this study.
- **HAM10000:** A publicly available dermatoscopic image dataset.

Please obtain each dataset from its authorized source and follow its license and usage conditions. Dataset files are not included in this repository unless explicitly stated.

## Experimental Results

The proposed hybrid model with two dense layers achieved the following classification accuracies:

| Dataset | Accuracy |
|---|---:|
| Skin-Disease-Dataset (SDD) | 97.00% |
| HAM10000 | 89.78% |

These results indicate the potential of hybrid CNN feature fusion for skin disease image classification.

> **Note:** Reported accuracy values are from the research experiments. Results may vary depending on data preprocessing, dataset splits, random seeds, and training configuration.

## Repository Structure

```text
skin-disease-classification-deep-learning/
├── README.md
├── requirements.txt
├── notebooks/
│   ├── data_preprocessing.ipynb
│   ├── individual_cnn_models.ipynb
│   └── hybrid_fusion_model.ipynb
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   ├── evaluate.py
│   └── hybrid_model.py
├── figures/
│   └── model_architecture.png
├── results/
│   ├── accuracy_comparison.png
│   ├── confusion_matrix.png
│   └── training_curves.png
└── docs/
    └── methodology.md
```

*The structure above is a suggested layout. Remove entries for files that are not yet included in the repository.*

## Technologies

- Python
- TensorFlow / Keras
- Convolutional Neural Networks (CNNs)
- Transfer Learning
- Computer Vision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/skin-disease-classification-deep-learning.git
cd skin-disease-classification-deep-learning
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Replace `YOUR_USERNAME` with your GitHub username. Make sure `requirements.txt` is included and lists the dependencies required by the implementation.

## Usage

Once the implementation files and datasets are available, follow the instructions in the relevant notebook or script to:

1. Prepare and preprocess the images.
2. Train and evaluate the individual CNN architectures.
3. Extract and fuse features using MobileNetV2, InceptionResNetV2, and DenseNet169.
4. Compare the dense-layer configurations.
5. Evaluate the trained models using appropriate classification metrics.

Detailed execution commands and dataset preparation instructions will be added alongside the implementation.

## Results and Visualizations

The following visualizations can be added to this section when available:

- Model architecture diagram
- Accuracy and loss curves
- CNN model comparison
- Confusion matrices
- Class-wise precision, recall, and F1-score

## Reproducibility

To support reproducibility, the repository should include the data preprocessing procedure, model configurations, training settings, evaluation scripts, and dataset split details. Any reported results should be interpreted in the context of the experimental setup.

## Disclaimer

This project is intended for academic and research purposes only. It is not a clinically validated diagnostic system and must not be used as a substitute for professional medical advice, diagnosis, or treatment. Any clinical application requires appropriate validation and oversight by qualified healthcare professionals.

## Citation

If you use this work, please cite the original research publication.

**Paper title:** To be added  
**Authors:** To be added  
**Journal / Conference:** To be added  
**DOI:** To be added

## Keywords

Deep Learning · Skin Disease Classification · Skin Cancer Detection · CNN · MobileNetV2 · InceptionResNetV2 · DenseNet169 · Feature Fusion · Transfer Learning · Medical Image Analysis
