The US Equity Regression Repository aims to use machine learning regression algorithms to predict the next-period z-score of free cash flow per share. The idea is that companies with relatively good FCF per share compared to historical data will perform better than their counterparts. The main processes undergone in this repository are outlined as follows:

  1. Data gathering and Consolidation: Perform fundamental data preprocessing starting with previously-scraped US pricing and fundamental data. 
  2. Preprocessing: This notebook walks imputing missing/NaN values, handling outliers with DBSCAN, scaling data, and using feature engineering to augment the dataset. There is particular emphasis in this notebook to use data visualizations on our data-tailoring journey.
  3. Premodeling: A longer notebook in which many of the steps may also be classified as preprocessing. The focus of this code is to specifically prepare our data for feeding through a Machine Learning model in Python. This notebook contains code focused on evaluating predictive power of features, tailoring the feature space, and using SKLearn's StackingRegressor to train a model that can be used on go-forward data.
  4. Machine Learning Modeling and Evaluation: With the fully trained model and holdout data available, this notebook starts by confirming efficiacy of the model on the holdout data, after which the performance of the model is analyzed according to various metrics.


