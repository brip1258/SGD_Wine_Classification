# Wine Classification Using SGD Classifiers

This project explores the use of Stochastic Gradient Descent (SGD) classifiers for multi-class classification of wine types based on their chemical properties. The goal is to apply and evaluate the performance of SGD-based models on a wine dataset stored in Parquet format, classifying wine into distinct categories.

## Dataset

The dataset used in this project is text-based and was provided by the course instructor. Due to its proprietary nature, the dataset is not available publicly. The dataset contains review_text from sommelier including:
- Flavor
- Color
- Smell

The target variable is the wine class, with multiple categories representing different types of wine (e.g.Cabernet Sauvignon, Chardonnay, Merlot, Pinot Noir, Riesling, Sauvignon Blanc, Syrah, Zinfandel).

## Model

The model is built using the **SGDClassifier** from `sklearn`, which is a linear classifier optimized for large-scale learning tasks. The classifier is configured with:
- **Loss function**: Hinge (for SVM-like classification) or log (for logistic regression).
- **Penalty**: L2 regularization (Ridge).
- **Max iterations**: 1000 (with early stopping).

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/wine-classification-sgd.git
   cd wine-classification-sgd
   ```
