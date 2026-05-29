**Lab #11: Credit Card Customer Segmentation (K-Means Clustering)*

**The Goal:**

In this project, I applied Unsupervised Learning techniques to segment credit card holders based on their usage behavior. Using a dataset of approximately 9,000 active users, the objective was to identify distinct customer personas such as 
high spenders or those reliant on cash advances to help financial institutions design data driven marketing strategies and personalized financial products.

**What I Did:**

•	Data Cleaning & Imputation: I handled missing values in critical behavioral features like MINIMUM_PAYMENTS and CREDIT_LIMIT using mean imputation. I also dropped the CUST_ID column, as it serves only as a unique identifier and does not contribute to the clustering logic.

•	Feature Scaling: Since K-Means relies on Euclidean distance, I utilized StandardScaler to normalize the data. This step was crucial to ensure that high magnitude features (like Balance) do not overshadow smaller scale features during the clustering process.

•	Elbow Method & Silhouette Analysis: I implemented the Elbow Method to find the optimal number of clusters (K). 
By analyzing the "Inertia" curve and confirming with the Silhouette score, I determined the most stable and meaningful number of segments for this customer base.

•	K-Means Model Implementation: I trained the final clustering model to group customers based on 17 behavioral variables, including purchase frequency, balance maintenance, and payment patterns.

•	Cluster Interpretation: I summarized the characteristics of each resulting cluster to define customer segments. 
This involved analyzing the mean values of each group to distinguish between "VIP Spenders," "Cash-Reliant Users," and "Conservative/Low-Activity Users."

**The Results:**

The clustering model successfully partitioned the customers into actionable segments with clear behavioral profiles. 
The analysis proved that customer value is not just about balance, but a combination of purchase frequency and credit utilization. These insights provide a solid foundation for targeted marketing campaigns, such as offering reward programs to active spenders or debt restructuring plans to cash-reliant segments.

**Tools Used:**

•	Python: The primary programming language.

•	Pandas & NumPy: For robust data manipulation and statistical imputation.

•	Scikit-Learn: For the K-Means algorithm, feature scaling, and model evaluation metrics.

•	Seaborn & Matplotlib: For generating the Elbow curve and behavioral distribution plots.

•	Google Colab: The environment for interactive data science development.

**How to View:**

Open the Lab#11 Ali Aljanabi.ipynb file in Google Colab or Jupyter Notebook. You will find the complete end-to-end unsupervised learning pipeline, including data normalization, K-optimization plots, and the final segment behavioral 
