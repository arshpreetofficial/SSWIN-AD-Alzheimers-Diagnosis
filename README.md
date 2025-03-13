# SSWIN-AD: Alzheimer's Disease Classification Using MRI Images

This repository contains the official implementation of the SSWIN-AD (Spectral Swin Transformer with Adaptive Contrast-aware Fine-Tuning) ensemble model proposed in our manuscript titled:

**"Improved Visibility of Brain Regions Using Contrast Limited Adaptive Histogram Equalization and Spectral Swin Transformer for Alzheimer’s Disease Classification on an Ensemble Deep Learning Model"**.

## 📌 Paper Information

*Authors:* Arshpreet Kaur and Jagdeep Kaur  
*Affiliation:* Department of Computer Science and Engineering, Dr. B. R. Ambedkar National Institute of Technology, Jalandhar, Punjab, India.

## 🚀 Overview

The proposed framework integrates:

- **Contrast Limited Adaptive Histogram Equalization (CLAHE)** preprocessing to enhance MRI visibility.
- **Spectral Swin Transformer (SSWIN)** for effective spectral-domain feature extraction.
- **Ensemble CNN architectures** (GoogLeNet, AlexNet, ResNet-18) optimized with Adaptive Contrast-Aware Fine-Tuning (ACaFT).

## 📁 Repository Structure

```plaintext
SSWIN-AD-Alzheimers-Diagnosis/
├── datasets/                  # Dataset preparation and instructions
├── preprocessing/             # Preprocessing scripts (CLAHE)
├── spectral_transformer/      # Spectral Swin Transformer implementation
├── models/                    # Pre-trained models and weights
│   └── pretrained_models/
│       ├── GoogLeNet/
│       ├── AlexNet/
│       └── ResNet18/
├── scripts/                   # Scripts for training, testing, evaluation
├── requirements.txt           # Required libraries
└── README.md                  # Project details
```

## 🛠️ Installation

### Requirements:
- Python 3.8+
- CUDA-enabled GPU recommended

### Installation Steps:
```bash
# Clone the repository
git clone https://github.com/your-username/SSWIN-AD-Alzheimers-Diagnosis.git
cd SSWIN-AD-Alzheimers-Diagnosis

# Install dependencies
pip install -r requirements.txt
```

## ⚙️ Quick Start

### Training Example:
```bash
python scripts/train.py --data_path datasets/ --model resnet18
```

### Evaluation Example:
```bash
python scripts/evaluate.py --model_path models/best_model.pth
```

## 📊 Results

| Dataset | Accuracy (%) | Precision (%) | Recall (%) | F1-Score (%) |
|---------|--------------|----------------|------------|--------------|
| ADNI    | 96.45 ± 1.2  | 97.50 ± 0.9   | 95.34 ± 1.0| 96.41 ± 1.1  |
| OASIS   | 95.90 ± 1.1  | 95.20 ± 1.1   | 95.60 ± 0.9| 95.40 ± 1.0  |

## 📝 Citation
Please cite our paper if you find the code or results useful:
```bibtex
@article{kaur2024sswin,
  title={Improved Visibility of Brain Regions Using Contrast Limited Adaptive Histogram Equalization and Spectral Swin Transformer for Alzheimer’s Disease Classification on an Ensemble Deep Learning Model},
  author={Kaur, Arshpreet and Kaur, Jagdeep},
  journal={Signal, Image and Video Processing},
  year={2024},
  publisher={Springer}
}
```

*(Replace citation details after paper acceptance.)*

## 📌 License
This project is licensed under the MIT License – see [LICENSE](LICENSE) for details.

## 📧 Contact

- **Corresponding Author:** Arshpreet Kaur  
  📧 Email: arshpreetk.cs.22@nitj.ac.in
