# feature_selection_functions
## by Lennart Wallentin, lennartwallentin@gmail.com 
Feature selection is the technique of finding the minimal subset of features that allows for the maximal predictive power. Feature selection has become a crucial preprocessing stage to overcome issues such as “the curse of dimensionality” and overfitting. Moreover, the feature selection techniques are particularly useful to reduce the data size because many classifiers scale in complexity with the dimensionality of the data. Feature selection also eases the understanding of the dataset’s structure by eliminating irrelevant and redundant features. Therefore, feature selection is widely used in nearly all data science pipelines. 

A benefit of using ensembles of decision tree methods like extreme gradient boosting (XGBoost) is that they provide estimates of feature importance from a trained model. Hence I have created functions that do a form of backward stepwise selection based on the feature importance and a set of other input values with the goal to return the number of features to keep (with the highest feature importance score) in regard to the AUC-score. 
I have created four functions, two for a more interpretable way of doing feature selection and the other two functions are automated and suitable to use in a data science pipeline especially in those occasions when you want to update your model. 

NOTE: For these functions I use AUC-score as the performance metric to compare the classifier and the number of features to keep, but that could easily be replaced by a F1-score, True Negative Rate, Accuracy, Precision, Recall etc.

This is the structure of the project 'feature_selection_lennart_wallentin.ipynb':
1. Interpretable Feature Selection 
2. Automated Feature Selection
