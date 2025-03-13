# Dataset Information for SSWIN-AD Alzheimer’s Classification

## Source:
This project utilizes MRI scans from the Alzheimer's Disease Neuroimaging Initiative (ADNI) dataset.

### Dataset Classes:
- CN: Cognitively Normal
- EMCI: Early Mild Cognitive Impairment
- LMCI: Late Mild Cognitive Impairment
- AD: Alzheimer’s Disease

## Dataset Structure:
datasets/ ├── train/ │ ├── CN/ │ ├── EMCI/ │ ├── LMCI/ │ └── AD/ └── test/ ├── CN/ ├── EMCI/ ├── LMCI/ └── AD/

## Steps to Download and Prepare Data:
1. Obtain access to ADNI database from [ADNI](https://adni.loni.usc.edu/).
2. Download MRI scans under the standardized protocol.
3. Perform preprocessing (e.g., CLAHE, resizing) using provided scripts.
4. Split data clearly into training (70%) and testing (30%) as per our manuscript.
5. Save preprocessed images into the respective class folders as shown above.

## Preprocessing:
- Image size: `224x224 pixels`
- Enhancement technique: `Contrast Limited Adaptive Histogram Equalization (CLAHE)`
- Format: `.png` or `.jpg`

## Note:
- Due to ADNI licensing restrictions, actual MRI scans cannot be uploaded here. Users must download directly from the official source and preprocess accordingly.


