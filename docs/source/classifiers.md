# Machine Learning Classifiers
---------------------------

## Training

### Selecting the data source
The user can train a machine learning model on the data. The input for the ML model can be: 
1. The data that has been processed with the tool during current session.
2. Upload a csv file with the data. The file should contain the same features as the training data.
3. A sample data with used for testing the tool.

### Train-test split
The data is split into training and testing sets. The user can specify the size of the training set by moving the slider. The default value is 0.8 (80% of the data is used for training).

### Selecting number of folds
The user can select the number of folds for cross-validation. The default value is 5.

### Selecting the classifiers
The user can select the classifiers to train the model on. The following classifiers are available:
- [**Logistic Regression**](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)

- [**Random Forest Classification**](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)

- [**Decision Tree Classifier**](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)

- [**Support Vector Machine (SVM)**](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)

- [**XGBoost**](https://xgboost.readthedocs.io/en/stable/python/python_api.html#xgboost.XGBClassifier)

- [**LightGBM**](https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html#lightgbm.LGBMClassifier)

- [**Ada Boost**](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html)

- [**KNeighbors**](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)

Once the classifiers are selected the models are trained and results reports for each classifier is ourputted. The combined ROC curves for all the selected models is available as well. 

### Saving the model
The models can be saved internally. For that the user needs to select yes in the select box "Would you like to save this model?" in the training results box. Creating a new Experiment or using an existing one and giving a name to the specific run is needed to save the model properly.

## Inference
A trained model can be loaded and used on unlabelled data to predict labels. The user can select the model to load from the dropdown of the previously saved models. The user can also select the data that has been processed with the tool during current session or a sample data with used for testing the tool. Once the model is loaded and the data is selected, the user can click the **Predict** button to make predictions.