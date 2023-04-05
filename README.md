# Deep Neural Networks for Classification using TensorFlow and Keras

## Aim
* To implement deep neural nets (using TensorFlow and Keras) to perform classification

## Approach
* Basic Data Exploration
    - Checks for Class imbalance
    - Checks for Normality
    - Checks for pairwise correlation and multicolinearity
    - Checks for outliers
* Data Preprocessing
    - Scaling
* NN using TF Estimator DNN Classifier
    - Adam optimization
* NN using Keras
    - Model Design: Sequential model with 2 hidden layers and one output layer as follows:

        * Hidden Layer 1: 20 nodes, ReLU activation
        * Hidden Layer 2: 40 nodes, ReLU activation
        * Hidden Layer 2: 15 nodes, ReLU activation
        * OutputLayer: 6 nodes, Softmax activation
    - Adam optimization with categorical cross entropy as the loss function and accuracy as the evaluation metric
    - Trained for 50 epochs

## Conclusion
From the confusion matrix and the value counts of the target label in the original data, we can see that the model has predicted well for the labels which had a dominant representation in the data. Hence the model performance can be improved by balancing the data inorder to have a balanced distribution across all the target labels. This can be achieved by upsampling or downsampling the data.


## Data Used for the Implementation
The data for the classification is from https://archive.ics.uci.edu/ml/datasets/wine+quality and filtered for red-wine only. The actual data has information related to red and white variants of the Portugese "Vinho Verde" wine. See the link for more details.