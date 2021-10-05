# feature_selection_functions
Feature selection is widely used in nearly all data science pipelines. Hence I have created functions that do a form of backward stepwise selection based on the XGBoost classifier feature importance and a set of other input values with the goal to return the number of features to keep (with the highest feature importance score) in regard to a prefered AUC-score.

NOTE: For these functions I use AUC-score as the performance metric to compare the classifier and the number of features to keep, but that could easily be replaced by a F1-score, True Negative Rate, Accuracy, Precision, Recall etc. 
