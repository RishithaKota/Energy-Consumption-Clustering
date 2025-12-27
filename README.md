# Energy-Consumption-Clustering
Energy Consumption Clustering is an unsupervised ML project that groups household energy usage patterns using K-Means. The data is cleaned, normalized, and reduced with PCA. Cluster quality is evaluated using the Elbow Method and Silhouette Score, and results are visualized in 2D PCA space.

## 🛠 Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  

---

##  Dataset Description
- The dataset contains **ACORN household categories (ACORN-A to ACORN-Q)** as columns.
- Rows represent different demographic or household-related indicators.
- Numerical values represent indexed energy or consumption-related attributes.

---

##  Methodology

### 1. Data Loading
- CSV file loaded using encoding-safe methods to handle non-UTF8 characters.

### 2. Data Cleaning
- Missing values handled using mean imputation.
- Invalid or negative values clipped to ensure realistic inputs.

### 3. Data Transformation
- Dataset transposed so that each ACORN group represents one observation.

### 4. Feature Normalization
- StandardScaler applied to normalize features.

### 5. Dimensionality Reduction (PCA)
- PCA reduces features to two components for visualization.

### 6. K-Means Clustering
- Elbow Method used to determine optimal number of clusters.
- K-Means applied to PCA-reduced data.

### 7. Evaluation
- Silhouette Score used to measure cluster quality.

### 8. Visualization
- 2D PCA scatter plot visualizes cluster separation.

---

##  Outputs & Generated Files

| File Name | Description |
|----------|-------------|
| cleaned_acorn_data.csv | Cleaned dataset |
| normalized_acorn_data.csv | Normalized features |
| pca_acorn_features.csv | PCA-reduced features |
| clustered_acorn_profiles.csv | Final clusters |
| pca_clusters_2D.csv | PCA + cluster labels |

---

##  How to Run
1. Open the Jupyter Notebook
2. Run all cells sequentially
3. CSV outputs will be generated automatically

---

##  Applications
- Energy usage profiling
- Demand forecasting
- Smart grid analytics
- Policy and planning support

---

##  Conclusion
The project demonstrates a complete unsupervised learning workflow for clustering energy consumption patterns using PCA and K-Means.

---

