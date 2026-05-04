## Hotel Booking Demand Predictive Modeling

**Project Overview:**

The aim of this project is to develop a high-performance classification system to forecast whether a hotel booking will be canceled. This tool will use a dataset of more than 119,000 bookings, and will aim to offer actionable insights to hotel management to enhance their revenue management and staffing efficiency.

**The Data Challenge:**

The dataset will have many different features including lead time, length of stay, number of adults/children and booking channel. One key step in this analysis was the manual elimination of variables of leakage- information that would not be available during the time of prediction- so that the results obtained by the model could be realistic and applicable to actual operations in the real world.

**Methodology and Approach:**

The workflow is split into three parts 70/15/15 and follows a rigorous train-validation-test split. This architecture will make sure that the final model will not only memorize the training data, but also be in a position to generalize to new unseen guests.
All data were preprocessed through a pipeline whereby categorical variables were converted to numerical forms and numeric variables scaled to ensure that all algorithms are fairly weighted.

**Models Tested:**

The project will compare six major classification algorithms:
Logistic Regression (Baseline)
Decision Tree Classifier
Random Forest Classifier
Gradient Boosting Classifier
K-Nearest Neighbors
Support Vector Classifier (Polynomial Kernel).

In order to take performance to the next level, two ensemble techniques were created: a Soft Voting Classifier and a Bayesian Stacking Ensemble. The Stacking Ensemble takes the predictions of the most performant models as inputs to a final "Meta-Model" which uses the inputs to produce the most accurate results possible.
In the evaluation, the Bayesian Stacking Ensemble turned out to be a better option, with a final Test Accuracy of 86.2% and a high ROC-AUC score. Better still, it scored high on Recall rate, i.e. it is especially effective at preventing cancellations. This enables hotel owners to adopt a form of overbooking or special promotions, in order to keep the rooms full.

**Conclusion:**

This project shows the ability of ensemble learning in the hospitality sector. We have made some progress by not merely doing what is right but by actually creating a model that will add some real financial value.
