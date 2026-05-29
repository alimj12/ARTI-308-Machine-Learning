**Lab #7: Logistic Regression Project**


**The Goal:**

In this project, I built a Binary Classification model using Logistic Regression to predict whether a specific internet user will click on an advertisement. The objective was to analyze user demographics and digital behavior such as daily internet usage and time spent on the site to create a predictive tool that can help businesses optimize their targeted marketing campaigns.

**What I Did:**

•	Exploratory Data Analysis (EDA): I explored the dataset to find meaningful correlations. Using Jointplots, I analyzed the 
relationship between Age and Area Income, as well as Daily Time Spent on Site versus Daily Internet Usage. These visualizations helped identify the specific user segments most likely to engage with ads.

•	Data Preparation: I focused on selecting the most impactful numerical features, including Daily Time Spent on Site, Age, Area Income, and Daily Internet Usage. I ensured the data was properly split into Training (70%) and Testing (30%) sets to validate the model's performance on unseen data.

•	Logistic Regression Modeling: I implemented and trained a LogisticRegression model. This involved teaching the algorithm to find the optimal "decision boundary" that separates users who click on ads from those who do not.

•	Classification Diagnostics: I evaluated the model using a Confusion Matrix to track true positives and false positives. 
I also generated a Classification Report to analyze precision, recall, and the F1-score, ensuring the model is reliable for real world deployment.

**The Results:**

The model performed exceptionally well, achieving an accuracy of 91%. The analysis confirmed that Daily Internet Usage and Daily Time Spent on Site are the strongest predictors of ad engagement. This project demonstrates how statistical learning can transform raw user data into actionable insights for the digital advertising industry.

**Tools Used:**

•	Python: The primary language for the analysis.

•	Pandas & NumPy: For data manipulation and scientific computing.

•	Seaborn & Matplotlib: For creating high-quality statistical plots and diagnostic visualizations.

•	Scikit-Learn: For building the machine learning pipeline and calculating evaluation metrics.

•	Google Colab: The environment for interactive development.

**How to View:**

Open the Lab#7 Ali Aljanabi.ipynb file in Google Colab or Jupyter Notebook. You will find the complete workflow, including detailed data visualizations, model training steps, and the final classification performance analysis.

