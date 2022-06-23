# MNIST Classification

 A machine learning model that classifies handwritten digits, given the handwritten images.
 
Frame the problem: A supervised learning problem because each image is labeled with the digit it represents. This is also a classification problem because the purpose of the model is to classify digits.

Performamnce measures: Accuracy, Confusion Matrix, Precision and Recall and the F1 Score.

Data Understanding: Data was viewed using the CSV reader node, verified data quality by checking for missing values, there were no missing values. Plotted the 300th row of the table and used the Data Row to Image node to view the image.

Data Preparation: Applied the Normalizer node to change the range of the pixels to be between 0 and 1. Also applied the Rule Engine node to create "if statement" : If the label is not 5, then replace the label with "not5".

Modeling: Applied the Logistic Regression Model to the Binary classifier to assign observations to a discrete set of classes. Evaluated the model using Cross-Validation and applied the Classification Threshold Analysis to decide on which threshold to use.

Multi-class Classificatio: Trained the Logistic Regression Model and computed the Macro F1 Score for Macro averaging as it treats all classes equally and is therefore ideal for an imbalanced dataset.

Evaluation: Applied the trained Logistic Regression Model for multi-class classification on the test data set to make predictions with the Logistic Regression Predictor node. Performance measures were obtained using the Scorer(Javascript)node. Finally applied the GroupBy node to compute the Macro F1 Score.

#followed the CRISP-DM framework#
