Classifying Hidden Data with KNN

The Goal

In this project, I worked with a dataset that was a bit of a mystery none of the columns had real names, just numerical values. The objective was to build a K-Nearest Neighbors (KNN) model that could look at these numbers and accurately predict which class a data point belonged to.


What I Did



Getting the Data Ready:

The first thing I realized was that the numbers in the different columns weren't on the same scale. Since KNN works by measuring the physical distance between data points, a large number in one column could easily trick the model into thinking that feature is more important than others. I fixed this by using StandardScaler to normalize everything, ensuring each feature had a mean of 0 and a standard deviation of 1.



Finding the Best K:

I started with a simple model where K=1, but I knew I could do better. To find the most accurate version of the model, I ran a loop that tested every K value from 1 to 40.

I plotted the error rates for each one to find the "Elbow." It was pretty clear from the graph that as K increased, the error rate dropped significantly. I noticed the model really stabilized around K=30, which gave me the best balance between speed and accuracy.



The Results:

Retraining the model with K=30 made a huge difference. My final accuracy ended up around 84%, which was a big jump from the initial test. The confusion matrix confirmed that the model was much better at distinguishing between the two classes than the baseline version.


Tools Used:

I used Python along with the standard data science stack: Pandas for handling the tables, Matplotlib for visualizing the error rates, and Scikit-Learn for the machine learning and data scaling.

How to View:

You can open the .ipynb file in Google Colab or Jupyter to see the step-by-step code, the visualizations, and the final classification report.
