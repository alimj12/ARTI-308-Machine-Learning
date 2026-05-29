Lab#4: Data Quality Assessment & Preprocessing


The Goal

In this project, I moved beyond basic analysis to perform advanced Data Preprocessing on the credit card fraud dataset. The primary objective was to engineer the data into a high-quality format suitable for machine learning, focusing on noise reduction, outlier handling, and compressing 30 technical dimensions into a streamlined set of principal components.

What I Did

•	Handling Missing Values & Noise: I implemented a robust missing value strategy using Median Imputation. This was chosen over the mean to prevent skewed financial data and outliers from biasing the dataset.

•	Outlier Detection (IQR Method): Using the Interquartile Range (IQR) technique, I identified and analyzed extreme transaction values. In a cybersecurity context, I treated these outliers not just as errors, but as potential "anomaly signatures" that often indicate fraudulent behavior.

•	Feature Scaling (Standardization): I applied StandardScaler (Z-score normalization) to the Time and Amount features. This centered the data around a mean of 0, ensuring that large transaction amounts don't overshadow other technical features ($V1-V28$) during model training.

•	Dimensionality Reduction (PCA): I performed Principal Component Analysis (PCA) to transform 30 complex features into 5 optimized Principal Components. This process captured ~53% of the total variance, effectively reducing noise and computational cost while preserving the core "fraud signals."

•	Visualizing Anomalies: I created a 2D PCA Projection plot to visualize the high-dimensional data. This allowed me to see how fraudulent-like transactions "drift" away from the main cluster of legitimate activities, providing a clear visual map for anomaly detection.

The Results

The preprocessing phase successfully simplified the dataset from 30 features down to 5, while maintaining over half of the original information. The visualization confirmed that fraud isn't always about the dollar amount, but about the statistical deviation from normal behavior. This refined dataset is now ready for high-performance classification models.

Tools Used

•	Python: For advanced technical automation.

•	Scikit-Learn: Used for the StandardScaler, SimpleImputer, and PCA algorithms.

•	Pandas & NumPy: For complex data structures and mathematical operations.

•	Seaborn & Matplotlib: To render the PCA projections and correlation heatmaps.

•	Google Colab: For cloud-based interactive development.

How to View

Open the Lab#4 Ali Aljanabi.ipynb file in Google Colab or Jupyter Notebook. The notebook follows a structured pipeline: from data cleaning to final dimensionality reduction, with detailed cybersecurity-focused insights at every step.

