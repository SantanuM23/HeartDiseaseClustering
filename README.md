# Heart Disease Clustering Project

## Project Overview
This project focuses on clustering patients based on heart disease data using unsupervised machine learning techniques. The data undergoes extensive preprocessing, feature engineering, and outlier handling before clustering. Visualizations are used throughout to analyze the data and clustering results.

---

## Table of Contents
1. [Data Preprocessing](#data-preprocessing)
2. [Feature Engineering](#feature-engineering)
3. [Handling Outliers](#handling-outliers)
4. [Clustering Analysis](#clustering-analysis)
5. [Visualizations](#visualizations)

---

## Data Preprocessing
1. **Dataset Information**:
    - Missing values were identified and handled using heatmaps.
    - Specific columns with missing values were filled with either `0` (numerical) or `'None'` (categorical).

2. **Feature Separation**:
    - Numerical Features
    - Categorical Features
    - Continuous and Discrete Features

3. **Encoding**:
    - Categorical features were one-hot encoded to make them suitable for machine learning algorithms.

---

## Feature Engineering
1. **Oldpeak Classification**:
    - `oldpeak` values were categorized into depression or elevation levels based on predefined thresholds.

2. **Cholesterol Grouping**:
    - Cholesterol levels were categorized into Low, Moderate, and High groups.

3. **Age Grouping**:
    - `age` was binned into groups based on ranges for better analysis.

4. **Other Features**:
    - Resting blood pressure and thalach features were grouped based on normal ranges and health standards.

---

## Handling Outliers
1. Continuous numerical features were analyzed using:
    - **Histograms**: To identify skewness.
    - **Boxplots**: To detect outliers visually.
    - **Q-Q Plots**: To check normality.

2. Outliers were capped and floored using the Interquartile Range (IQR) method.

---

## Clustering Analysis
1. **KMeans Clustering**:
    - The elbow method was used to determine the optimal number of clusters.
    - Silhouette scores were calculated for various cluster sizes to validate the clustering quality.

2. **Final Clustering**:
    - Clustering was performed with the optimal number of clusters.

---

## Visualizations
1. **Correlation Heatmaps**:
    - Correlations of continuous features and missing data were visualized using heatmaps.

2. **Missing Data Heatmap**:
    - Identified patterns in missing data across the dataset.

3. **Outlier Visualizations**:
    - Histograms, boxplots, and Q-Q plots were used for all continuous features.

4. **Clustering Results**:
    - Scatter plots visualized the distribution of clusters and centroids.

---

## Results
- Data preprocessing and feature engineering improved the clustering results.
- KMeans clustering successfully grouped patients into clusters based on heart disease-related features.

---

## Technologies Used
- **Programming Language**: Python
- **Libraries**:
  - `pandas` for data manipulation.
  - `numpy` for numerical computations.
  - `seaborn` and `matplotlib` for visualizations.
  - `scipy` for statistical analysis.
  - `scikit-learn` for clustering and evaluation.

---

## Installation
1. Clone the repository:
    ```bash
    git clone <repository-url>
    ```
2. Install the required libraries:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

3. Run the script:
    ```bash
    python clustering_analysis.py
    ```


