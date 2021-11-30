### K-Nearest Neighbors (KNN)
[K-Nearest Neighbors](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm) (KNN) is a non-parametric classification method. It can be used for classification or regression problems.    

In KNN, the distance between the test data and the training points is used to predict the correct class. Select the K number of points that are closest to the test data, and the KNN algorithm will calculate the probability that the training data belongs to the K number of classes and the class with the greatest probability will be selected. As for the regression problem, regression values are determined by the mean of the K selected training points.  

The output depends on whether K-NN is used for classification or regression:
* In K-NN classification, the output is a class membership. An object is classified by a plurality vote of its neighbors, with the object being assigned to the class most common among its k nearest neighbors (k is a positive integer, typically small). If k = 1, then the object is simply assigned to the class of that single nearest neighbor.
* In k-NN regression, the output is the property value for the object. This value is the average of the values of k nearest neighbors.  

K-NN is a type of classification where the function is only approximated locally and all computation is deferred until function evaluation. Since this algorithm relies on distance for classification, if the features represent different physical units or come in vastly different scales then normalizing the training data can improve its accuracy dramatically. The smaller the K, the more complex of the model. 


![Image of knn1](http://res.cloudinary.com/dyd911kmh/image/upload/f_auto,q_auto:best/v1531424125/KNN_final1_ibdm8a.png)
