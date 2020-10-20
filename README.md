# Exploratory-SVM-analysis
Exploratory SVM analysis

## Context

Supervised Machine Learning algorithms i.e. Support vector machines are being used extensively which involves the process of training the model and interpreting the model behaviour. The complexity of understanding the model behaviour w.r.t the trained dataset increases with the increase in the number of support vectors generated. 
The idea here is to optimize the model, for improving model interpretation, by determining the minimal support vectors that effectively represents the original support-vector space, removing the noisy support vectors which may result in overfitting the model.

## Description

The minimal optimal support vectors is determined by recursively removing the original support vectors from train data and re-training the model with resultant dataset and comparing the model results (the confusion-matrix and the accuracy) i.e.
1)	Build a linear SVM and identify the hyperplane for the IoT dataset (D1). Identify the Support Vectors (SV1) that contribute in defining Hyper plane HP1.  Measure Accuracy of the model
2)	Now create a new training dataset (D2) by excluding the identified support vectors (SV1) for the original dataset (D1)
3)	Build a model using the training data obtained in the above step and identify the next set of support Vectors (SV2)
4)	Measure the Accuracy for above and repeat steps 2, 3, 4 till we identify min-imal set of support vectors needed to build the model.

