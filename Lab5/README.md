**Lab #5: Feature Engineering (Classification)**

**The Goal:**

In this project, I focused on the most critical phase of the Machine Learning pipeline: Feature Engineering. Using a Talabat-style dataset, the objective was to transform raw order data into high-value predictive features. By engineering logistical, temporal, and financial metrics, I aimed to provide a Random Forest model with the "intelligence" needed to accurately predict the final Order_Status (Completed vs. Cancelled).

**What I Did:**

•	Logistical Efficiency Mapping: I engineered the delivery_speed_km_per_hour feature to quantify delivery performance. This allowed the model to distinguish between geographical distance and actual operational efficiency, highlighting logistical bottlenecks.

•	Temporal Stress Analysis: I developed a refined is_peak_hour logic, specifically targeting high-demand windows (Lunch: 12–14 and Dinner: 18–21). This helped identify how operational "rush hours" impact delivery success rates.

•	Business-Driven Binning: I implemented a Price Tiering strategy (low, medium, high, very_high) and calculated price_per_item. This captured the "premiumness" of orders, helping the model understand if high-value transactions or restaurant types influence cancellation patterns.

•	Dimensionality Management: To handle high-cardinality categorical data, I applied a Top-K reduction (testing $K=10$ and $K=30$) for item names. This balanced model granularity with computational efficiency, grouping rare items into an "Other" category to reduce noise.

•	Feature Selection & Optimization: Using SelectFromModel with Random Forest importance, I streamlined the dataset. I removed redundant identifiers (IDs) and raw timestamps to prevent overfitting and ensure the model only learns from truly predictive patterns.

**The Results:**

The feature engineering process proved highly effective, achieving a robust model accuracy of 0.8519. The analysis revealed that while expanding item categories (top_k=30) shifted feature importance towards geospatial data, a streamlined model with engineered features maintained high predictive integrity. This confirms that how you represent the data (Features) is just as important as the algorithm itself.

**Tools Used:**

•	Python: The core language for technical automation.

•	Pandas & NumPy: For complex data transformations and mathematical engineering.

•	Scikit-Learn: For feature selection (SelectKBest/SelectFromModel) and model evaluation.

•	Matplotlib & Seaborn: For visualizing feature importance and distribution tiers.

**How to View:**

Open the Lab#5 Ali Aljanabi.ipynb file in Google Colab or Jupyter Notebook. You will find the complete feature engineering pipeline, from raw data parsing to the final optimized feature matrix.

