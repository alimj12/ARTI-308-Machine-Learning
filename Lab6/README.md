**Lab #6: E-commerce Customer Spend Prediction.**

**The Goal:**

In this project, I leveraged Linear Regression to analyze customer behavior for an E-commerce platform. The objective was to determine which digital channel Mobile App or Website has a more significant impact on the "Yearly Amount Spent" by customers, helping the company prioritize their development efforts effectively.

**What I Did:**

•	Exploratory Data Analysis (EDA): I used Jointplots and Pairplots to explore relationships between features like Time on App, Time on Website, and Length of Membership. This visual analysis revealed a strong linear correlation between membership duration and total spending.

•	Data Partitioning: I split the customer data into Training (70%) and Testing (30%) sets to ensure the model's performance was validated against unseen customer profiles.

•	Model Implementation: I trained a Linear Regression model using Scikit Learn to map customer metrics to their yearly expenditure.

•	Coefficient Analysis & Interpretation: I calculated and analyzed the model's coefficients. This crucial step quantified the specific impact of each feature revealing exactly how much expenditure increases for every additional minute spent on the app versus the website.

•	Performance Metrics: I assessed the model’s reliability using MAE, MSE, and RMSE. The results showed a very high level of predictive accuracy, with minimal error in estimating customer spend.

**The Results:**

The analysis provided a clear strategic insight: Time spent on the Mobile App and the Length of Membership are the primary drivers of revenue. The model's coefficients clearly demonstrated that investments in the mobile experience yield significantly higher returns than website optimizations, providing a data-driven foundation for business decision-making.

**Tools Used:**

•	Python: The core analytical language.

•	Pandas & NumPy: For data manipulation and numerical operations.

•	Scikit Learn: For regression modeling and statistical evaluation.

•	Seaborn & Matplotlib: For creating advanced statistical visualizations and correlation heatmaps.

**How to View:**

Open the Lab#6 Ali Aljanabi.ipynb file in Google Colab or Jupyter Notebook to see the complete workflow, including the detailed correlation analysis and the final strategic recommendations based on the regression coefficients.

