# Learning-to-Label-From-Clustering-to-Classification
Evaluating performance of multiple classifiers on unlabeled image and text datset.

# Image Processing and Unsupervised Image Classification

## Overview
This project explores image processing, clustering, and classification techniques on unlabeled image data. The objective is to perform unsupervised clustering to generate pseudo-labels, and train supervised machine learning models using those generated labels.

## Objectives
- Visualize and preprocess image data.
- Apply PCA for dimensionality reduction.
- Perform unsupervised image clustering.
- Generate pseudo-labels using clustering algorithms.
- Train and evaluate classification models using generated labels.

## Dataset
- Unlabeled MNIST grayscale image dataset.
- Image size: **28 × 28 pixels**
- Images are flattened and transformed into feature vectors for analysis.

## Methodology

### 1. Data Preprocessing
- Load image dataset (.npy format).
- Reshape images into 28×28 format.
- Flatten images into feature vectors.

### 2. Principal Component Analysis (PCA)
- Standardize image features.
- Reduce dimensionality using PCA.
- Analyze:
  - Explained variance
  - Reconstruction error (MSE)
  - Original vs reconstructed images

### 3. Clustering
Implemented:
- K-Means Clustering
- Gaussian Mixture Models (GMM)

Evaluation:
- Silhouette Score
- Cluster visualization

### 4. Pseudo Label Generation
Cluster assignments are used as labels for supervised learning.

### 5. Classification Models
Trained models:
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)

Evaluation metrics:
- Accuracy
- Classification Report
- Confusion Matrix

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn

## Results

- K-means method was better at clustering than GMM.
- Logistic regression was the most accurate classification model.
  

- # Text Encoding and Word Embedding Analysis using Word2Vec

## Overview
This project focuses on Natural Language Processing (NLP) techniques for text preprocessing, word embedding generation, clustering, visualization, and classification. The project builds semantic word representations using Word2Vec and analyzes relationships among words through clustering.

## Objectives
- Clean and preprocess textual data.
- Perform tokenization, stemming, and lemmatization.
- Generate dense word embeddings using Word2Vec.
- Visualize semantic relationships between words.
- Cluster similar words.
- Build machine learning classifiers using generated embeddings.

## Dataset
Text corpus containing documents that undergo preprocessing and encoding.

## Methodology

### 1. Text Preprocessing

Implemented:
- Text cleaning
- Unicode normalization
- Tokenization
- Stopword removal
- Stemming
- Lemmatization

Libraries:
- NLTK
- Regular Expressions (Regex)

### 2. Word Embedding Generation

Model:
- Word2Vec (Gensim)

Parameters:
- Vector Size: 100
- Context Window: 5
- Continuous Bag of Words (CBOW)

Output:
- Dense semantic vector representations for words.

### 3. Embedding Visualization

Dimensionality Reduction:
- t-SNE
- PCA

Purpose:
- Visualize semantic similarity between words in 2D space.

### 4. Clustering

Implemented:
- K-Means
- DBSCAN
- HDBSCAN

Evaluation:
- Silhouette Score
- Cluster Visualization

### 5. Classification Models

Trained models:
- Logistic Regression
- Support Vector Machine (SVM)
- XGBoost Classifier

Evaluation Metrics:
- Accuracy
- Classification Report
- Confusion Matrix

## Technologies Used

- Python
- NLTK
- Gensim
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- XGBoost
- HDBSCAN

## Results

- K-Means clustering successfully groups visually similar images.
- Supervised classifiers trained on pseudo-labels achieve meaningful classification performance.


