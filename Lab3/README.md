Lab#3: Credit Card Fraud Detection with EDA

The Goal

In this project, I performed a comprehensive Exploratory Data Analysis (EDA) on a highly imbalanced dataset of credit card transactions. The objective was to uncover hidden patterns, analyze temporal trends of fraudulent activities, and understand the relationships between anonymized technical features (V1-V28) to prepare the data for building a robust Fraud Detection system.

What I Did

•	Data Cleaning & Preprocessing: I started by ensuring the data was "clean" for analysis. This involved checking for missing values and duplicates. Since fraud datasets are naturally imbalanced (legitimate transactions far outnumber fraudulent ones), I focused on analyzing the distribution of the Class target variable.

•	Bivariate & Multivariate Analysis: I explored the relationship between transaction Amount and Time. Since fraudulent transactions are often "hidden" within the noise of normal data, I used advanced layering techniques in my scatter plots to highlight fraud points (in red) against legitimate ones (in blue), making the anomalies clearly visible.

•	Correlation & Feature Insights: I generated a Correlation Heatmap to see how the features relate to one another. Since the features $V1-V28$ are transformed using PCA (Principal Component Analysis), I looked for strong positive or negative correlations with the Class variable to identify which features are the most significant "red flags" for fraud.

•	Time-Based Distribution: I analyzed the temporal patterns of fraud using a histogram. This revealed that fraudulent activities aren't random; they often occur in bursts or clusters, which is a vital insight for real-time security monitoring.

The Results
The EDA confirmed that the dataset is extremely imbalanced, meaning traditional accuracy metrics won't be enough. I discovered that fraud isn't necessarily tied to high value amounts, but rather to specific patterns in the hidden technical features. This analysis provides a solid foundation for the next phase: Machine Learning Modeling.

Tools Used
•	Python: The core language.
•	Pandas: For data manipulation and structure.
•	Seaborn & Matplotlib: For creating professional, cybersecurity-focused visualizations.
•	Google Colab: The environment for interactive development.

How to View
Open the Lab#3 Ali Aljanabi.ipynb file in Google Colab or Jupyter Notebook. You will find the step by step code, detailed visualizations, and insights derived from each stage of the analysis.
