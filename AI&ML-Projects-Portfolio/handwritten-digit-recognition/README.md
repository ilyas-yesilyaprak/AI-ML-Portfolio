# Handwritten Digit Recognition (MNIST)

This project classifies handwritten digits using two machine learning models: k-Nearest Neighbors (k-NN) and Decision Trees.

## 📊 Dataset
- **MNIST** dataset from Keras API (70,000 grayscale 28x28 images)
- **Split**: 80% training, 20% validation
- **Normalization**: pixel values scaled to [0, 1] by dividing by 255

## 🔍 Exploratory Data Analysis
- Class distribution visualization
- Pixel intensity statistics and histograms
- Misclassification visualization using images

## 🧠 Models & Parameters

### k-NN Classifier
- Tradeoff between overfitting and generalization

### Decision Tree Classifier
- Tested `max_depth`: 5, 10
- Best result with `max_depth = 10`, `min_samples_split = 2`

## 📈 Evaluation
- Accuracy, Precision, Recall, F1-score
- Confusion Matrix and ROC Curves for all 10 classes
- Displayed most misclassified examples

## 🛠️ Tech Stack
Python, Scikit-learn, Keras (for MNIST), NumPy, Matplotlib, Seaborn

## 🚀 How to Run
1. Install dependencies (scikit-learn, matplotlib, etc.)
2. Run the notebook cell by cell to train and evaluate both models
