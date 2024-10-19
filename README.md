# Logistic Regression Model with Categorical Encoding and Performance Evaluation

This project demonstrates how to build a **Logistic Regression** model for binary classification using Python. The workflow includes data preprocessing, categorical encoding, class imbalance handling, model training, and performance evaluation using various metrics.

## Features

- **Data Preprocessing**: Handles both categorical and numerical features using `OneHotEncoder` and `LabelEncoder`.
- **Class Imbalance**: Implements class weighting to address imbalanced datasets.
- **Logistic Regression Model**: Trained using `LogisticRegression` from Scikit-learn with class weights.
- **Model Evaluation**: Includes accuracy, F1-score, confusion matrix, ROC-AUC, Precision-Recall curve, and cross-validation.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. Install the required Python libraries:

    ```bash
    pip install -r requirements.txt
    ```

3. If you're using Google Drive to load datasets, you can use the `gdown` module to download the dataset. You can install it with:

    ```bash
    pip install gdown
    ```

## Dataset

The dataset is downloaded from Google Drive. Replace the `dataset` variable with the actual dataset ID to load the data.

```python
import gdown

dataset = '1GCmHooX1xOvyIsvdDvGrMBzmJeC4zB0D'
url = f'https://drive.google.com/uc?id={dataset}'
output_path = '/dataset.csv'
gdown.download(url, output_path, quiet=False)
