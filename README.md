# Brain Decoding with Haxby Dataset

This project demonstrates a simple **brain decoding** approach using fMRI data from the **Haxby 2001 dataset**. The goal is to classify brain activity patterns associated with viewing **faces vs. houses** using **machine learning**.

## 🚀 Project Overview

- **Dataset:** Haxby 2001 fMRI dataset (subject 1)
- **Tech Stack:** Python, Jupyter Notebook, Nilearn, Scikit-learn, NumPy, Matplotlib
- **Goal:** Predict visual stimuli (faces vs. houses) based on brain activity
- **Methods:** Feature extraction with **PCA**, classification using **Logistic Regression**, and **brain activation mapping**

## 📂 Dataset Details

The Haxby dataset is a publicly available fMRI dataset where subjects viewed images of different categories (faces, houses, cats, bottles, etc.). This project focuses on distinguishing between **faces** and **houses**.

- Functional MRI data: `func` (4D NIfTI images)
- Labels (stimuli categories): `session_target`
- Brain mask (ventral temporal region): `mask_vt`
- Anatomical image: `anat`

## 📜 Installation

To run this project, you need Python 3.7+ and the following dependencies:

```bash
pip install numpy matplotlib scikit-learn nilearn jupyter
```

## 🏗️ How to Run

1. Launch Jupyter Notebook:

```bash
jupyter notebook
```

2. Open the `brain_decoding.ipynb` notebook and run the cells step by step.

## 🔬 Workflow

1. **Download** the Haxby dataset
2. **Preprocess**: Extract fMRI signals and apply a brain mask
3. **Feature Engineering**: Reduce dimensionality using PCA
4. **Train a classifier**: Use logistic regression to predict face vs. house
5. **Evaluate model performance**: Accuracy & cross-validation
6. **Visualize brain regions** that contribute to classification
7. **Visualize time series** of a voxel and performing Fourier Transform
8. **Comparing different classifiers**

## 📊 Results

- **Test Accuracy:** \~80-90% (may vary by run)
- **Cross-Validation Accuracy:** Consistent performance across folds
- **Brain Activation Map:** Highlights key areas used for decoding

## 📷 Example Visualization

The following figure shows the **brain regions most predictive of faces vs. houses**:



## 🎯 Future Improvements

- Extend classification to **all image categories** (not just faces & houses)
- Use **Deep Learning (CNNs or RNNs)** for improved accuracy
- Implement **time-series analysis** of fMRI data

## 📖 References

- Haxby et al. (2001) **Distributed and Overlapping Representations of Faces and Objects in Ventral Temporal Cortex**
- [Nilearn Documentation](https://nilearn.github.io/)

---

🚀 **Built for demonstrating neuroimaging & machine learning techniques in Jupyter Notebook**

