# 🩺 Skin Disease Classification Using Deep Learning and Hybrid CNN Feature Fusion

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Research-red)
[![Dataset](https://img.shields.io/badge/Dataset-Download-blue?logo=google-drive)](https://www.kaggle.com/datasets/chayanmondalabir/citrus-leaf-pathology-multi-class-image-dataset)

### Deep Learning Framework for Citrus Skin Disease Detection 

<img src="Image/AI-Powered Skin Disease Classification Infographic.png" alt="Lemon Leaf Disease Dataset" width="700">

</div>

## 📌 Overview

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

## 🧠 Proposed Method

The proposed hybrid architecture uses three pretrained CNN models as feature extractors:

1. **MobileNetV2** – extracts compact visual representations.
2. **InceptionResNetV2** – captures multi-scale visual features.
3. **DenseNet169** – learns rich feature representations through dense connectivity.

The extracted features are fused and passed through fully connected layers. Configurations with 1, 2, 3, and 4 dense layers are investigated.

**Workflow:**

<img src="Image/proposed model .png" alt="Lemon Leaf Disease Dataset" width="700">



`Input Images → Preprocessing → CNN Feature Extraction → Feature Fusion → Dense Layers → Classification`

## 🗂️ Datasets

The experiments use two datasets:

- **Skin-Disease-Dataset (SDD):** A local dataset used in this study.
[Available on Kaggle Repo Link] (https://www.kaggle.com/datasets/subirbiswas19/skin-disease-dataset).
  
- **HAM10000:** A publicly available dermatoscopic image dataset.
 [Available Link ](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T)
## 📊 Experimental Results

The proposed hybrid model with two dense layers achieved the following classification accuracies:

| Dataset | Accuracy |
|---|---:|
| Skin-Disease-Dataset (SDD) | 97.00% |
| HAM10000 | 89.78% |

These results indicate the potential of hybrid CNN feature fusion for skin disease image classification.

> **Note:** Reported accuracy values are from the research experiments. Results may vary depending on data preprocessing, dataset splits, random seeds, and training configuration.

## 📁 Repository Structure

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

*The structure above will be added upto publish the research paper.*

## 🛠️ Technologies

- Python
- TensorFlow / Keras
- Convolutional Neural Networks (CNNs)
- Transfer Learning
- Computer Vision
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/subirbiswas192001/skin-disease-classification-deep-learning.git
cd skin-disease-classification-deep-learning
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

# 🚀 Usage

Once the implementation files and datasets are available, follow the instructions in the relevant notebook or script to:

1. Prepare and preprocess the images.
2. Train and evaluate the individual CNN architectures.
3. Extract and fuse features using MobileNetV2, InceptionResNetV2, and DenseNet169.
4. Compare the dense-layer configurations.
5. Evaluate the trained models using appropriate classification metrics.

Detailed execution commands and dataset preparation instructions will be added alongside the implementation.

## 📈 Results and Visualizations

- Model architecture diagram
- Accuracy and loss curves
- CNN model comparison
- Confusion matrices
- Class-wise precision, recall, and F1-score

### 🔬 Research Contributions

The major contributions of this research include:

- Comparative evaluation of multiple state-of-the-art CNN architectures for skin disease classification.
- Development of a hybrid feature-fusion architecture integrating MobileNetV2, InceptionResNetV2, and DenseNet169.
- Investigation of different dense-layer configurations for improved feature representation and classification.
- Experimental evaluation using both a local skin disease dataset and the publicly available HAM10000 dataset.
- Exploration of deep learning approaches for automated medical image analysis.

## ⚠️ Disclaimer

This project is intended for academic and research purposes only. It is not a clinically validated diagnostic system and must not be used as a substitute for professional medical advice, diagnosis, or treatment. Any clinical application requires appropriate validation and oversight by qualified healthcare professionals.

## 📚 Citation

If you use this repository, its implementation, or the proposed methodology in your research, please cite the original publication.

Research Paper Details

Title: To be updated.

Authors: To be updated.

Journal/Conference: To be updated.

DOI: To be updated.

The complete citation will be provided following publication of the research paper.

## 🔎 Keywords

Deep Learning · Skin Disease Classification · Skin Cancer Detection · CNN · MobileNetV2 · InceptionResNetV2 · DenseNet169 · Feature Fusion · Transfer Learning · Medical Image Analysis

<div align="center">

🌟 Advancing AI for Better Healthcare

Research • Deep Learning • Medical Image Analysis • Reproducible Science

If you find this research useful, consider giving this repository a ⭐ on GitHub.

</div>
