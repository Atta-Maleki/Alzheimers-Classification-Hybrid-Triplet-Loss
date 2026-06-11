# Alzheimer's Disease Classification using Hybrid Distance Triplet Loss

This repository contains the official implementation of the methodology described in our paper: **"Automated Alzheimer's Disease Classification Using a Hybrid Distance Triplet Loss in Feature Embedding Space"**.

## Abstract
This project presents a novel approach to Alzheimer's disease (AD) classification using MRI images. We propose a Feature Embedding Network (FEN) designed to extract and refine discriminative features. The FEN incorporates a hybrid distance function—integrating Euclidean distance, cosine similarity, and Earth Mover's Distance—to capture nuanced differences in brain structure indicative of AD progression. Through a triplet loss framework, our model optimizes embeddings to cluster similar images while separating dissimilar ones, achieving 94.89% accuracy on the test set.

## Methodology
The methodology leverages a Triplet Network architecture with a MobileNetV2 backbone for feature extraction. Key features include:
* **Hybrid Distance Metric:** Integration of Euclidean, Cosine, and EMD metrics for robust feature comparison.
* **Triplet Loss Framework:** Training to optimize the embeddings of anchor, positive, and negative examples.
* **Robust Classification:** Enhanced clustering of similar brain structure images indicative of AD progression.

## Repository Structure
* `Paper2_TripletLoss_Github.ipynb`: The primary Jupyter notebook containing the full pipeline:
    * **Data Loading & Preprocessing:** Handles image data and sanity checks.
    * **Model Architecture:** Construction of the Triplet Network and L2 normalization.
    * **Training:** Model compilation and triplet training.
    * **Evaluation:** Embedding extraction, classifier training, and performance visualization.

## Getting Started
To run the code provided in `Paper2_TripletLoss_Github.ipynb`, ensure you have the following environment and data requirements:

1.  **Environment:** A Google Colab environment is recommended, as the notebook is pre-configured for Google Drive integration.
2.  **Dependencies:** Ensure `tensorflow`, `numpy`, `matplotlib`, `imblearn`, and `scikit-learn` are installed.
3.  **Data:** The code expects preprocessed image data (e.g., `trainImages.npy`, `trainLabels.npy`) stored in your Google Drive under the path `/content/drive/MyDrive/OASIS_P/pre/`[Download From Kaggle : https://www.kaggle.com/].

## Citation
If you use this code or our methodology in your research, please cite our paper:

```bibtex
@inproceedings{maleki2025automated,
  title={Automated Alzheimer's Disease Classification Using a Hybrid Distance Triplet Loss in Feature Embedding Space},
  author={Maleki, Atta and Zomorodi, Mariam and P{\l}awiak, Pawe{\l}},
  booktitle={Proceedings of the 2025 18th International Conference on Computer Science and Information Technology},
  pages={226--232},
  year={2025}
}
