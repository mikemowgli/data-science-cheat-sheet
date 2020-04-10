# NOTES

* with deep learning, no need to identify features before training the model. The training will auto-discover what features impact the output
* there are as many neurons in the last layer as there are classes to choose from (if use case is to read hand-written digits, there are 10 output classes. If the use-case is to tell is a person is a man or a woman, there could be either 1 output class (one neuron with values 1 for man, 0 for woman), or two output classes (one neuron for man, one for woman). Careful that a different activation function and type of regression must then be used.
* the sigmoid activation function is interesting when multiple neurons of the last layer can have a non-zero value (non-mutually exclusive output)
* the softmax activation fuction is good at setting one output as 1 whereas all others should be set to 0. (mutually exclusive outputs). So 'softmax' is always applied to the output of the last layer when we deal with mutually exclusive classes (example use case: is this flower an iris, a rose or a tulip?)
* the number of inputs is the number of features
* if we need a binary single answer in our last layer, we use a sigmoid activtion function on the last layer so we have 0 if result is negative and 1 if positove.
* Unsupervised learning is when we don't know what are the features we have in the data set (audio recording for instance). We don't have the labels.
  * 'Data mining' is a technique to extract features from the data. It can be done by "clustering" (grouping similar items under the same umbrella), or dimension reduction (or pattern extraction).
* Supervised learning is when we have the labels. Then the problem could be of two types:
  * Regression: if the answer is for instance to predict house prices. The answer to regression problems is a real number. The linear regression is one model that applies to regression typed-problems
  * Classification: when we need to categorize, for instance, fraudulent and non-fraudulent payments. The aneswer is a boolean, on an integer (just the amount of classes). The logistic regression is one model to solve classification problems
* Feature selection: https://www.youtube.com/watch?v=YNgP05M_HVc
* Data preprocessing: https://www.youtube.com/watch?v=bN5aZLp0gvw
* Cross-Validation is the fact that the data set is splitted between training and testing sets
* K-fold crovalidation is when I reshuffle my data set multiple time, apply cross-validation again, and train the model over and over.


### ZTDL tutorial

* Download and install anaconda from anaconda.com

```
$ source /data/tmp/analytics/anaconda3/bin/activate
git clone https://github.com/Dataweekends/zero_to_deep_learning_video.git
$ conda init
$ cd zero_to_deep_learning_video
$ conda create env
$ conda activate ztdl
$ jupyter notebook
```
*  copy token
* create tunnel to 8888
* open local browser to http://localhost:8888
* paste token
