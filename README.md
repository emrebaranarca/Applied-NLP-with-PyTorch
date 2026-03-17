# Applied-NLP-with-PyTorch

This repository contains a complete **notebook-based NLP pipeline** for crisis/disaster tweet detection.
The main work is implemented in:

- `Crisis-Detection-NLP-Pipeline.ipynb`

---

## Table of Contents

- [Project Overview](#project-overview)
- [What This Project Covers](#what-this-project-covers)
- [Repository Structure](#repository-structure)
- [Dataset](#dataset)
- [Environment and Requirements](#environment-and-requirements)
- [How to Run](#how-to-run)
- [Notebook Workflow (Step-by-Step)](#notebook-workflow-step-by-step)
- [Outputs](#outputs)
- [Notes](#notes)
- [License](#license)

## Project Overview

The goal of this project is to classify social media text related to crisis/disaster events.
It follows an end-to-end practical workflow:

1. Load and inspect data
2. Clean and preprocess text
3. Build text features
4. Train and evaluate multiple baseline/deep models
5. Compare model performance
6. Generate submission-ready outputs

The notebook includes both **traditional ML** (e.g., TF-IDF + Logistic Regression) and **deep learning sequence approaches**.

## What This Project Covers

- Exploratory analysis of train/test data
- Text cleaning and normalization
- Feature engineering for NLP
- Baseline model training and evaluation
- Sequence modeling with TensorFlow/Keras preprocessing
- LSTM-based modeling with PyTorch
- Comparative model evaluation and visualization

## Repository Structure

```text
Applied-NLP-with-PyTorch/
├── Crisis-Detection-NLP-Pipeline.ipynb   # Main end-to-end notebook
├── README.md                             # Project documentation
└── LICENSE                               # Apache License 2.0
```

## Dataset

The notebook references Kaggle paths from the NLP Getting Started competition:

- `/kaggle/input/competitions/nlp-getting-started/train.csv`
- `/kaggle/input/competitions/nlp-getting-started/test.csv`

If you run locally (outside Kaggle), download the dataset and update file paths in the notebook cells accordingly.

## Environment and Requirements

- Python 3.8+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- nltk
- torch
- tensorflow
- transformers

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk torch tensorflow transformers
```

## How to Run

1. Open the notebook:
   - `Crisis-Detection-NLP-Pipeline.ipynb`
2. Run cells in order from top to bottom.
3. If you are not on Kaggle:
   - Replace Kaggle input paths with your local dataset paths.
4. Review metrics/plots and generated outputs (including submission file paths used in the notebook).

## Notebook Workflow (Step-by-Step)

The notebook is organized into practical sections (comments/titles inside code cells), including:

1. **Data loading**
   - Read train/test CSV files
   - Preview columns and examples

2. **EDA and target inspection**
   - Dataset shape checks
   - Target distribution summaries
   - Visual plots

3. **Text preprocessing**
   - Regex-based cleaning
   - Token-level transformations and normalization

4. **Feature engineering**
   - TF-IDF vectorization
   - Train/validation split

5. **Baseline model(s)**
   - Logistic Regression with TF-IDF
   - Evaluation with classification metrics and confusion matrix

6. **Sequence preparation**
   - Keras tokenizer usage
   - Sequence conversion and padding

7. **Deep learning models**
   - LSTM (PyTorch)
   - Bidirectional LSTM (PyTorch)

8. **Model comparison**
   - Performance comparison and visual analysis

## Outputs

The notebook includes code to create prediction outputs and references paths such as:

- `/kaggle/working/submission.csv`

When running locally, adjust output directories as needed.

## Notes

- This repository is notebook-first and does not currently include separate package, CI, or test infrastructure.
- For reproducibility, keep package versions fixed in your environment where possible.

## License

This project is licensed under the Apache License 2.0. See `LICENSE` for details.
