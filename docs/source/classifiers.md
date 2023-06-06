# Machine Learning Classifiers
---------------------------

## Model Training
This module contains the following classifiers:
- **Logistic Regression**: Logistic Regression (aka logit, MaxEnt) classifier.
- **LightGBM**: LightGBM is a gradient boosting framework that uses tree based learning algorithms.
- **Random Forest**: A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting.
- **Support Vector Machine**: Support Vector Machine (SVM) is a supervised machine learning algorithm which can be used for both classification or regression challenges. However,  it is mostly used in classification problems.

Once the classifiers are selected the models are trained and the ROC curves for all the models are shown in the graph. The model can be saved by creating a new Experiment and giving it a name and clicking on the "Save model" button.

## Inference
The trained model can be used to make predictions on new data. The new data can be uploaded as a csv file. The file should contain the same features as the training data. The predictions are shown in a table and can be downloaded as a csv file.