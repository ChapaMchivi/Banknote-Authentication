# Banknote Authentication with Clustering & PCA

> **Unsupervised learning meets fraud detection — clustering banknotes with PCA and OpenML.**
> **Modular, reproducible clustering pipeline for banknote authentication — built for clarity and impact.**

![Python](https://img.shields.io/badge/Python-3.13-blue.svg)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.6.1-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Portfolio--Ready-brightgreen.svg)

This project applies unsupervised learning techniques to explore patterns in banknote authentication data. Using dimensionality reduction and clustering, it reveals structure in the data without relying on labels — ideal for anomaly detection and fraud analysis.

## 📊 Project Highlights

-  Cleaned and visualized OpenML banknote dataset
-  Applied PCA and K-Means clustering with silhouette scoring
-  Modular pipeline with reusable functions and centralized paths
-  Visualizations saved to structured folders for portfolio review
-  GitHub-integrated and reproducible with requirements.txt

## 📁 Dataset Reference

**Dataset Title:** [Banknote Authentication](https://www.openml.org/search?type=data&status=active&id=1462)  
**Author:** Volker Lohweg (University of Applied Sciences, Ostwestfalen-Lippe)  
**Source:** UCI Machine Learning Repository (2012)  
**Citation:** Please cite the UCI repository when using this dataset.

### 📄 Description

This dataset contains features extracted from images of genuine and forged banknotes. The images were digitized using an industrial camera typically used for print inspection, producing grayscale images at ~660 dpi. A Wavelet Transform was applied to extract statistical features from each image.

### 🔍 Attribute Information

| Feature | Description                                      | Type     |
|---------|--------------------------------------------------|----------|
| V1      | Variance of Wavelet Transformed image            | Numeric  |
| V2      | Skewness of Wavelet Transformed image            | Numeric  |
| V3      | Kurtosis of Wavelet Transformed image            | Numeric  |
| V4      | Entropy of image                                 | Numeric  |
| Class   | Target variable: 0 = genuine, 1 = forged          | Nominal  |

- 📌 Instances: 1,372  
- 📌 Features: 5 (4 numeric, 1 nominal)  
- 📌 Missing values: None

## 🛠️ Technologies Used

| Tool            | Purpose                          |
|-----------------|----------------------------------|
| Python          | Core programming language        |
| pandas          | Data cleaning and manipulation   |
| scikit-learn    | Clustering, PCA, scaling         |
| matplotlib      | Visualizations                   |
| openml          | Dataset retrieval                |
| Git & GitHub    | Version control and collaboration|

## 📁 Project Structure

banknote-authentication/
├── code/                         # Modular Python scripts
│   └── banknote_clustering_pipeline.py
│   └── utils/                    # Optional: helper functions (e.g., plotting, scoring)
│       └── __init__.py
│       └── visualizations.py
│       └── clustering.py
├── data/                         # Raw and processed datasets
│   └── banknote_authentication.csv
├── images/                       # Saved visual outputs
│   ├── stats/                    # Mean, std tables
│   ├── boxplots/                 # Feature distributions
│   ├── distributions/            # Histograms, density plots
│   └── clustering/               # PCA plots, K-Means results
├── notebooks/                    # Optional: exploratory Jupyter notebooks
│   └── EDA_banknote.ipynb
├── requirements.txt              # Python dependencies
├── README.md                     # Project overview and instructions
└── LICENSE                       # Optional: usage terms

## 🚀 How to Run

```bash
# Clone the repo
git clone https://github.com/ChapaMchivi/Banknote-Authentication.git
cd Banknote-Authentication

# Install dependencies
pip install -r requirements.txt


## Environment Setup

To reproduce this project, install dependencies via:

```bash
pip install -r requirements.txt


- Optionally include your Python version (e.g., `Python 3.13`) for clarity.
- If you want to lock versions even tighter, consider using a `pip-tools` workflow or `conda` environment file.

