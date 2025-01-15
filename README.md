# MesotheliomaDiagnosis

My project is on Comprehensive Analysis and Predictive Modeling of Mesothelioma Data available publicly at https://archive.ics.uci.edu/dataset/351/mesothelioma+s+disease+data+setLinks to an external site.

Links to an external site.Objective:  The primary goal of this project is to analyze a dataset related to mesothelioma diagnosis and develop predictive models to classify and understand the progression of the disease. This study aims to identify key features, handle outliers effectively, and utilize machine learning techniques to improve diagnostic accuracy and interpretability.

 

Dataset Description:
Dimensions
Rows (observations): 324
Columns (features): 33, covering a mix of numeric, categorical, and boolean variables . The features are related to: 
Demographics: Age, gender, city of origin.
Exposure History: Duration and intensity of asbestos exposure.
Clinical Features: Symptoms like dyspnea, chest pain, weakness.
Laboratory Data: Total protein, albumin, glucose, pleural fluid WBC, and other biochemical markers.
Target Variable: Binary classification indicating the presence or absence of mesothelioma.
 

Models Used:
To predict the binary outcome (class.of.diagnosis), I propose using the following machine learning models:

Decision Tree:

A simple yet interpretable model to analyze how different features influence the diagnosis.
Useful for visualizing the decision-making process.
Random Forest (Bagging):

An ensemble method that improves accuracy and reduces overfitting by combining multiple decision trees.
Feature importance analysis to identify the most significant predictors.
Gradient Boosting (Boosting):

A more sophisticated ensemble technique that optimizes the model by focusing on misclassified samples.
Implemented using XGBoost for better performance and handling of feature interactions.
Naive Bayes:

A probabilistic model used for comparison, leveraging the assumption of feature independence.
Logistic Regression:

A baseline model for binary classification.
Provides interpretable coefficients to understand the relationship between features and the outcome.
Support Vector Machine (SVM):

A powerful classifier, particularly useful in handling complex boundaries in the feature space.
Heterogeneous Ensemble Model:

Combining predictions from Random Forest, Gradient Boosting, and Logistic Regression to improve overall performance.
 

 

Evaluation Metrics:
I would evaluate the models using: 

Accuracy: Overall correctness of predictions.
Precision and Recall: To handle the imbalance in the dataset.
F1-Score: A harmonic mean of precision and recall.
ROC-AUC: To assess the separability of classes.
 

Anticipated Outcomes:
Identification of key features influencing mesothelioma diagnosis.
Insights into the clinical and biochemical factors contributing to mesothelioma progression.
 

Challenge : Main challenge this dataset poses is the way to handle outliers for skewed distributions. The way each are handled changes the way the model behaves and tweaking them in such a way that performance ascends is quite an exciting challenge I look forward to !

Another hurdle here would be that the dataset has enough observations for training and testing, though the positive class (mesothelioma cases) is smaller, requiring careful handling of class imbalance. 

 

How is this different from actual study: This is my most favorite part of the project !

The study is based on traditional models and serves mid-range accuracy without significant feature transormations. I would use different kinds of models (not used in the original research) to see how the data behaves on those models along with an heterogenous ensemble . My aim is to increase predictive performance using high scoring significant features .
