**Lab #10: Iris Flower Classification with Support Vector Machines (SVM)**

**The Goal:**

In this project, I implemented a Support Vector Machines (SVM) model to classify different species of Iris flowers. The objective was to analyze biological measurements such as sepal and petal dimensions to build a high precision classifier capable of distinguishing between three related species: Setosa, Versicolor, and Virginica.

**What I Did:**

•	Multivariate Data Exploration: I performed an extensive Exploratory Data Analysis (EDA) using Pairplots to visualize the relationships between all features. This helped identify that the "Setosa" species is linearly separable from the others, while "Versicolor" and "Virginica" require a more complex decision boundary.

•	Model Training & Implementation: I built a baseline SVM classifier using the RBF (Radial Basis Function) kernel. I split the dataset into training and testing sets to evaluate the model’s ability to generalize to new, unseen biological samples.

•	Hyperparameter Tuning with GridSearchCV: To maximize performance, I used GridSearchCV to systematically find the optimal values for the parameters C (regularization) and gamma (kernel coefficient). This automated optimization ensured the model found the most effective decision boundary.

•	Diagnostic Evaluation: I generated a Confusion Matrix and a Classification Report to assess the model's accuracy. This detailed breakdown allowed me to verify the precision and recall for each individual species, ensuring the model wasn't biased toward one type of flower.

**The Results:**

The optimized SVM model achieved an impressive accuracy of 98%. The analysis confirmed that while simple sepal measurements provide a baseline, the combination of petal length and width is highly predictive of the species. The project demonstrated that even with overlapping data points, a tuned SVM with an RBF kernel can achieve near perfect classification.

**Tools Used:**

•	Python: The primary language for machine learning.

•	Pandas & NumPy: For data structural analysis and numerical processing.

•	Scikit-Learn: For the SVM algorithm, GridSearchCV optimization, and performance metrics.

•	Seaborn & Matplotlib: For advanced statistical visualizations and pair-wise relationship plots.

•	Google Colab / Jupyter Notebook: The interactive development environment.

**How to View:**

Open the Lab#10 Ali Aljanabi.ipynb file in Google Colab or Jupyter Notebook. You will find the complete classification pipeline, including the pairplot visualizations, the grid search results, and the final model performance metrics.

