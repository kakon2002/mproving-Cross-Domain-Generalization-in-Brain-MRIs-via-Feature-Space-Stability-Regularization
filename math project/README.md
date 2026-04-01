# Math Project: Feature Space Stability Regularization for Brain MRI Cross-Domain Generalization

This project implements mathematical analysis and data processing for improving cross-domain generalization in brain MRI classification using feature space stability regularization.

## Overview

The script `main.py` performs comprehensive data auditing and preparation for two brain MRI datasets:
- **Kaggle MRI Dataset**: A collection of brain MRI images organized by splits (training/validation/testing) and classes
- **BRISC-2025 Dataset**: Another brain MRI dataset for classification tasks

The goal is to enhance model performance across different domains (e.g., different MRI scanners, protocols) by ensuring stability in the feature space during training.

## Features

- **Dataset Auditing**: Detailed analysis of dataset structure, class distributions, and file formats
- **Data Extraction**: Automated extraction of compressed datasets to local directories
- **Path Verification**: Robust checking of dataset paths and write permissions
- **Cross-Platform Compatibility**: Designed to work in Google Colab environment with Drive integration

## Prerequisites

- Python 3.7+
- Google Colab (recommended) or local Python environment with access to dataset paths
- Required Python packages:
  - `pathlib` (built-in)
  - `zipfile` (built-in)
  - `collections` (built-in)
  - `datetime` (built-in)
  - `google.colab` (for Colab environment)

## Dataset Setup

1. **Kaggle MRI Dataset**:
   - Download the dataset zip file
   - Place it at: `/content/drive/MyDrive/project dataset/kaggle MRI.zip` (Colab) or update `KAGGLE_ZIP` path

2. **BRISC-2025 Dataset**:
   - Download and extract the BRISC-2025 dataset
   - Place it at: `/content/drive/MyDrive/project dataset/brisc_2025` (Colab) or update `BRISC_ROOT` path

3. **Output Directory**:
   - Set `SAVE_ROOT` to your desired output location (default: `/content/drive/MyDrive/project dataset/outputs_fssr/`)

## Usage

1. Open `main.py` in Google Colab or your Python environment
2. Update the dataset paths if necessary
3. Run the script:

```python
python main.py
```

The script will:
- Verify environment and paths
- Audit the Kaggle MRI dataset structure
- Extract the Kaggle dataset to local storage
- Analyze the BRISC-2025 dataset
- Prepare data for further processing

## Output

The script generates:
- Detailed dataset statistics (class counts, file extensions, splits)
- Extracted datasets in local directories
- Verification of data integrity and accessibility

## Project Structure

```
math project/
├── main.py              # Main data processing and auditing script
└── README.md           # This file
```

## Contributing

This is part of a larger research project on cross-domain generalization in medical imaging. For contributions or questions, please refer to the main project repository.

## License

[Add appropriate license information]

## Citation

If you use this code in your research, please cite:

[Add citation information when available]