# Predicting Leukemia Subtypes Using Gene Expression Profiles and Deep Learning

## Overview

This project applies **machine learning** and **deep learning** techniques to gene expression data to predict leukemia subtypes (ALL vs. AML). By leveraging principal component analysis (PCA) for dimensionality reduction and neural networks for classification, the notebook demonstrates a reproducible pipeline for biomedical data exploration and disease subtype prediction.

---

## Table of Contents

- [Project Objective](#project-objective)
- [Dataset Description](#dataset-description)
- [Environment & Dependencies](#environment--dependencies)
- [Methodology](#methodology)
- [Key Results](#key-results)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)
- [References](#references)

---

## Project Objective

- Predict and classify **leukemia subtypes** (Acute Lymphoblastic Leukemia - ALL and Acute Myeloid Leukemia - AML) using gene expression profiles.
- Develop a reproducible machine learning pipeline for biomedical data analysis.

---

## Dataset Description

- **Source**: Affymetrix microarray gene expression profiles.
- **Samples**: Patient data labeled as 'ALL' (47 cases) and 'AML' (25 cases).
- **Features**: 
  - Gene expression values for 7,129 genes (columns include gene names such as `AFFX-BioB-5_at`).
  - Patient metadata including sample IDs and cancer type labels.

---

## Environment & Dependencies

- **Language**: Python 3.6.4
- **Key Libraries**:
  - `numpy`, `pandas`
  - `scikit-learn`
  - `tensorflow`/`keras`
  - `matplotlib`, `seaborn`
- **Platform**: Compatible with Google Colab (supports `google.colab.drive.mount` for accessing files on Google Drive)

---

## Methodology

1. **Data Loading**
   - Reads the gene expression data and associated patient labels from `actual.csv`.
   
2. **Preprocessing**
   - Normalizes features using `StandardScaler`.
   - Applies **Principal Component Analysis (PCA)** to reduce dimensionality for visualization and improved model input.

3. **Model Development**
   - Uses the Tensorflow/Keras API to build a neural network classifier.
   - Trains the model on gene expression patterns to distinguish between ALL and AML subtypes.

4. **Evaluation**
   - Assesses performance via accuracy and confusion matrix.
   - Uses train/test splits for robust evaluation.

---

## Key Results

- The pipeline demonstrates high accuracy in distinguishing between ALL and AML using the selected gene expression features.
- Visualization and classification results highlight distinct gene expression patterns between the subtypes.

---

## Visualizations

- **3D PCA plots** to show class separation.
- **Confusion matrices** and **heatmaps** to summarize classification outcomes.

---

## How to Run

1. **Clone the Repository**
