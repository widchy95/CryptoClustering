# CryptoClustering

## Project Overview
The **CryptoClustering** project aims to perform K-Means clustering analysis on a cryptocurrency market dataset to identify patterns and similarities between different cryptocurrencies based on their performance metrics. This project involves data preparation, scaling, PCA transformation, and clustering visualization to reveal insights about market trends.

## Folder Structure
```
CryptoClustering
│
├── Crypto_Clustering.ipynb   # Main Jupyter Notebook for analysis
│
├── Resources                 # Directory for data files
│   └── crypto_market_data.csv  # CSV file containing the crypto market data
│
└── README.md                 # Project description file
```

## Project Steps and Process

### 1. Data Preparation
- Load the cryptocurrency market data from `crypto_market_data.csv`.
- Display and inspect the dataset to understand its structure and features.

### 2. Data Preprocessing
- Use `StandardScaler` from `scikit-learn` to normalize the data to ensure features are on a comparable scale.
- Create a DataFrame containing the scaled data while retaining the `coin_id` as the index.

### 3. Elbow Method to Find Optimal k
- Use the Elbow Method to identify the optimal number of clusters (`k`) by calculating the inertia for a range of `k` values from 1 to 11.
- Plot the Elbow curve to visualize the optimal number of clusters for K-Means.

### 4. K-Means Clustering
- Fit the K-Means model to the original scaled data and predict cluster assignments.
- Create a scatter plot to visualize the clustering results using key performance metrics as axes.

### 5. PCA Transformation
- Apply Principal Component Analysis (PCA) to reduce the dimensionality of the data to three principal components while retaining most of the variance.
- Use the PCA-transformed data for further K-Means clustering.

### 6. Clustering with PCA Data
- Fit the K-Means model to the PCA-transformed data and predict cluster assignments.
- Create visualizations to compare the clustering results from the original data and the PCA-transformed data.

### 7. Results Visualization and Analysis
- Create comparative plots for cluster analysis and Elbow curves for both original and PCA data.
- Discuss the impact of using fewer features on clustering performance and interpretability.

## Deployment and Submission
To ensure full credit for this project:

1. **Submit the GitHub Repository**: Ensure the repository is cloned locally and contains all project files.
2. **Use Command Line for Git Operations**:
   - Add files to the repository using Git commands.
3. **Include Commit Messages**:
   - Ensure that commit messages are informative and reflect the changes made.

## Installation and Libraries Required
Make sure to install the following Python libraries to run the project:

- `pandas`
- `hvplot`
- `scikit-learn`

Install them using:
```bash
pip install pandas hvplot scikit-learn
```

## Usage
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/widchy95/CryptoClustering.git
   cd CryptoClustering
   ```

2. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Crypto_Clustering.ipynb
   ```

3. Follow the step-by-step analysis and execute the code cells to see the results.

## Conclusion
The **CryptoClustering** project showcases the process of clustering cryptocurrencies using K-Means with both the original and PCA-reduced data. The comparison of clustering results highlights how dimensionality reduction can impact the analysis and visualization of complex datasets.

**Widchy Joachim**
*Data Analyst*
