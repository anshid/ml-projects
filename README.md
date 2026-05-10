# Machine Learning Projects 🚀

Welcome to my Machine Learning repository! 

> ⚠️ **Note:** This is an active, **working repository**. I am continuously learning and experimenting, so I will keep updating this repo and adding new project files, models, and notes over time.

This repository contains various ML models, exercises, and projects I have built while learning Machine Learning concepts—ranging from basic regression and unsupervised learning to more complex classification tasks.

---

## 📂 Current Projects

### 1. [Seoul Bikes Regression](project_seoul_bikes_regression.ipynb)
A regression model to predict bike rental demand at noon in Seoul based on weather conditions.

- **Dataset:** UCI Seoul Bike Sharing Demand — 8,760 hourly records filtered to 365 noon observations
- **Techniques:** Exploratory data analysis, feature selection, univariate & multivariate linear regression, TensorFlow/Keras neural network (32→32→1 architecture)
- **Key Result:** Multiple linear regression achieved R² = 0.528; linear regression outperformed the neural network on test MSE, highlighting that the relationship is largely linear

---

### 2. [MAGIC Gamma Telescope Classification](project_MAGIC_Gamma_Telescope.ipynb)
A binary classification task distinguishing high-energy gamma rays from cosmic ray background noise using telescope imaging data.

- **Dataset:** UCI MAGIC Gamma Telescope — 19,020 samples, 10 Hillas parameter features, imbalanced classes (gamma vs. hadron)
- **Techniques:** RandomOverSampler (SMOTE-style), StandardScaler, KNN, Naive Bayes, Logistic Regression, SVM, TensorFlow/Keras neural network with grid search hyperparameter tuning
- **Key Results:**

| Model | Test Accuracy |
|-------|--------------|
| KNN (k=1 & k=5) | 82% |
| Naive Bayes | 74% |
| Logistic Regression | 79% |
| SVM | 87% |
| Neural Network | **88%** |

---

### 3. [Seeds Unsupervised Learning](project_seeds_unsupervised.ipynb)
An unsupervised learning project applying clustering to a wheat seeds dataset to discover natural groupings without using labels.

- **Dataset:** UCI Seeds Dataset — 210 samples, 7 geometric features (area, perimeter, compactness, etc.), 3 wheat varieties
- **Techniques:** K-Means clustering (k=3), PCA dimensionality reduction to 2 components, pairwise scatter plot exploration, cluster vs. true-label comparison
- **Key Result:** K-Means cleanly separated the three seed varieties; PCA projection preserved the cluster structure, confirming strong natural groupings in the data

---

### 4. [MNIST Image Classifier](MNIST_image_classifier.ipynb)
A classic image classification project training models to recognise handwritten digits from the MNIST dataset.

- **Dataset:** MNIST — 60,000 training / 10,000 test images (28×28 grayscale, 10 classes)
- **Techniques:** Two PyTorch architectures compared — a fully-connected `LinearMNIST` baseline and a `SimpleCNN` with 2 convolutional layers, ReLU, and max pooling; trained with Adam optimizer and CrossEntropyLoss
- **Key Result:** `SimpleCNN` reached **99.09% test accuracy** in just 5 epochs with minimal overfitting

---

### 5. [Add Numbers ML Model](add_numbers_ml_model.ipynb)
An introductory PyTorch exercise demonstrating how a neural network can learn a simple mathematical relationship from scratch.

- **Dataset:** 100,000 synthetically generated random number pairs in [−100, 100]; target = x₁ + x₂
- **Techniques:** PyTorch 2-input linear network, MSELoss, SGD optimizer, 5,000 training epochs
- **Key Result:** Learned weights converged to ≈ [1.0, 1.0] — the correct coefficients for addition — with loss dropping from ~2,725 to ~0.016

---

### 6. [Linear Regression & Gradient Descent — Visual Teaching Notebook](LinearRegression_GradientDescentAlgorithmV1.ipynb)
A step-by-step educational notebook that builds deep intuition for linear regression and gradient descent through interactive visualizations. Designed for beginners with no prior ML background.

- **Dataset:** 200-point synthetic dataset generated from a known true line (y = 4x + 7 + noise), chosen so the reader can verify that the algorithm recovers the correct parameters
- **Concepts covered:** MSE loss function, convex loss surfaces, partial derivative derivations (hidden in collapsible cells for those who want the calculus), gradient descent update rule, learning rate selection
- **Visualizations:**
  - 3D interactive loss surface (bowl shape illustrating convexity)
  - **Dual-panel interactive slider** — left panel shows the gradient descent path on the loss contour map; right panel shows the evolving regression line in data space; both update in sync
  - Loss curve (convergence monitoring)
  - 3D trajectory of gradient descent overlaid on the loss surface
  - Side-by-side learning rate comparison (too small / just right / too large)
- **Key insight conveyed:** Gradient descent moves through *parameter space* (slope, intercept) — the regression line improves only because the parameters improve. The synchronized dual-panel visualization makes this abstract idea concrete and observable.

---

## 📊 Quick Overview

| Project | Learning Type | Key Techniques | Best Result |
|---------|--------------|----------------|-------------|
| Seoul Bikes | Regression | Linear Reg, TF/Keras NN, Feature Selection | R² = 0.528 |
| MAGIC Telescope | Binary Classification | KNN, SVM, LR, NB, NN + SMOTE | 88% accuracy |
| Seeds Clustering | Unsupervised | K-Means, PCA | 3 clean clusters |
| MNIST Classifier | Image Classification | CNN (PyTorch), 2 architectures | 99.09% test accuracy |
| Add Numbers | Intro / Regression | PyTorch linear net | Weights ≈ [1.0, 1.0] |
| LR & GD Visual | Educational / Optimization | Gradient Descent, Interactive Plotly, MSE Loss Surface | Recovers true m=4, b=7 |

---

## 🛠️ Technologies & Libraries Used

**Deep Learning:** PyTorch, TensorFlow / Keras  
**Machine Learning:** Scikit-learn, imbalanced-learn (SMOTE)  
**Data & Analysis:** Pandas, NumPy  
**Visualization:** Matplotlib, Seaborn, Plotly  
**Data Sources:** UCI ML Repository, Kaggle Hub  
**Environment:** Jupyter Notebook, Python 3

---

*Feel free to explore the notebooks and follow along as I add more projects!*
