# Disease Prediction System

A machine learning system that predicts diseases based on symptoms. Compares four ML algorithms and selects the best prediction across all models.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TanaySasane/Disease-Prediction-System/blob/main/main.ipynb)

## Overview

- Predicts **41 diseases** from **132 symptoms**
- Trained on **4920 samples**
- Achieves **100% accuracy** on test data
- Compares 4 ML algorithms side by side

## Models Used

| Model | Type |
|---|---|
| Multinomial Naive Bayes | Probabilistic |
| Decision Tree | Tree-based |
| Random Forest | Ensemble |
| Gradient Boosting | Ensemble |

## Tech Stack

- Python 3.x
- Scikit-learn
- Pandas
- Jupyter Notebook
- PyYAML
- Joblib

## Run on Google Colab (no setup needed)

Click the badge above or go to:
[colab.research.google.com](https://colab.research.google.com) → File → Open Notebook → GitHub → paste this repo URL

The first cell in the notebook handles cloning and installing dependencies automatically.

## Run Locally

```bash
git clone https://github.com/TanaySasane/Disease-Prediction-System.git
cd Disease-Prediction-System
pip install scikit-learn pandas pyyaml seaborn matplotlib Pillow joblib
jupyter notebook main.ipynb
```

## Project Structure

```
├── main.ipynb               # Main notebook — training + evaluation
├── config.yaml              # Model and dataset configuration
├── training_data.csv        # Training dataset (4920 samples, 132 features)
├── test_data.csv            # Test dataset (42 samples)
└── saved_model*.joblib      # Pre-trained model files
```

## Dataset

- 132 symptom features (binary: present/absent)
- 41 disease classes
- Source: Symptom-disease mapping dataset
