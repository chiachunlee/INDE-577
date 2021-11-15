## Supervised Learning
------------------------
Machine Learning systems can be classified according to the amount and type of
supervision they get during training. There are four major categories: supervised
learning, unsupervised learning, semisupervised learning, and Reinforcement Learn"
ing.   
In supervised learning, the training data you feed to the algorithm includes the desired
solutions, called labels.   
A typical supervised learning task is classi"cation. The spam filter is a good example
of this: it is trained with many example emails along with their class (spam or ham),
and it must learn how to classify new emails.
Another typical task is to predict a target numeric value, such as the price of a car,
given a set of features (mileage, age, brand, etc.) called predictors. This sort of task is
called regression. To train the system, you need to give it many examples
of cars, including both their predictors and their labels (i.e., their prices). Some regression algorithms can be used for classification as well, and vice
versa. For example, Logistic Regression is commonly used for classification, as it can
output a value that corresponds to the probability of belonging to a given class
