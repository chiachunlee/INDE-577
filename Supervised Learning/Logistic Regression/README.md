### Logistic Regression
Logistic regression models the probabilities for classification problems with two possible outcomes. It’s an extension of the linear regression model for classification problems.   

The linear regression model can work well for regression, but fails for classification. Why is that? In case of two classes, you could label one of the classes with 0 and the other with 1 and use linear regression. Technically it works and most linear model programs will spit out weights for you. But there are a few problems with this approach:
1. A linear model does not output probabilities, but it treats the classes as numbers (0 and 1) and fits the best hyperplane (for a single feature, it is a line) that minimizes the distances between the points and the hyperplane. So it simply interpolates between the points, and you cannot interpret it as probabilities.
2. A linear model also extrapolates and gives you values below zero and above one. This is a good sign that there might be a smarter approach to classification.
3. Since the predicted outcome is not a probability, but a linear interpolation between points, there is no meaningful threshold at which you can distinguish one class from the other.
4. Linear models do not extend to classification problems with multiple classes. You would have to start labeling the next class with 2, then 3, and so on. The classes might not have any meaningful order, but the linear model would force a weird structure on the relationship between the features and your class predictions.   

A solution for classification is logistic regression. Instead of fitting a straight line or hyperplane, the logistic regression model uses the logistic function to squeeze the output of a linear equation between 0 and 1. The logistic function is defined as: <img src="https://render.githubusercontent.com/render/math?math=\sigma(z) = \frac{1}{1%2Be^{-z}}">
 
And it looks like this: <img src="https://christophm.github.io/interpretable-ml-book/images/logistic-function-1.png" width="500"/> <center>It outputs numbers between 0 and 1. At input 0, it outputs 0.5.</center>   
In the linear regression model, we have modelled the relationship between outcome and features with a linear equation: 
<img src="https://render.githubusercontent.com/render/math?math= \hat y^i=	">
\hat y^i=β_{0}+β_{1}x_{1}^i+…+β_{p}x_{p}^i
